# Comparing `tmp/tarandm_analytics-0.0.4.tar.gz` & `tmp/tarandm_analytics-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarandm_analytics-0.0.4.tar", max compression
+gzip compressed data, was "tarandm_analytics-0.0.5.tar", max compression
```

## Comparing `tarandm_analytics-0.0.4.tar` & `tarandm_analytics-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1032 2023-07-04 12:44:56.893796 tarandm_analytics-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6370 2023-06-29 09:18:17.981136 tarandm_analytics-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-29 09:18:17.984041 tarandm_analytics-0.0.4/tarandm_analytics/__init__.py
--rw-r--r--   0        0        0     1187 2023-07-04 12:38:00.698987 tarandm_analytics-0.0.4/tarandm_analytics/base.py
--rw-r--r--   0        0        0        0 2023-07-03 15:26:41.279844 tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/__init__.py
--rw-r--r--   0        0        0      207 2023-07-04 06:21:18.742105 tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    19457 2023-07-04 06:49:41.746694 tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc
--rw-r--r--   0        0        0     4023 2023-07-04 06:21:24.012030 tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc
--rw-r--r--   0        0        0    25553 2023-07-04 12:34:53.453053 tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/create_predictive_model.py
--rw-r--r--   0        0        0     4641 2023-06-29 09:18:17.986082 tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/model_visualization.py
--rw-r--r--   0        0        0     6934 1970-01-01 00:00:00.000000 tarandm_analytics-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1033 2023-07-05 14:44:19.539412 tarandm_analytics-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6370 2023-06-29 09:18:17.981136 tarandm_analytics-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 09:18:17.984041 tarandm_analytics-0.0.5/tarandm_analytics/__init__.py
+-rw-r--r--   0        0        0      911 2023-07-05 14:43:36.988316 tarandm_analytics-0.0.5/tarandm_analytics/base.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:26:41.279844 tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-04 06:21:18.742105 tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    19213 2023-07-05 11:50:34.592817 tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc
+-rw-r--r--   0        0        0     4023 2023-07-04 06:21:24.012030 tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc
+-rw-r--r--   0        0        0    25299 2023-07-05 14:43:37.000470 tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/create_predictive_model.py
+-rw-r--r--   0        0        0     4641 2023-06-29 09:18:17.986082 tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/model_visualization.py
+-rw-r--r--   0        0        0     6935 1970-01-01 00:00:00.000000 tarandm_analytics-0.0.5/PKG-INFO
```

### Comparing `tarandm_analytics-0.0.4/pyproject.toml` & `tarandm_analytics-0.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "tarandm_analytics"
-version = "0.0.4"
+version = "0.0.5"
 description = "Package contains support functions for creating predictive models in format compatible with TaranDM software."
 authors = ["Marek Teller <mteller@taran.ai>"]
 readme = "README.md"
 packages = [
     { include = "tarandm_analytics" }
 ]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 pandas = {version = "*", source = "pypi"}
 scikit-learn = {version = "1.2.2", source = "pypi"}
-aiohttp = {version = "*", source = "pypi"}
+requests = {version = "*", source = "pypi"}
 llvmlite = {version = "*", source = "pypi"}
 numba = {version = "==0.56.4", source = "pypi"}
 shap = {version = "*", source = "pypi"}
 matplotlib = {version = "*", source = "pypi"}
 path = {version = "*", source = "pypi"}
 xgboost = {version = "*", source = "pypi"}
 structlog = {version="*", source = "pypi"}
```

### Comparing `tarandm_analytics-0.0.4/README.md` & `tarandm_analytics-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.4/tarandm_analytics/base.py` & `tarandm_analytics-0.0.5/tarandm_analytics/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-import asyncio
-
-import aiohttp
+import requests
 import structlog
-from aiohttp import ClientSession, ClientTimeout
+from requests.auth import HTTPBasicAuth
 
 logger = structlog.get_logger(__name__)
 
 
 class TaranDMAnalytics:
     def __init__(self, endpoint_url: str, username: str, password: str) -> None:
         self.endpoint_url = endpoint_url + ("" if endpoint_url.endswith("/") else "/")
         self.username = username
         self.password = password
 
-        asyncio.ensure_future(self.validate_url())
-
-    async def validate_url(self) -> None:
-        authentication = aiohttp.BasicAuth(login=self.username, password=self.password)
+        self.validate_url()
 
-        async with ClientSession(auth=authentication, timeout=ClientTimeout(total=3)) as session:
-            url = self.endpoint_url + "info"
-            response = await session.get(url=url)
-
-            if response.status == 200:
-                logger.info(f"Connection to {self.endpoint_url} was established.")
-            elif response.status == 401:
-                message = await response.text()
-                logger.error(
-                    f"Authentication failed. Check that provided credentials are correct. Endpoint message: '{message}'"
-                )
+    def validate_url(self) -> None:
+        url = self.endpoint_url + "info"
+        response = requests.get(url=url, auth=HTTPBasicAuth(self.username, self.password))
+
+        if response.status_code == 200:
+            logger.info(f"Connection to {self.endpoint_url} was established.")
+        elif response.status_code == 401:
+            logger.info(f"Connection to {self.endpoint_url} cannot be established. Endpoint error message: "
+                        f"{response.text}")
```

### Comparing `tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc` & `tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 06:49:40 2023 UTC, .py size: 25566 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,1217 +1,1201 @@
-00000000: 6f0d 0d0a 0000 0000 04c1 a364 de63 0000  o..........d.c..
+00000000: 6f0d 0d0a 0000 0000 6256 a564 7063 0000  o.......bV.dpc..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 f600 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 1201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6401 6c06 5a06 6400 6402 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
-00000070: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
-00000080: 6d0d 5a0d 0100 6400 6403 6c01 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000090: 6d0f 5a0f 0100 6400 6404 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
-000000a0: 0100 6400 6405 6c12 6d13 5a13 0100 6400  ..d.d.l.m.Z...d.
-000000b0: 6406 6c14 6d15 5a15 0100 6400 6407 6c16  d.l.m.Z...d.d.l.
-000000c0: 6d17 5a17 0100 6400 6408 6c18 6d19 5a19  m.Z...d.d.l.m.Z.
-000000d0: 0100 6400 6401 6c1a 5a1a 6400 6401 6c1b  ..d.d.l.Z.d.d.l.
-000000e0: 5a1c 6400 6409 6c1d 6d1e 5a1e 6d1f 5a1f  Z.d.d.l.m.Z.m.Z.
-000000f0: 6d20 5a20 6d21 5a21 0100 6400 640a 6c22  m Z m!Z!..d.d.l"
-00000100: 6d23 5a23 0100 6502 a024 6525 a101 5a26  m#Z#..e..$e%..Z&
-00000110: 4700 640b 640c 8400 640c 6523 8303 5a27  G.d.d...d.e#..Z'
-00000120: 6401 5300 290d e900 0000 004e 2906 da04  d.S.)......N)...
-00000130: 4c69 7374 da04 4469 6374 da05 556e 696f  List..Dict..Unio
-00000140: 6eda 084f 7074 696f 6e61 6cda 0341 6e79  n..Optional..Any
-00000150: da05 5475 706c 6529 02da 0d43 6c69 656e  ..Tuple)...Clien
-00000160: 7454 696d 656f 7574 da0d 436c 6965 6e74  tTimeout..Client
-00000170: 5365 7373 696f 6e29 01da 0450 6174 6829  Session)...Path)
-00000180: 01da 1652 616e 646f 6d46 6f72 6573 7443  ...RandomForestC
-00000190: 6c61 7373 6966 6965 7229 01da 124c 6f67  lassifier)...Log
-000001a0: 6973 7469 6352 6567 7265 7373 696f 6e29  isticRegression)
-000001b0: 01da 0742 6f6f 7374 6572 2901 da0d 726f  ...Booster)...ro
-000001c0: 635f 6175 635f 7363 6f72 6529 04da 2573  c_auc_score)..%s
-000001d0: 6861 705f 7375 6d6d 6172 795f 706c 6f74  hap_summary_plot
-000001e0: 5f6c 6f67 6973 7469 635f 7265 6772 6573  _logistic_regres
-000001f0: 7369 6f6e da19 7368 6170 5f73 756d 6d61  sion..shap_summa
-00000200: 7279 5f70 6c6f 745f 7867 626f 6f73 74da  ry_plot_xgboost.
-00000210: 1f73 6861 705f 7375 6d6d 6172 795f 706c  .shap_summary_pl
-00000220: 6f74 5f72 616e 646f 6d5f 666f 7265 7374  ot_random_forest
-00000230: da14 6c65 6172 6e69 6e67 5f63 7572 7665  ..learning_curve
-00000240: 735f 706c 6f74 2901 da10 5461 7261 6e44  s_plot)...TaranD
-00000250: 4d41 6e61 6c79 7469 6373 6300 0000 0000  MAnalyticsc.....
-00000260: 0000 0000 0000 0000 0000 0028 0000 0000  ...........(....
-00000270: 0000 0073 cc02 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000280: 6700 6401 a201 5a03 6402 6504 6403 6504  g.d...Z.d.e.d.e.
-00000290: 6404 6504 6606 8700 6601 6405 6406 840c  d.e.f...f.d.d...
-000002a0: 5a05 6436 6409 640a 8404 5a06 0908 0908  Z.d6d.d...Z.....
-000002b0: 0908 0908 0908 0908 0908 0908 0908 0908  ................
-000002c0: 0908 0908 0908 0908 0908 6437 640b 6507  ..........d7d.e.
-000002d0: 6508 6509 650a 650b 6a0c 6604 1900 640c  e.e.e.e.j.f...d.
-000002e0: 650d 6504 1900 640d 650e 6504 1900 640e  e.e...d.e.e...d.
-000002f0: 650e 6504 1900 640f 650e 650b 6a0c 1900  e.e...d.e.e.j...
-00000300: 6410 650e 6504 1900 6411 650e 6504 1900  d.e.e...d.e.e...
-00000310: 6412 650e 650f 1900 6413 650e 650f 6504  d.e.e...d.e.e.e.
-00000320: 6504 6602 1900 1900 6414 650e 650f 1900  e.f.....d.e.e...
-00000330: 6415 650e 650f 6504 6504 6602 1900 1900  d.e.e.e.e.f.....
-00000340: 6416 650e 6504 1900 6417 650e 6504 1900  d.e.e...d.e.e...
-00000350: 6418 650e 6504 1900 6419 650e 650f 6504  d.e.e...d.e.e.e.
-00000360: 6507 6504 650d 6504 1900 6602 1900 6602  e.e.e.e...f...f.
-00000370: 1900 1900 641a 650e 650f 1900 6407 6510  ....d.e.e...d.e.
-00000380: 650f 6504 6511 6602 1900 650d 650f 6504  e.e.e.f...e.e.e.
-00000390: 6511 6602 1900 1900 6602 1900 6622 641b  e.f.....f...f"d.
-000003a0: 641c 8405 5a12 0908 6438 641d 6504 641e  d...Z...d8d.e.d.
-000003b0: 650e 650d 650f 6504 6511 6602 1900 1900  e.e.e.e.e.f.....
-000003c0: 1900 6407 6408 6606 641f 6420 8405 5a13  ..d.d.f.d.d ..Z.
-000003d0: 6514 0908 6438 6421 6504 6422 6504 641d  e...d8d!e.d"e.d.
-000003e0: 6504 641e 650e 650d 650f 6504 6511 6602  e.d.e.e.e.e.e.f.
-000003f0: 1900 1900 1900 6407 6408 660a 6423 6424  ......d.d.f.d#d$
-00000400: 8405 8301 5a15 6514 6407 6516 6602 6425  ....Z.e.d.e.f.d%
-00000410: 6426 8404 8301 5a17 6407 6516 6602 6427  d&....Z.d.e.f.d'
-00000420: 6428 8404 5a18 640f 650b 6a0c 6416 650e  d(..Z.d.e.j.d.e.
-00000430: 6504 1900 6418 6504 6419 650f 6504 6507  e...d.e.d.e.e.e.
-00000440: 6504 650d 6504 1900 6602 1900 6602 1900  e.e.e...f...f...
-00000450: 6407 650e 650d 650f 6504 6511 6602 1900  d.e.e.e.e.e.f...
-00000460: 1900 1900 660a 6429 642a 8404 5a19 6514  ....f.d)d*..Z.e.
-00000470: 640f 650b 6a0c 6407 6504 6604 642b 642c  d.e.j.d.e.f.d+d,
-00000480: 8404 8301 5a1a 0908 0908 0908 6439 640f  ....Z.......d9d.
-00000490: 650b 6a0c 642d 650e 6504 1900 6416 650e  e.j.d-e.e...d.e.
-000004a0: 6504 1900 6417 650e 6504 1900 6407 650d  e...d.e.e...d.e.
-000004b0: 650f 6504 6511 6602 1900 1900 660a 642e  e.e.e.f.....f.d.
-000004c0: 642f 8405 5a1b 640b 6511 6407 6504 6604  d/..Z.d.e.d.e.f.
-000004d0: 6430 6431 8404 5a1c 6514 640e 6504 6407  d0d1..Z.e.d.e.d.
-000004e0: 6504 6604 6432 6433 8404 8301 5a1d 6514  e.f.d2d3....Z.e.
-000004f0: 0908 0908 643a 640f 650b 6a0c 640c 650d  ....d:d.e.j.d.e.
-00000500: 6504 1900 640b 6511 640e 6504 6411 650e  e...d.e.d.e.d.e.
-00000510: 6504 1900 641a 650e 650f 1900 6407 6510  e...d.e.e...d.e.
-00000520: 650d 650f 1900 650d 650f 1900 6602 1900  e.e...e.e...f...
-00000530: 660e 6434 6435 8405 8301 5a1e 8700 0400  f.d4d5....Z.....
-00000540: 5a1f 5300 293b da15 4578 706f 7274 5072  Z.S.);..ExportPr
-00000550: 6564 6963 7469 7665 4d6f 6465 6c29 04da  edictiveModel)..
-00000560: 0358 4742 da13 4c4f 4749 5354 4943 5f52  .XGB..LOGISTIC_R
-00000570: 4547 5245 5353 494f 4eda 0d52 414e 444f  EGRESSION..RANDO
-00000580: 4d5f 464f 5245 5354 da0c 4558 5045 5254  M_FOREST..EXPERT
-00000590: 5f53 434f 5245 da0c 656e 6470 6f69 6e74  _SCORE..endpoint
-000005a0: 5f75 726c da08 7573 6572 6e61 6d65 da08  _url..username..
-000005b0: 7061 7373 776f 7264 6304 0000 0000 0000  passwordc.......
-000005c0: 0000 0000 0004 0000 0005 0000 0003 0000  ................
-000005d0: 0073 1600 0000 7400 8300 6a01 7c01 7c02  .s....t...j.|.|.
-000005e0: 7c03 6401 8d03 0100 6400 5300 2902 4e29  |.d.....d.S.).N)
-000005f0: 0372 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000600: 2902 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
-00000610: 745f 5f29 04da 0473 656c 6672 1900 0000  t__)...selfr....
-00000620: 721a 0000 0072 1b00 0000 a901 da09 5f5f  r....r........__
-00000630: 636c 6173 735f 5fa9 00fa 8143 3a5c 576f  class__....C:\Wo
-00000640: 726b 5c54 6172 616e 5c47 6974 5c54 6172  rk\Taran\Git\Tar
-00000650: 616e 444d 5c41 6e61 6c79 7469 6373 5c70  anDM\Analytics\p
-00000660: 7265 6469 6374 6976 652d 6d6f 6465 6c2d  redictive-model-
-00000670: 7375 7070 6f72 745c 7461 7261 6e64 6d5f  support\tarandm_
-00000680: 616e 616c 7974 6963 735c 6578 706f 7274  analytics\export
-00000690: 5f70 7265 6469 6374 6976 655f 6d6f 6465  _predictive_mode
-000006a0: 6c5c 6372 6561 7465 5f70 7265 6469 6374  l\create_predict
-000006b0: 6976 655f 6d6f 6465 6c2e 7079 721d 0000  ive_model.pyr...
-000006c0: 0024 0000 0073 0200 0000 1601 7a1e 4578  .$...s......z.Ex
-000006d0: 706f 7274 5072 6564 6963 7469 7665 4d6f  portPredictiveMo
-000006e0: 6465 6c2e 5f5f 696e 6974 5f5f da06 7265  del.__init__..re
-000006f0: 7475 726e 4e63 0100 0000 0000 0000 0000  turnNc..........
-00000700: 0000 0100 0000 0100 0000 c300 0000 7306  ..............s.
-00000710: 0000 0081 0164 0053 00a9 014e 7221 0000  .....d.S...Nr!..
-00000720: 0029 0172 1e00 0000 7221 0000 0072 2100  .).r....r!...r!.
-00000730: 0000 7222 0000 00da 1676 616c 6964 6174  ..r".....validat
-00000740: 655f 616e 616c 7974 6963 735f 7572 6c27  e_analytics_url'
-00000750: 0000 0073 0400 0000 0280 0402 7a2c 4578  ...s........z,Ex
-00000760: 706f 7274 5072 6564 6963 7469 7665 4d6f  portPredictiveMo
-00000770: 6465 6c2e 7661 6c69 6461 7465 5f61 6e61  del.validate_ana
-00000780: 6c79 7469 6373 5f75 726c da05 6d6f 6465  lytics_url..mode
-00000790: 6cda 0a61 7474 7269 6275 7465 73da 0a6d  l..attributes..m
-000007a0: 6f64 656c 5f6e 616d 65da 0a6d 6f64 656c  odel_name..model
-000007b0: 5f74 7970 65da 0464 6174 61da 0a6c 6162  _type..data..lab
-000007c0: 656c 5f6e 616d 65da 0c74 6172 6765 745f  el_name..target_
-000007d0: 636c 6173 73da 1161 7474 7269 6275 7465  class..attribute
-000007e0: 5f62 696e 6e69 6e67 da18 6174 7472 6962  _binning..attrib
-000007f0: 7574 655f 7472 616e 7366 6f72 6d61 7469  ute_transformati
-00000800: 6f6e da0f 6879 7065 7270 6172 616d 6574  on..hyperparamet
-00000810: 6572 73da 1561 7474 7269 6275 7465 5f64  ers..attribute_d
-00000820: 6573 6372 6970 7469 6f6e da12 636f 6c75  escription..colu
-00000830: 6d6e 5f6e 616d 655f 7361 6d70 6c65 da10  mn_name_sample..
-00000840: 636f 6c75 6d6e 5f6e 616d 655f 6461 7465  column_name_date
-00000850: da16 636f 6c75 6d6e 5f6e 616d 655f 7072  ..column_name_pr
-00000860: 6564 6963 7469 6f6e da14 6576 616c 7561  ediction..evalua
-00000870: 7465 5f70 6572 666f 726d 616e 6365 da14  te_performance..
-00000880: 6c65 6172 6e69 6e67 5f63 7572 7665 735f  learning_curves_
-00000890: 6461 7461 6312 0000 0000 0000 0000 0000  datac...........
-000008a0: 001a 0000 0008 0000 0043 0000 0073 f201  .........C...s..
-000008b0: 0000 7c0b 6401 7500 7206 6900 7d0b 7c04  ..|.d.u.r.i.}.|.
-000008c0: 6401 7500 7211 7c00 6a00 7c01 6402 8d01  d.u.r.|.j.|.d...
-000008d0: 7d12 6e1e 7c04 7c00 6a01 7601 722d 7402  }.n.|.|.j.v.r-t.
-000008e0: a003 6403 7c04 9b00 6404 6405 a004 7c00  ..d.|...d.d...|.
-000008f0: 6a01 a101 9b00 6406 9d05 a101 0100 7c00  j.....d.......|.
-00000900: 6a00 7c01 6402 8d01 7d12 6e02 7c04 7d12  j.|.d...}.n.|.}.
-00000910: 7c03 6401 7500 7243 7c00 6a05 7c12 6407  |.d.u.rC|.j.|.d.
-00000920: 8d01 7d13 7402 a003 6408 7c13 9b00 6409  ..}.t...d.|...d.
-00000930: 9d03 a101 0100 6e02 7c03 7d13 7406 a007  ......n.|.}.t...
-00000940: 7c01 a101 7d14 7408 a009 7c14 a101 7d15  |...}.t...|...}.
-00000950: 7c15 a00a 640a a101 7d16 7c16 7c02 7c13  |...d...}.|.|.|.
-00000960: 7c12 640b 9c04 7d17 7c05 6401 7500 7265  |.d...}.|.d.u.re
-00000970: 7402 a003 640c a101 0100 6e17 740b 7c05  t...d.....n.t.|.
-00000980: 8301 640d 6b02 7271 7402 a003 640e a101  ..d.k.rqt...d...
-00000990: 0100 6e0b 7c00 6a0c 7c05 7c06 7c0d 7c0e  ..n.|.j.|.|.|.|.
-000009a0: 640f 8d04 7c17 6410 3c00 7c0b 7282 7c0b  d...|.d.<.|.r.|.
-000009b0: 7c17 6411 3c00 7c0a 7288 7c0a 7c17 6412  |.d.<.|.r.|.|.d.
-000009c0: 3c00 7c06 728e 7c06 7c17 6413 3c00 7c07  <.|.r.|.|.d.<.|.
-000009d0: 7294 7c07 7c17 6414 3c00 7c08 729a 7c08  r.|.|.d.<.|.r.|.
-000009e0: 7c17 6415 3c00 7c09 72a0 7c09 7c17 6416  |.d.<.|.r.|.|.d.
-000009f0: 3c00 7c0c 72a6 7c0c 7c17 6417 3c00 7c10  <.|.r.|.|.d.<.|.
-00000a00: 6401 7501 72e4 7c05 6401 7500 72b4 7402  d.u.r.|.d.u.r.t.
-00000a10: a003 6418 a101 0100 6e30 740b 7c05 8301  ..d.....n0t.|...
-00000a20: 640d 6b02 72c0 7402 a003 6419 a101 0100  d.k.r.t...d.....
-00000a30: 6e24 7c0f 6401 7500 72ca 7402 a003 641a  n$|.d.u.r.t...d.
-00000a40: a101 0100 6e1a 7c0f 7c05 6a0d 7601 72d9  ....n.|.|.j.v.r.
-00000a50: 7402 a003 641b 7c0f 9b00 641c 9d03 a101  t...d.|...d.....
-00000a60: 0100 6e0b 7c00 6a0e 7c05 7c0d 7c0f 7c10  ..n.|.j.|.|.|.|.
-00000a70: 641d 8d04 7c17 641e 3c00 7c00 6a0f 7c05  d...|.d.<.|.j.|.
-00000a80: 7c02 7c01 7c12 7c07 7c11 641f 8d06 5c02  |.|.|.|.|.d...\.
-00000a90: 7d18 7d19 7c19 7c17 6420 3c00 7c17 7c18  }.}.|.|.d <.|.|.
-00000aa0: 6602 5300 2921 610a 1200 0046 756e 6374  f.S.)!a....Funct
-00000ab0: 696f 6e20 7072 6570 6172 6573 2069 6e70  ion prepares inp
-00000ac0: 7574 2064 6174 6120 666f 7220 6275 696c  ut data for buil
-00000ad0: 6420 6d6f 6465 6c20 7a69 7020 6669 6c65  d model zip file
-00000ae0: 2c20 7468 6174 2069 7320 7265 6164 7920  , that is ready 
-00000af0: 746f 2062 6520 696d 706c 656d 656e 7465  to be implemente
-00000b00: 6420 696e 2054 6172 616e 444d 2073 6f66  d in TaranDM sof
-00000b10: 7477 6172 652e 0a20 2020 2020 2020 2043  tware..        C
-00000b20: 7265 6174 6564 2069 6e70 7574 2064 6174  reated input dat
-00000b30: 6120 7769 6c6c 2062 6520 7365 6e74 2074  a will be sent t
-00000b40: 6f20 7468 6520 5461 7261 6e44 4d20 656e  o the TaranDM en
-00000b50: 6470 6f69 6e74 2c20 7468 726f 7567 6820  dpoint, through 
-00000b60: 7768 6963 6820 6669 6e61 6c20 6d6f 6465  which final mode
-00000b70: 6c20 7a69 7020 6669 6c65 2069 7320 7265  l zip file is re
-00000b80: 7475 726e 6564 2e0a 0a20 2020 2020 2020  turned...       
-00000b90: 203a 7061 7261 6d20 6d6f 6465 6c3a 2054   :param model: T
-00000ba0: 7261 696e 6564 2070 7265 6469 6374 6976  rained predictiv
-00000bb0: 6520 6d6f 6465 6c2e 204f 6e65 206f 6620  e model. One of 
-00000bc0: 6672 6f6d 2022 736b 6c65 6172 6e2e 656e  from "sklearn.en
-00000bd0: 7365 6d62 6c65 2e52 616e 646f 6d46 6f72  semble.RandomFor
-00000be0: 6573 7443 6c61 7373 6966 6965 7222 2c0a  estClassifier",.
-00000bf0: 2020 2020 2020 2020 2273 6b6c 6561 726e          "sklearn
-00000c00: 2e6c 696e 6561 725f 6d6f 6465 6c2e 4c6f  .linear_model.Lo
-00000c10: 6769 7374 6963 5265 6772 6573 7369 6f6e  gisticRegression
-00000c20: 222c 2022 7867 626f 6f73 742e 426f 6f73  ", "xgboost.Boos
-00000c30: 7465 7222 2c20 2270 642e 4461 7461 4672  ter", "pd.DataFr
-00000c40: 616d 6522 2e20 2270 642e 4461 7461 4672  ame". "pd.DataFr
-00000c50: 616d 6522 2072 6570 7265 7365 6e74 7320  ame" represents 
-00000c60: 6578 7065 7274 0a20 2020 2020 2020 2073  expert.        s
-00000c70: 636f 7265 6361 7264 206d 6f64 656c 2c20  corecard model, 
-00000c80: 7768 6572 6520 7573 6572 206d 616e 7561  where user manua
-00000c90: 6c6c 7920 6465 6669 6e65 7320 7661 6c75  lly defines valu
-00000ca0: 6573 2066 6f72 2070 7265 6469 6374 6f72  es for predictor
-00000cb0: 2062 696e 732e 0a20 2020 2020 2020 203a   bins..        :
-00000cc0: 7061 7261 6d20 6174 7472 6962 7574 6573  param attributes
-00000cd0: 3a20 4c69 7374 206f 6620 6d6f 6465 6c20  : List of model 
-00000ce0: 7072 6564 6963 746f 7273 2e0a 2020 2020  predictors..    
-00000cf0: 2020 2020 3a70 6172 616d 206d 6f64 656c      :param model
-00000d00: 5f6e 616d 653a 204e 616d 6520 6f66 2074  _name: Name of t
-00000d10: 6865 206d 6f64 656c 2028 7769 6c6c 2062  he model (will b
-00000d20: 6520 7669 7369 626c 6520 696e 2054 6172  e visible in Tar
-00000d30: 616e 444d 2047 5549 292e 0a20 2020 2020  anDM GUI)..     
-00000d40: 2020 203a 7061 7261 6d20 6d6f 6465 6c5f     :param model_
-00000d50: 7479 7065 3a20 5479 7065 206f 6620 7468  type: Type of th
-00000d60: 6520 6d6f 6465 6c2e 204f 6e65 206f 6620  e model. One of 
-00000d70: 2258 4742 222c 2022 4c4f 4749 5354 4943  "XGB", "LOGISTIC
-00000d80: 5f52 4547 5245 5353 494f 4e22 2c20 2252  _REGRESSION", "R
-00000d90: 414e 444f 4d5f 464f 5245 5354 222c 2022  ANDOM_FOREST", "
-00000da0: 4558 5045 5254 5f53 434f 5245 222e 0a20  EXPERT_SCORE".. 
-00000db0: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
-00000dc0: 7461 3a20 4461 7461 7365 7420 7573 6564  ta: Dataset used
-00000dd0: 2066 6f72 206d 6f64 656c 2074 7261 696e   for model train
-00000de0: 696e 672e 2052 6571 7569 7265 6420 746f  ing. Required to
-00000df0: 2063 616c 6375 6c61 7465 206d 6f64 656c   calculate model
-00000e00: 2070 6572 666f 726d 616e 6365 2c20 616e   performance, an
-00000e10: 6420 6465 7363 7269 7074 6976 6520 7374  d descriptive st
-00000e20: 6174 6973 7469 6373 0a20 2020 2020 2020  atistics.       
-00000e30: 2061 626f 7574 2064 6576 656c 6f70 6d65   about developme
-00000e40: 6e74 2073 616d 706c 652e 0a20 2020 2020  nt sample..     
-00000e50: 2020 203a 7061 7261 6d20 6c61 6265 6c5f     :param label_
-00000e60: 6e61 6d65 3a20 4e61 6d65 206f 6620 7468  name: Name of th
-00000e70: 6520 7461 7267 6574 2076 6172 6961 626c  e target variabl
-00000e80: 652e 2053 686f 756c 6420 6265 2069 6e63  e. Should be inc
-00000e90: 6c75 6465 6420 696e 2064 6174 6120 746f  luded in data to
-00000ea0: 2070 726f 7065 726c 7920 6576 616c 7561   properly evalua
-00000eb0: 7465 206d 6f64 656c 2070 6572 666f 726d  te model perform
-00000ec0: 616e 6365 2e0a 2020 2020 2020 2020 3a70  ance..        :p
-00000ed0: 6172 616d 2074 6172 6765 745f 636c 6173  aram target_clas
-00000ee0: 733a 2054 6172 6765 7420 636c 6173 7320  s: Target class 
-00000ef0: 7072 6564 6963 7465 6420 6279 2074 6865  predicted by the
-00000f00: 206d 6f64 656c 2e0a 2020 2020 2020 2020   model..        
-00000f10: 3a70 6172 616d 2061 7474 7269 6275 7465  :param attribute
-00000f20: 5f62 696e 6e69 6e67 3a20 4174 7472 6962  _binning: Attrib
-00000f30: 7574 6520 6269 6e6e 696e 6720 2869 6620  ute binning (if 
-00000f40: 6170 706c 6965 6429 2e20 496e 2069 6e66  applied). In inf
-00000f50: 6572 656e 6365 2070 6861 7365 2c20 7765  erence phase, we
-00000f60: 2066 6972 7374 2061 7070 6c79 2070 7265   first apply pre
-00000f70: 6469 6374 6f72 0a20 2020 2020 2020 2074  dictor.        t
-00000f80: 7261 6e73 666f 726d 6174 696f 6e20 2869  ransformation (i
-00000f90: 6620 6465 6669 6e65 6429 2061 6e64 2074  f defined) and t
-00000fa0: 6865 6e20 6269 6e6e 696e 672e 2052 6573  hen binning. Res
-00000fb0: 756c 7469 6e67 2076 616c 7565 2069 7320  ulting value is 
-00000fc0: 7061 7373 6564 2074 6f20 6d6f 6465 6c20  passed to model 
-00000fd0: 7072 6564 6963 7420 6d65 7468 6f64 2e0a  predict method..
-00000fe0: 0a20 2020 2020 2020 2042 696e 6e69 6e67  .        Binning
-00000ff0: 2073 686f 756c 6420 6265 2070 726f 7669   should be provi
-00001000: 6465 6420 6173 2061 2064 6963 7469 6f6e  ded as a diction
-00001010: 6172 7920 7769 7468 2066 6f6c 6c6f 7769  ary with followi
-00001020: 6e67 2073 7472 7563 7475 7265 3a0a 2020  ng structure:.  
-00001030: 2020 2020 2020 6269 6e6e 696e 6720 3d20        binning = 
-00001040: 7b0a 2020 2020 2020 2020 2020 2020 276e  {.            'n
-00001050: 756d 6572 6963 616c 5f70 7265 6469 6374  umerical_predict
-00001060: 6f72 3127 3a20 7b0a 2020 2020 2020 2020  or1': {.        
-00001070: 2020 2020 2020 2020 2764 7479 7065 273a          'dtype':
-00001080: 2027 4e55 4d45 5249 4341 4c27 2c0a 2020   'NUMERICAL',.  
-00001090: 2020 2020 2020 2020 2020 2020 2020 2762                'b
-000010a0: 696e 7327 3a20 5b2d 6e70 2e69 6e66 2c20  ins': [-np.inf, 
-000010b0: 3230 2c20 3335 2c20 3530 2c20 6e70 2e69  20, 35, 50, np.i
-000010c0: 6e66 5d2c 0a20 2020 2020 2020 2020 2020  nf],.           
-000010d0: 2020 2020 2027 6269 6e5f 7661 6c73 273a       'bin_vals':
-000010e0: 205b 312c 2032 2c20 332c 2034 2c20 3130   [1, 2, 3, 4, 10
-000010f0: 3030 5d2c 0a20 2020 2020 2020 2020 2020  00],.           
-00001100: 2020 2020 2027 6e75 6c6c 5f76 616c 273a       'null_val':
-00001110: 2030 0a20 2020 2020 2020 2020 2020 207d   0.            }
-00001120: 2c0a 2020 2020 2020 2020 2020 2020 2763  ,.            'c
-00001130: 6174 6567 6f72 6963 616c 5f70 7265 6469  ategorical_predi
-00001140: 6374 6f72 3127 3a20 7b0a 2020 2020 2020  ctor1': {.      
-00001150: 2020 2020 2020 2020 2020 2764 7479 7065            'dtype
-00001160: 273a 2027 4341 5445 474f 5249 4341 4c27  ': 'CATEGORICAL'
-00001170: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001180: 2020 2762 696e 7327 3a20 5b5b 274d 275d    'bins': [['M']
-00001190: 2c20 5b27 4627 5d5d 272c 0a20 2020 2020  , ['F']]',.     
-000011a0: 2020 2020 2020 2020 2020 2027 6269 6e5f             'bin_
-000011b0: 7661 6c73 273a 205b 312c 2032 2c20 332c  vals': [1, 2, 3,
-000011c0: 2034 2c20 3130 3030 5d2c 0a20 2020 2020   4, 1000],.     
-000011d0: 2020 2020 2020 2020 2020 2027 6e75 6c6c             'null
-000011e0: 5f76 616c 273a 2030 0a20 2020 2020 2020  _val': 0.       
-000011f0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00001200: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-00001210: 7d0a 2020 2020 2020 2020 4b65 7973 206f  }.        Keys o
-00001220: 6620 7072 6f76 6964 6564 2064 6963 7469  f provided dicti
-00001230: 6f6e 6172 7920 6172 6520 6e61 6d65 7320  onary are names 
-00001240: 6f66 2074 6865 2070 7265 6469 6374 6f72  of the predictor
-00001250: 732e 2054 6172 616e 444d 2073 7570 706f  s. TaranDM suppo
-00001260: 7274 7320 274e 554d 4552 4943 414c 2720  rts 'NUMERICAL' 
-00001270: 616e 6420 2743 4154 4547 4f52 4943 414c  and 'CATEGORICAL
-00001280: 2720 6461 7461 0a20 2020 2020 2020 2074  ' data.        t
-00001290: 7970 6573 206f 6620 7072 6564 6963 746f  ypes of predicto
-000012a0: 7273 2e20 466f 7220 6e75 6d65 7269 6361  rs. For numerica
-000012b0: 6c20 7072 6564 6963 746f 7273 2c20 6269  l predictors, bi
-000012c0: 6e6e 696e 6720 6973 2064 6566 696e 6564  nning is defined
-000012d0: 2062 7920 7072 6f76 6964 696e 6720 6c69   by providing li
-000012e0: 7374 206f 6620 6269 6e20 626f 7264 6572  st of bin border
-000012f0: 732e 2046 6f72 0a20 2020 2020 2020 2063  s. For.        c
-00001300: 6174 6567 6f72 6963 616c 2070 7265 6469  ategorical predi
-00001310: 6374 6f72 732c 2062 696e 6e69 6e67 2069  ctors, binning i
-00001320: 7320 6465 6669 6e65 6420 6279 2070 726f  s defined by pro
-00001330: 7669 6469 6e67 206c 6973 7420 6f66 206c  viding list of l
-00001340: 6973 7473 2e20 496e 6e65 7220 6c69 7374  ists. Inner list
-00001350: 7320 6465 6669 6e65 2076 616c 7565 7320  s define values 
-00001360: 7468 6174 2062 656c 6f6e 670a 2020 2020  that belong.    
-00001370: 2020 2020 746f 2065 6163 6820 6772 6f75      to each grou
-00001380: 702e 2042 6f74 6820 274e 554d 4552 4943  p. Both 'NUMERIC
-00001390: 414c 2720 616e 6420 2743 4154 4547 4f52  AL' and 'CATEGOR
-000013a0: 4943 414c 2720 6461 7461 2074 7970 6573  ICAL' data types
-000013b0: 2063 6f6e 7461 696e 2061 7474 7269 6275   contain attribu
-000013c0: 7465 7320 2762 696e 5f76 616c 7327 2061  tes 'bin_vals' a
-000013d0: 6e64 0a20 2020 2020 2020 2027 6e75 6c6c  nd.        'null
-000013e0: 5f76 616c 272e 2054 686f 7365 2061 7265  _val'. Those are
-000013f0: 2076 616c 7565 7320 7573 6564 2066 6f72   values used for
-00001400: 2065 6e63 6f64 696e 6720 7468 6520 6269   encoding the bi
-00001410: 6e73 2e20 276e 756c 6c5f 7661 6c27 2069  ns. 'null_val' i
-00001420: 7320 616e 2065 6e63 6f64 696e 6720 7661  s an encoding va
-00001430: 6c75 6520 666f 7220 6e75 6c6c 2076 616c  lue for null val
-00001440: 7565 730a 2020 2020 2020 2020 286d 6973  ues.        (mis
-00001450: 7369 6e67 7329 2e0a 0a20 2020 2020 2020  sings)...       
-00001460: 203a 7061 7261 6d20 6174 7472 6962 7574   :param attribut
-00001470: 655f 7472 616e 7366 6f72 6d61 7469 6f6e  e_transformation
-00001480: 3a20 5472 616e 7366 6f72 6d61 7469 6f6e  : Transformation
-00001490: 206f 6620 7468 6520 7072 6564 6963 746f   of the predicto
-000014a0: 7273 2e20 5472 616e 7366 6f72 6d61 7469  rs. Transformati
-000014b0: 6f6e 2069 7320 6170 706c 6965 6420 6265  on is applied be
-000014c0: 666f 7265 2062 696e 6e69 6e67 2e20 4966  fore binning. If
-000014d0: 2062 6f74 680a 2020 2020 2020 2020 7472   both.        tr
-000014e0: 616e 7366 6f72 6d61 7469 6f6e 2061 6e64  ansformation and
-000014f0: 2062 696e 6e69 6e67 2061 7265 2064 6566   binning are def
-00001500: 696e 6564 2c20 7072 6564 6963 746f 7220  ined, predictor 
-00001510: 6973 2066 6972 7374 2074 7261 6e73 666f  is first transfo
-00001520: 726d 6564 2061 6e64 2062 696e 6e69 6e67  rmed and binning
-00001530: 2069 7320 6170 706c 6965 6420 6f76 6572   is applied over
-00001540: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-00001550: 6f62 7461 696e 6564 2061 6674 6572 2074  obtained after t
-00001560: 7261 6e73 666f 726d 6174 696f 6e2e 0a0a  ransformation...
-00001570: 2020 2020 2020 2020 5472 616e 7366 6f72          Transfor
-00001580: 6d61 7469 6f6e 2073 686f 756c 6420 6265  mation should be
-00001590: 2070 726f 7669 6465 6420 6173 2061 2064   provided as a d
-000015a0: 6963 7469 6f6e 6172 7920 7769 7468 2066  ictionary with f
-000015b0: 6f6c 6c6f 7769 6e67 2073 7472 7563 7475  ollowing structu
-000015c0: 7265 3a0a 2020 2020 2020 2020 7472 616e  re:.        tran
-000015d0: 7366 6f72 6d61 7469 6f6e 203d 207b 0a20  sformation = {. 
-000015e0: 2020 2020 2020 2020 2020 2027 6e75 6d65             'nume
-000015f0: 7269 6361 6c5f 7072 6564 6963 746f 7231  rical_predictor1
-00001600: 273a 2027 7b6e 756d 6572 6963 616c 5f70  ': '{numerical_p
-00001610: 7265 6469 6374 6f72 317d 202b 2031 270a  redictor1} + 1'.
-00001620: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00001630: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00001640: 2020 496e 2074 7261 6e73 666f 726d 6174    In transformat
-00001650: 696f 6e20 666f 726d 756c 612c 2061 6e79  ion formula, any
-00001660: 7468 696e 6720 696e 2022 7b7d 2220 6973  thing in "{}" is
-00001670: 2063 6f6e 7369 6465 7265 6420 6173 2070   considered as p
-00001680: 7265 6469 6374 6f72 2061 6e64 2077 696c  redictor and wil
-00001690: 6c20 6265 2072 6570 6c61 6365 6420 7769  l be replaced wi
-000016a0: 7468 2070 7265 6469 6374 6f72 2076 616c  th predictor val
-000016b0: 7565 0a20 2020 2020 2020 2064 7572 696e  ue.        durin
-000016c0: 6720 666f 726d 756c 6120 6576 616c 7561  g formula evalua
-000016d0: 7469 6f6e 2e0a 0a20 2020 2020 2020 203a  tion...        :
-000016e0: 7061 7261 6d20 6879 7065 7270 6172 616d  param hyperparam
-000016f0: 6574 6572 733a 204d 6f64 656c 2068 7970  eters: Model hyp
-00001700: 6572 7061 7261 6d65 7465 7273 2e0a 2020  erparameters..  
-00001710: 2020 2020 2020 3a70 6172 616d 2067 656e        :param gen
-00001720: 6572 616c 5f6e 6f74 6573 3a20 4469 6374  eral_notes: Dict
-00001730: 696f 6e61 7279 206f 6620 6765 6e65 7261  ionary of genera
-00001740: 6c20 6e6f 7465 7320 6162 6f75 7420 7468  l notes about th
-00001750: 6520 6d6f 6465 6c2e 204e 6f74 6573 2077  e model. Notes w
-00001760: 696c 6c20 6265 2064 6973 706c 6179 6564  ill be displayed
-00001770: 2069 6e20 4755 492e 0a20 2020 2020 2020   in GUI..       
-00001780: 203a 7061 7261 6d20 6174 7472 6962 7574   :param attribut
-00001790: 655f 6465 7363 7269 7074 696f 6e3a 2044  e_description: D
-000017a0: 6963 7469 6f6e 6172 7920 7769 7468 2064  ictionary with d
-000017b0: 6573 6372 6970 7469 6f6e 206f 6620 7072  escription of pr
-000017c0: 6564 6963 746f 7273 2e0a 2020 2020 2020  edictors..      
-000017d0: 2020 3a70 6172 616d 2063 6f6c 756d 6e5f    :param column_
-000017e0: 6e61 6d65 5f73 616d 706c 653a 204e 616d  name_sample: Nam
-000017f0: 6520 6f66 2074 6865 2063 6f6c 756d 6e20  e of the column 
-00001800: 696e 2064 6174 612c 2074 6861 7420 6465  in data, that de
-00001810: 6669 6e65 7320 6469 6666 6572 656e 7420  fines different 
-00001820: 6461 7461 2073 616d 706c 6520 7479 7065  data sample type
-00001830: 7320 2874 7261 696e 2c20 7465 7374 2c20  s (train, test, 
-00001840: 6574 632e 292e 0a20 2020 2020 2020 2049  etc.)..        I
-00001850: 6620 7072 6f76 6964 6564 2c20 7361 6d70  f provided, samp
-00001860: 6c65 2073 7461 7469 7374 6963 7320 7769  le statistics wi
-00001870: 6c6c 2062 6520 7374 6f72 6564 2069 6e20  ll be stored in 
-00001880: 6d6f 6465 6c20 6d65 7461 6461 7461 2e0a  model metadata..
-00001890: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-000018a0: 6f6c 756d 6e5f 6e61 6d65 5f64 6174 653a  olumn_name_date:
-000018b0: 204e 616d 6520 6f66 2074 6865 2063 6f6c   Name of the col
-000018c0: 756d 6e20 696e 2064 6174 612c 2074 6861  umn in data, tha
-000018d0: 7420 6465 6669 6e65 7320 7469 6d65 2064  t defines time d
-000018e0: 696d 656e 7369 6f6e 2e20 4966 2070 726f  imension. If pro
-000018f0: 7669 6465 642c 2069 6e66 6f72 6d61 7469  vided, informati
-00001900: 6f6e 2061 626f 7574 0a20 2020 2020 2020  on about.       
-00001910: 2074 696d 6520 7261 6e67 6520 7573 6564   time range used
-00001920: 2069 6e20 6465 7665 6c6f 706d 656e 7420   in development 
-00001930: 7361 6d70 6c65 2064 6174 6120 7769 6c6c  sample data will
-00001940: 2062 6520 7374 6f72 6564 2069 6e20 6d6f   be stored in mo
-00001950: 6465 6c20 6d65 7461 6461 7461 2e0a 2020  del metadata..  
-00001960: 2020 2020 2020 3a70 6172 616d 2063 6f6c        :param col
-00001970: 756d 6e5f 6e61 6d65 5f70 7265 6469 6374  umn_name_predict
-00001980: 696f 6e3a 204e 616d 6520 6f66 2074 6865  ion: Name of the
-00001990: 2063 6f6c 756d 6e20 696e 2064 6174 612c   column in data,
-000019a0: 2074 6861 7420 686f 6c64 7320 6d6f 6465   that holds mode
-000019b0: 6c20 7072 6564 6963 7469 6f6e 2e20 5468  l prediction. Th
-000019c0: 6973 2063 6f6c 756d 6e20 6973 2075 7365  is column is use
-000019d0: 6420 746f 0a20 2020 2020 2020 2065 7661  d to.        eva
-000019e0: 6c75 6174 6520 6d6f 6465 6c20 7065 7266  luate model perf
-000019f0: 6f72 6d61 6e63 652e 0a20 2020 2020 2020  ormance..       
-00001a00: 203a 7061 7261 6d20 6576 616c 7561 7465   :param evaluate
-00001a10: 5f70 6572 666f 726d 616e 6365 3a20 4469  _performance: Di
-00001a20: 6374 696f 6e61 7279 2074 6861 7420 6465  ctionary that de
-00001a30: 6669 6e65 7320 7065 7266 6f72 6d61 6e63  fines performanc
-00001a40: 6520 746f 2062 6520 6576 616c 7561 7465  e to be evaluate
-00001a50: 6420 2d20 7768 6963 6820 7461 7267 6574  d - which target
-00001a60: 2061 6e64 206f 7665 7220 7768 6963 680a   and over which.
-00001a70: 2020 2020 2020 2020 7361 6d70 6c65 2074          sample t
-00001a80: 7970 6573 2e20 5573 6520 666f 6c6c 6f77  ypes. Use follow
-00001a90: 696e 6720 7374 7275 6374 7572 653a 0a0a  ing structure:..
-00001aa0: 2020 2020 2020 2020 6576 616c 7561 7465          evaluate
-00001ab0: 5f70 6572 666f 726d 616e 6365 203d 207b  _performance = {
-00001ac0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00001ad0: 2020 203a 7061 7261 6d20 6c65 6172 6e69     :param learni
-00001ae0: 6e67 5f63 7572 7665 735f 6461 7461 3a20  ng_curves_data: 
-00001af0: 4461 7461 2066 6f72 2070 6c6f 7474 696e  Data for plottin
-00001b00: 6720 6c65 6172 6e69 6e67 2063 7572 7665  g learning curve
-00001b10: 7320 706c 6f74 2069 6e20 666f 6c6c 6f77  s plot in follow
-00001b20: 696e 6720 7374 7275 6374 7572 653a 0a0a  ing structure:..
-00001b30: 2020 2020 2020 2020 6c65 6172 6e69 6e67          learning
-00001b40: 5f63 7572 7665 735f 6461 7461 203d 207b  _curves_data = {
-00001b50: 0a20 2020 2020 2020 2020 2020 2027 7361  .            'sa
-00001b60: 6d70 6c65 3127 3a20 7b0a 2020 2020 2020  mple1': {.      
-00001b70: 2020 2020 2020 2020 2020 276d 6574 7269            'metri
-00001b80: 6331 273a 205b 0a20 2020 2020 2020 2020  c1': [.         
-00001b90: 2020 2020 2020 2020 2020 2030 2e35 2c0a             0.5,.
-00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bb0: 2020 2020 302e 342c 0a20 2020 2020 2020      0.4,.       
-00001bc0: 2020 2020 2020 2020 2020 2020 2030 2e33               0.3
-00001bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001be0: 205d 0a20 2020 2020 2020 2020 2020 207d   ].            }
-00001bf0: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-00001c00: 616d 706c 6532 273a 207b 0a20 2020 2020  ample2': {.     
-00001c10: 2020 2020 2020 2020 2020 2027 6d65 7472             'metr
-00001c20: 6963 3127 3a20 5b0a 2020 2020 2020 2020  ic1': [.        
-00001c30: 2020 2020 2020 2020 2020 2020 302e 362c              0.6,
-00001c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c50: 2020 2020 2030 2e35 2c0a 2020 2020 2020       0.5,.      
-00001c60: 2020 2020 2020 2020 2020 2020 2020 302e                0.
-00001c70: 340a 2020 2020 2020 2020 2020 2020 2020  4.              
-00001c80: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-00001c90: 7d0a 2020 2020 2020 2020 7d0a 2020 2020  }.        }.    
-00001ca0: 2020 2020 3a72 6574 7572 6e3a 0a20 2020      :return:.   
-00001cb0: 2020 2020 204e 2901 7226 0000 007a 0c4d       N).r&...z.M
-00001cc0: 6f64 656c 2074 7970 6520 277a 2927 2069  odel type 'z)' i
-00001cd0: 7320 696e 7661 6c69 642e 2053 7570 706f  s invalid. Suppo
-00001ce0: 7274 6564 206d 6f64 656c 2074 7970 6573  rted model types
-00001cf0: 2061 7265 3a20 fa02 2c20 7a2e 2e20 5769   are: .., z.. Wi
-00001d00: 6c6c 2074 7279 2074 6f20 6465 7465 6374  ll try to detect
-00001d10: 206d 6f64 656c 2074 7970 6520 6175 746f   model type auto
-00001d20: 6d61 7469 6361 6c6c 792e a901 7229 0000  matically...r)..
-00001d30: 007a 344d 6f64 656c 206e 616d 6520 7761  .z4Model name wa
-00001d40: 7320 6e6f 7420 7072 6f76 6964 6564 2e20  s not provided. 
-00001d50: 4765 6e65 7261 7465 6420 6d6f 6465 6c20  Generated model 
-00001d60: 6e61 6d65 3a20 277a 0227 2eda 0561 7363  name: 'z.'...asc
-00001d70: 6969 2904 7226 0000 00da 0a70 7265 6469  ii).r&.....predi
-00001d80: 6374 6f72 7372 2800 0000 7229 0000 007a  ctorsr(...r)...z
-00001d90: 414e 6f20 6461 7461 7365 7420 7761 7320  ANo dataset was 
-00001da0: 7072 6f76 6964 6564 2e20 4361 6e6e 6f74  provided. Cannot
-00001db0: 2065 7661 6c75 6174 6520 7361 6d70 6c65   evaluate sample
-00001dc0: 2064 6573 6372 6970 7469 6f6e 2064 6174   description dat
-00001dd0: 612e 7201 0000 007a 4d50 726f 7669 6465  a.r....zMProvide
-00001de0: 6420 6461 7461 7365 7420 6861 7320 3020  d dataset has 0 
-00001df0: 6f62 7365 7276 6174 696f 6e73 2e20 4361  observations. Ca
-00001e00: 6e6e 6f74 2065 7661 6c75 6174 6520 7361  nnot evaluate sa
-00001e10: 6d70 6c65 2064 6573 6372 6970 7469 6f6e  mple description
-00001e20: 2064 6174 612e 2904 722a 0000 00da 1163   data.).r*.....c
-00001e30: 6f6c 756d 6e5f 6e61 6d65 5f6c 6162 656c  olumn_name_label
-00001e40: 7231 0000 0072 3200 0000 5a17 7361 6d70  r1...r2...Z.samp
-00001e50: 6c65 5f64 6573 6372 6970 7469 6f6e 5f64  le_description_d
-00001e60: 6174 61da 0d67 656e 6572 616c 5f6e 6f74  ata..general_not
-00001e70: 6573 722f 0000 0072 2b00 0000 722c 0000  esr/...r+...r,..
-00001e80: 0072 2d00 0000 722e 0000 0072 3000 0000  .r-...r....r0...
-00001e90: 7a3b 4e6f 2064 6174 6173 6574 2077 6173  z;No dataset was
-00001ea0: 2070 726f 7669 6465 642e 2043 616e 6e6f   provided. Canno
-00001eb0: 7420 6576 616c 7561 7465 206d 6f64 656c  t evaluate model
-00001ec0: 2070 6572 666f 726d 616e 6365 2e7a 4750   performance.zGP
-00001ed0: 726f 7669 6465 6420 6461 7461 7365 7420  rovided dataset 
-00001ee0: 6861 7320 3020 6f62 7365 7276 6174 696f  has 0 observatio
-00001ef0: 6e73 2e20 4361 6e6e 6f74 2065 7661 6c75  ns. Cannot evalu
-00001f00: 6174 6520 6d6f 6465 6c20 7065 7266 6f72  ate model perfor
-00001f10: 6d61 6e63 652e 7a78 4e61 6d65 206f 6620  mance.zxName of 
-00001f20: 7468 6520 636f 6c75 6d6e 7320 7468 6174  the columns that
-00001f30: 2068 6f6c 6473 2070 7265 6469 6374 696f   holds predictio
-00001f40: 6e73 2028 636f 6c75 6d6e 5f6e 616d 655f  ns (column_name_
-00001f50: 7072 6564 6963 7469 6f6e 2920 7761 7320  prediction) was 
-00001f60: 6e6f 7420 7072 6f76 6964 6564 2e20 4361  not provided. Ca
-00001f70: 6e6e 6f74 2065 7661 6c75 6174 6520 6d6f  nnot evaluate mo
-00001f80: 6465 6c20 7065 7266 6f72 6d61 6e63 652e  del performance.
-00001f90: 7a35 5072 6f76 6964 6564 206e 616d 6520  z5Provided name 
-00001fa0: 6f66 2074 6865 2063 6f6c 756d 6e73 2074  of the columns t
-00001fb0: 6861 7420 686f 6c64 7320 7072 6564 6963  hat holds predic
-00001fc0: 7469 6f6e 7320 277a 3427 2069 7320 6e6f  tions 'z4' is no
-00001fd0: 7420 696e 2064 6174 612e 2043 616e 6e6f  t in data. Canno
-00001fe0: 7420 6576 616c 7561 7465 206d 6f64 656c  t evaluate model
-00001ff0: 2070 6572 666f 726d 616e 6365 2e29 0472   performance.).r
-00002000: 2a00 0000 7231 0000 0072 3300 0000 7234  *...r1...r3...r4
-00002010: 0000 005a 116d 6f64 656c 5f70 6572 666f  ...Z.model_perfo
-00002020: 726d 616e 6365 2906 722a 0000 0072 2700  rmance).r*...r'.
-00002030: 0000 7226 0000 0072 2900 0000 722c 0000  ..r&...r)...r,..
-00002040: 0072 3500 0000 5a0f 6174 7461 6368 6564  .r5...Z.attached
-00002050: 5f69 6d61 6765 7329 10da 0f5f 6765 745f  _images)..._get_
-00002060: 6d6f 6465 6c5f 7479 7065 da15 7375 7070  model_type..supp
-00002070: 6f72 7465 645f 6d6f 6465 6c5f 7479 7065  orted_model_type
-00002080: 73da 066c 6f67 6765 72da 0777 6172 6e69  s..logger..warni
-00002090: 6e67 da04 6a6f 696e da14 5f67 656e 6572  ng..join.._gener
-000020a0: 6174 655f 6d6f 6465 6c5f 6e61 6d65 da06  ate_model_name..
-000020b0: 7069 636b 6c65 da05 6475 6d70 73da 0662  pickle..dumps..b
-000020c0: 6173 6536 34da 0962 3634 656e 636f 6465  ase64..b64encode
-000020d0: da06 6465 636f 6465 da03 6c65 6eda 1c5f  ..decode..len.._
-000020e0: 6765 745f 6461 7461 5f73 616d 706c 655f  get_data_sample_
-000020f0: 6465 7363 7269 7074 696f 6eda 0763 6f6c  description..col
-00002100: 756d 6e73 da21 5f67 6574 5f70 7265 6469  umns.!_get_predi
-00002110: 6374 6976 655f 6d6f 6465 6c5f 7065 7266  ctive_model_perf
-00002120: 6f72 6d61 6e63 65da 105f 6765 6e65 7261  ormance.._genera
-00002130: 7465 5f69 6d61 6765 7329 1a72 1e00 0000  te_images).r....
-00002140: 7226 0000 0072 2700 0000 7228 0000 0072  r&...r'...r(...r
-00002150: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
-00002160: 0000 0072 2d00 0000 722e 0000 0072 2f00  ...r-...r....r/.
-00002170: 0000 723b 0000 0072 3000 0000 7231 0000  ..r;...r0...r1..
-00002180: 0072 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
-00002190: 7235 0000 005a 106d 6f64 656c 5f74 7970  r5...Z.model_typ
-000021a0: 655f 6669 6e61 6c5a 106d 6f64 656c 5f6e  e_finalZ.model_n
-000021b0: 616d 655f 6669 6e61 6c5a 0c6d 6f64 656c  ame_finalZ.model
-000021c0: 5f62 696e 6172 795a 146d 6f64 656c 5f62  _binaryZ.model_b
-000021d0: 696e 6172 795f 656e 636f 6465 645a 1b6d  inary_encodedZ.m
-000021e0: 6f64 656c 5f62 696e 6172 795f 656e 636f  odel_binary_enco
-000021f0: 6465 645f 7374 7269 6e67 da0c 7265 7175  ded_string..requ
-00002200: 6573 745f 6461 7461 da06 696d 6167 6573  est_data..images
-00002210: da0b 696d 6167 6573 5f6d 6574 6172 2100  ..images_metar!.
-00002220: 0000 7221 0000 0072 2200 0000 da1d 7072  ..r!...r".....pr
-00002230: 6570 6172 655f 7072 6564 6963 7469 7665  epare_predictive
-00002240: 5f6d 6f64 656c 5f64 6174 612b 0000 0073  _model_data+...s
-00002250: 9a00 0000 0869 0401 0801 0e01 0a01 0401  .....i..........
-00002260: 0801 0a01 06ff 04ff 0e04 0402 0802 0c01  ................
-00002270: 1401 0402 0a02 0a01 0a01 0202 0201 0201  ................
-00002280: 0201 06fc 0807 0c01 0c01 0c01 0402 0201  ................
-00002290: 0201 0201 0201 0afc 0407 0801 0401 0801  ................
-000022a0: 0401 0801 0401 0801 0401 0801 0401 0801  ................
-000022b0: 0401 0801 0802 0801 0c01 0c01 0c01 0801  ................
-000022c0: 0401 0201 06ff 0a04 0401 0a01 06ff 0405  ................
-000022d0: 0201 0201 0201 0201 0afc 0407 0201 0201  ................
-000022e0: 0201 0201 0201 0201 0afa 0808 0802 7a33  ..............z3
-000022f0: 4578 706f 7274 5072 6564 6963 7469 7665  ExportPredictive
-00002300: 4d6f 6465 6c2e 7072 6570 6172 655f 7072  Model.prepare_pr
-00002310: 6564 6963 7469 7665 5f6d 6f64 656c 5f64  edictive_model_d
-00002320: 6174 61da 0866 696c 656e 616d 6572 4d00  ata..filenamerM.
-00002330: 0000 6304 0000 0000 0000 0000 0000 000c  ..c.............
-00002340: 0000 0009 0000 00c3 0000 0073 0801 0000  ...........s....
-00002350: 8101 7c03 6400 7500 7207 6700 7d03 7c00  ..|.d.u.r.g.}.|.
-00002360: 6a00 6401 1700 7d04 7401 6a02 7c00 6a03  j.d...}.t.j.|.j.
-00002370: 7c00 6a04 6402 8d02 7d05 7405 7c05 7406  |.j.d...}.t.|.t.
-00002380: 6403 6404 8d01 6405 8d02 3400 4900 6400  d.d...d...4.I.d.
-00002390: 4800 9a55 7d06 7c06 6a07 7c04 7c01 6406  H..U}.|.j.|.|.d.
-000023a0: 8d02 4900 6400 4800 7d07 7c07 6a08 6407  ..I.d.H.}.|.j.d.
-000023b0: 6b02 723f 7409 a00a 6408 a101 0100 7c07  k.r?t...d.....|.
-000023c0: a00b a100 4900 6400 4800 7d08 6e1d 7c07  ....I.d.H.}.n.|.
-000023d0: a00b a100 4900 6400 4800 7d09 7409 a00c  ....I.d.H.}.t...
-000023e0: 6409 7c09 640a 1900 9b00 9d02 a101 0100  d.|.d...........
-000023f0: 0900 5700 6400 0400 0400 8303 4900 6400  ..W.d.......I.d.
-00002400: 4800 0100 6400 5300 7c08 640b 1900 7d0a  H...d.S.|.d...}.
-00002410: 7c08 640c 1900 7d0b 7c00 a00d 7c0a 7c0b  |.d...}.|...|.|.
-00002420: 7c02 7c03 a104 0100 5700 6400 0400 0400  |.|.....W.d.....
-00002430: 8303 4900 6400 4800 0100 6400 5300 3100  ..I.d.H...d.S.1.
-00002440: 4900 6400 4800 737d 7701 0100 0100 0100  I.d.H.s}w.......
-00002450: 5900 0100 6400 5300 290d 4e7a 2061 6e61  Y...d.S.).Nz ana
-00002460: 6c79 7469 6373 2f62 7569 6c64 5f70 7265  lytics/build_pre
-00002470: 6469 6374 6976 655f 6d6f 6465 6c29 025a  dictive_model).Z
-00002480: 056c 6f67 696e 721b 0000 00e9 1400 0000  .loginr.........
-00002490: 2901 da05 746f 7461 6c29 025a 0461 7574  )...total).Z.aut
-000024a0: 68da 0774 696d 656f 7574 2902 da03 7572  h..timeout)...ur
-000024b0: 6cda 046a 736f 6ee9 c800 0000 7a40 5375  l..json.....z@Su
-000024c0: 6363 6573 7366 756c 6c79 2063 616c 6c65  ccessfully calle
-000024d0: 6420 2761 6e61 6c79 7469 6373 2f62 7569  d 'analytics/bui
-000024e0: 6c64 5f70 7265 6469 6374 6976 655f 6d6f  ld_predictive_mo
-000024f0: 6465 6c27 2065 6e64 706f 696e 742e 7a3c  del' endpoint.z<
-00002500: 556e 6162 6c65 2074 6f20 6361 6c6c 2027  Unable to call '
-00002510: 616e 616c 7974 6963 732f 6275 696c 645f  analytics/build_
-00002520: 7072 6564 6963 7469 7665 5f6d 6f64 656c  predictive_model
-00002530: 2720 656e 6470 6f69 6e74 3a20 da07 6d65  ' endpoint: ..me
-00002540: 7373 6167 655a 1e65 7874 656e 6465 645f  ssageZ.extended_
-00002550: 7072 6564 6963 7469 7665 5f6d 6f64 656c  predictive_model
-00002560: 5f79 616d 6cda 1365 7874 6572 6e61 6c5f  _yaml..external_
-00002570: 6d6f 6465 6c5f 6a73 6f6e 290e 7219 0000  model_json).r...
-00002580: 00da 0761 696f 6874 7470 5a09 4261 7369  ...aiohttpZ.Basi
-00002590: 6341 7574 6872 1a00 0000 721b 0000 0072  cAuthr....r....r
-000025a0: 0900 0000 7208 0000 00da 0367 6574 da06  ....r......get..
-000025b0: 7374 6174 7573 723e 0000 00da 0469 6e66  statusr>.....inf
-000025c0: 6f72 5500 0000 da05 6572 726f 72da 0b73  orU.....error..s
-000025d0: 6176 655f 746f 5f7a 6970 290c 721e 0000  ave_to_zip).r...
-000025e0: 0072 4c00 0000 7250 0000 0072 4d00 0000  .rL...rP...rM...
-000025f0: 7254 0000 005a 0e61 7574 6865 6e74 6963  rT...Z.authentic
-00002600: 6174 696f 6eda 0773 6573 7369 6f6e da08  ation..session..
-00002610: 7265 7370 6f6e 7365 5a0d 7265 7370 6f6e  responseZ.respon
-00002620: 7365 5f64 6174 615a 1072 6573 706f 6e73  se_dataZ.respons
-00002630: 655f 6d65 7373 6167 65da 1365 7874 656e  e_message..exten
-00002640: 6465 645f 6d6f 6465 6c5f 7961 6d6c 7258  ded_model_yamlrX
-00002650: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00002660: 0000 da16 6275 696c 645f 7072 6564 6963  ....build_predic
-00002670: 7469 7665 5f6d 6f64 656c ef00 0000 7324  tive_model....s$
-00002680: 0000 0002 8008 0304 010a 0212 011c 0114  ................
-00002690: 010a 010a 0110 010e 0214 0102 0116 f808  ................
-000026a0: 0908 0112 022e f47a 2c45 7870 6f72 7450  .......z,ExportP
-000026b0: 7265 6469 6374 6976 654d 6f64 656c 2e62  redictiveModel.b
-000026c0: 7569 6c64 5f70 7265 6469 6374 6976 655f  uild_predictive_
-000026d0: 6d6f 6465 6c72 6100 0000 7258 0000 0063  modelra...rX...c
-000026e0: 0400 0000 0000 0000 0000 0000 0a00 0000  ................
-000026f0: 0800 0000 4300 0000 73e8 0000 007c 0364  ....C...s....|.d
-00002700: 0075 0072 0667 007d 0364 0164 0284 007d  .u.r.g.}.d.d...}
-00002710: 0474 00a0 01a1 007d 0574 026a 037c 0564  .t.....}.t.j.|.d
-00002720: 0374 026a 0464 048d 038f 297d 067c 047c  .t.j.d....)}.|.|
-00002730: 0674 00a0 057c 00a1 0164 0583 0301 007c  .t...|...d.....|
-00002740: 047c 0674 00a0 057c 01a1 0164 0683 0301  .|.t...|...d....
-00002750: 007c 0344 005d 0c7d 077c 047c 067c 0764  .|.D.].}.|.|.|.d
-00002760: 0719 007c 0764 0819 0083 0301 0071 2c57  ...|.d.......q,W
-00002770: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
-00002780: 4377 0101 0001 0001 0059 0001 0074 067c  Cw.......Y...t.|
-00002790: 0283 017d 087c 08a0 0764 09a1 0173 557c  ...}.|...d...sU|
-000027a0: 0864 0937 007d 0874 087c 0864 0a83 028f  .d.7.}.t.|.d....
-000027b0: 107d 097c 09a0 097c 05a0 0aa1 00a1 0101  .}.|...|........
-000027c0: 0057 0064 0004 0004 0083 0301 0064 0053  .W.d.........d.S
-000027d0: 0031 0073 6d77 0101 0001 0001 0059 0001  .1.smw.......Y..
-000027e0: 0064 0053 0029 0b4e 6303 0000 0000 0000  .d.S.).Nc.......
-000027f0: 0000 0000 0003 0000 0005 0000 0053 0000  .............S..
-00002800: 0073 5400 0000 7400 7c01 7401 6a02 8302  .sT...t.|.t.j...
-00002810: 7214 7c01 a003 6401 a101 0100 7401 a004  r.|...d.....t...
-00002820: 7c01 a005 a100 a006 a100 a101 7d01 7c01  |...........}.|.
-00002830: a003 6401 7407 6a08 a102 0100 7c01 a003  ..d.t.j.....|...
-00002840: 6401 a101 0100 7c00 a009 7c02 7c01 a00a  d.....|...|.|...
-00002850: a100 a102 0100 6400 5300 2902 4e72 0100  ......d.S.).Nr..
-00002860: 0000 290b da0a 6973 696e 7374 616e 6365  ..)...isinstance
-00002870: da02 696f da08 5374 7269 6e67 494f da04  ..io..StringIO..
-00002880: 7365 656b da07 4279 7465 7349 4fda 0472  seek..BytesIO..r
-00002890: 6561 64da 0665 6e63 6f64 65da 026f 73da  ead..encode..os.
-000028a0: 0853 4545 4b5f 454e 44da 0877 7269 7465  .SEEK_END..write
-000028b0: 7374 72da 0867 6574 7661 6c75 6529 03da  str..getvalue)..
-000028c0: 0761 7263 6869 7665 da06 6275 6666 6572  .archive..buffer
-000028d0: da04 6e61 6d65 7221 0000 0072 2100 0000  ..namer!...r!...
-000028e0: 7222 0000 00da 0861 6464 5f66 696c 650c  r".....add_file.
-000028f0: 0100 0073 0c00 0000 0c01 0a01 1201 0e01  ...s............
-00002900: 0a01 1401 7a33 4578 706f 7274 5072 6564  ....z3ExportPred
-00002910: 6963 7469 7665 4d6f 6465 6c2e 7361 7665  ictiveModel.save
-00002920: 5f74 6f5f 7a69 702e 3c6c 6f63 616c 733e  _to_zip.<locals>
-00002930: 2e61 6464 5f66 696c 65da 0177 2903 da04  .add_file..w)...
-00002940: 6669 6c65 da04 6d6f 6465 da0b 636f 6d70  file..mode..comp
-00002950: 7265 7373 696f 6e7a 1365 7874 656e 6465  ressionz.extende
-00002960: 645f 6d6f 6465 6c2e 7961 6d6c 7a13 6578  d_model.yamlz.ex
-00002970: 7465 726e 616c 5f6d 6f64 656c 2e6a 736f  ternal_model.jso
-00002980: 6eda 0569 6d61 6765 7250 0000 007a 042e  n..imagerP...z..
-00002990: 7a69 70da 0277 6229 0b72 6400 0000 7267  zip..wb).rd...rg
-000029a0: 0000 00da 077a 6970 6669 6c65 da07 5a69  .....zipfile..Zi
-000029b0: 7046 696c 65da 0c5a 4950 5f44 4546 4c41  pFile..ZIP_DEFLA
-000029c0: 5445 4472 6500 0000 720a 0000 00da 0865  TEDre...r......e
-000029d0: 6e64 7377 6974 68da 046f 7065 6eda 0577  ndswith..open..w
-000029e0: 7269 7465 da09 6765 7462 7566 6665 7229  rite..getbuffer)
-000029f0: 0a72 6100 0000 7258 0000 0072 5000 0000  .ra...rX...rP...
-00002a00: 724d 0000 0072 7100 0000 da03 6f75 74da  rM...rq.....out.
-00002a10: 027a 66da 0369 6d67 da04 7061 7468 da01  .zf..img..path..
-00002a20: 6672 2100 0000 7221 0000 0072 2200 0000  fr!...r!...r"...
-00002a30: 725e 0000 0005 0100 0073 2200 0000 0804  r^.......s".....
-00002a40: 0401 0802 0808 1401 1201 1201 0801 1601  ................
-00002a50: 02ff 1cfd 0806 0a01 0801 0c02 1001 22ff  ..............".
-00002a60: 7a21 4578 706f 7274 5072 6564 6963 7469  z!ExportPredicti
-00002a70: 7665 4d6f 6465 6c2e 7361 7665 5f74 6f5f  veModel.save_to_
-00002a80: 7a69 7063 0200 0000 0000 0000 0000 0000  zipc............
-00002a90: 0200 0000 0500 0000 4300 0000 734c 0000  ........C...sL..
-00002aa0: 0074 0074 017c 0083 0183 0164 016b 0272  .t.t.|.....d.k.r
-00002ab0: 0c74 0264 0283 0182 0174 0074 017c 0083  .t.d.....t.t.|..
-00002ac0: 0183 0164 036b 0472 2074 0264 0474 0074  ...d.k.r t.d.t.t
-00002ad0: 017c 0083 0183 019b 0064 059d 0383 0182  .|.......d......
-00002ae0: 0174 037c 007c 0164 068d 0253 0029 074e  .t.|.|.d...S.).N
-00002af0: e901 0000 007a 4c4f 6e6c 7920 6f6e 6520  .....zLOnly one 
-00002b00: 636c 6173 7320 7072 6573 656e 7420 696e  class present in
-00002b10: 2079 5f74 7275 652e 2052 4f43 2041 5543   y_true. ROC AUC
-00002b20: 2073 636f 7265 2069 7320 6e6f 7420 6465   score is not de
-00002b30: 6669 6e65 6420 696e 2074 6861 7420 6361  fined in that ca
-00002b40: 7365 2ee9 0200 0000 7a44 4155 4320 6576  se......zDAUC ev
-00002b50: 616c 7561 7469 6f6e 2073 7570 706f 7274  aluation support
-00002b60: 7320 6f6e 6c79 2062 696e 6172 7920 6c61  s only binary la
-00002b70: 6265 6c73 2e20 5072 6f76 6964 6564 206c  bels. Provided l
-00002b80: 6162 656c 2063 6f6e 7461 696e 7320 7a0e  abel contains z.
-00002b90: 2075 6e69 7175 6520 7661 6c75 6573 2902   unique values).
-00002ba0: da06 795f 7472 7565 da07 795f 7363 6f72  ..y_true..y_scor
-00002bb0: 6529 0472 4700 0000 da03 7365 74da 0a56  e).rG.....set..V
-00002bc0: 616c 7565 4572 726f 7272 0e00 0000 2902  alueErrorr....).
-00002bd0: da05 6c61 6265 6cda 0a70 7265 6469 6374  ..label..predict
-00002be0: 696f 6e72 2100 0000 7221 0000 0072 2200  ionr!...r!...r".
-00002bf0: 0000 da0d 5f65 7661 6c75 6174 655f 6175  ...._evaluate_au
-00002c00: 6322 0100 0073 0e00 0000 1002 0801 1001  c"...s..........
-00002c10: 0201 1201 04ff 0c05 7a23 4578 706f 7274  ........z#Export
-00002c20: 5072 6564 6963 7469 7665 4d6f 6465 6c2e  PredictiveModel.
-00002c30: 5f65 7661 6c75 6174 655f 6175 6363 0300  _evaluate_aucc..
-00002c40: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-00002c50: 0000 4300 0000 7314 0000 0064 017c 00a0  ..C...s....d.|..
-00002c60: 007c 017c 02a1 0214 0064 0218 0053 0029  .|.|.....d...S.)
-00002c70: 034e 7285 0000 0072 8400 0000 2901 728c  .Nr....r....).r.
-00002c80: 0000 0029 0372 1e00 0000 728a 0000 0072  ...).r....r....r
-00002c90: 8b00 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
-00002ca0: 0000 00da 0e5f 6576 616c 7561 7465 5f67  ....._evaluate_g
-00002cb0: 696e 692e 0100 0073 0200 0000 1401 7a24  ini....s......z$
-00002cc0: 4578 706f 7274 5072 6564 6963 7469 7665  ExportPredictive
-00002cd0: 4d6f 6465 6c2e 5f65 7661 6c75 6174 655f  Model._evaluate_
-00002ce0: 6769 6e69 6305 0000 0000 0000 0000 0000  ginic...........
-00002cf0: 000f 0000 000d 0000 0043 0000 0073 3401  .........C...s4.
-00002d00: 0000 7c02 6401 7500 7214 7400 a001 6402  ..|.d.u.r.t...d.
-00002d10: a101 0100 7c00 6a02 7c01 6403 8d01 7d02  ....|.j.|.d...}.
-00002d20: 6404 7c01 7c02 3c00 6e18 7c02 7c01 6a03  d.|.|.<.n.|.|.j.
-00002d30: 7601 722c 7400 a001 6405 7c02 9b00 6406  v.r,t...d.|...d.
-00002d40: 9d03 a101 0100 7c00 6a02 7c01 6403 8d01  ......|.j.|.d...
-00002d50: 7d02 6404 7c01 7c02 3c00 7c00 6a04 7c00  }.d.|.|.<.|.j.|.
-00002d60: 6a05 6407 9c02 7d05 6700 7d06 7c01 7c02  j.d...}.g.}.|.|.
-00002d70: 1900 a006 a100 7d07 7c04 a007 a100 4400  ......}.|.....D.
-00002d80: 5d58 5c02 7d08 7d09 7408 7c09 7409 8302  ]X\.}.}.t.|.t...
-00002d90: 724b 7c09 6701 7d09 7c07 4400 5d49 7d0a  rK|.g.}.|.D.]I}.
-00002da0: 7c01 7c02 1900 7c0a 6b02 7d0b 6900 7d0c  |.|...|.k.}.i.}.
-00002db0: 7c09 4400 5d31 7d0d 7c0d a00a a100 7c05  |.D.]1}.|.....|.
-00002dc0: 7601 7273 7400 a001 6408 7c0d 9b00 6409  v.rst...d.|...d.
-00002dd0: 7c0d 9b00 640a 640b a00b 7c05 a101 9b00  |...d.d...|.....
-00002de0: 9d06 a101 0100 7159 7c05 7c0d a00a a100  ......qY|.|.....
-00002df0: 1900 7c01 7c0b 1900 7c08 1900 7c01 7c0b  ..|.|...|...|.|.
-00002e00: 1900 7c03 1900 8302 7d0e 7c0e 7c0c 7c0d  ..|.....}.|.|.|.
-00002e10: a00a a100 3c00 7159 7c06 a00c 7c08 7c0a  ....<.qY|...|.|.
-00002e20: a00a a100 7c0c 640c 9c03 a101 0100 714d  ....|.d.......qM
-00002e30: 713f 7c06 5300 290d 61f7 0400 000a 2020  q?|.S.).a.....  
-00002e40: 2020 2020 2020 4675 6e63 7469 6f6e 2063        Function c
-00002e50: 616c 6375 6c61 7465 7320 6469 6666 6572  alculates differ
-00002e60: 656e 7420 7065 7266 6f72 6d61 6e63 6520  ent performance 
-00002e70: 6d65 7472 6963 7320 6f66 2070 7265 6469  metrics of predi
-00002e80: 6374 6976 6520 6d6f 6465 6c2e 0a0a 2020  ctive model...  
-00002e90: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
-00002ea0: 613a 2044 6174 6173 6574 2074 6f20 6265  a: Dataset to be
-00002eb0: 2075 7365 6420 666f 7220 6576 616c 7561   used for evalua
-00002ec0: 7469 6e67 2070 6572 666f 726d 616e 6365  ting performance
-00002ed0: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00002ee0: 2063 6f6c 756d 6e5f 6e61 6d65 5f73 616d   column_name_sam
-00002ef0: 706c 653a 204e 616d 6520 6f66 2074 6865  ple: Name of the
-00002f00: 2063 6f6c 756d 6e20 696e 7369 6465 2027   column inside '
-00002f10: 6461 7461 2720 7468 6174 2064 6973 7469  data' that disti
-00002f20: 6e67 7569 7368 6573 2074 7970 6520 6f66  nguishes type of
-00002f30: 2064 6174 6120 7361 6d70 6c65 732e 2043   data samples. C
-00002f40: 6f6c 756d 6e20 6361 6e0a 2020 2020 2020  olumn can.      
-00002f50: 2020 2020 2020 2020 2063 6f6e 7461 696e           contain
-00002f60: 2066 6f72 2069 6e73 7461 6e63 6520 7661   for instance va
-00002f70: 6c75 6573 2027 7472 6169 6e27 2c20 2776  lues 'train', 'v
-00002f80: 616c 6964 272c 2027 7465 7374 272e 2054  alid', 'test'. T
-00002f90: 6869 7320 7769 6c6c 2064 6566 696e 6520  his will define 
-00002fa0: 7768 6963 6820 6f62 7365 7276 6174 696f  which observatio
-00002fb0: 6e73 2062 656c 6f6e 6720 746f 2074 7261  ns belong to tra
-00002fc0: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
-00002fd0: 2020 7365 742c 2076 616c 6964 6174 696f    set, validatio
-00002fe0: 6e20 7365 7420 616e 6420 7465 7374 2073  n set and test s
-00002ff0: 6574 2e0a 2020 2020 2020 2020 3a70 6172  et..        :par
-00003000: 616d 2063 6f6c 756d 6e5f 6e61 6d65 5f70  am column_name_p
-00003010: 7265 6469 6374 696f 6e3a 204e 616d 6520  rediction: Name 
-00003020: 6f66 2074 6865 2063 6f6c 756d 6e20 696e  of the column in
-00003030: 7369 6465 2027 6461 7461 2720 7468 6174  side 'data' that
-00003040: 2068 6f6c 6473 2076 616c 7565 7320 6f66   holds values of
-00003050: 2070 7265 6469 6374 6976 6520 6d6f 6465   predictive mode
-00003060: 6c20 7072 6564 6963 7469 6f6e 2e0a 2020  l prediction..  
-00003070: 2020 2020 2020 3a70 6172 616d 2065 7661        :param eva
-00003080: 6c75 6174 655f 7065 7266 6f72 6d61 6e63  luate_performanc
-00003090: 653a 2044 6963 7469 6f6e 6172 7920 7468  e: Dictionary th
-000030a0: 6174 2064 6566 696e 6573 2077 6861 7420  at defines what 
-000030b0: 6d65 7472 6963 7320 7368 6f75 6c64 2062  metrics should b
-000030c0: 6520 6576 616c 7561 7465 642e 204b 6579  e evaluated. Key
-000030d0: 7320 696e 2064 6963 7469 6f6e 6172 7920  s in dictionary 
-000030e0: 6d75 7374 2072 6566 6572 0a20 2020 2020  must refer.     
-000030f0: 2020 2020 2020 2020 2020 746f 2063 6f6c            to col
-00003100: 756d 6e73 2069 6e20 2764 6174 6127 2074  umns in 'data' t
-00003110: 6861 7420 7769 6c6c 2062 6520 7573 6564  hat will be used
-00003120: 2061 7320 7472 7565 206c 6162 656c 2e20   as true label. 
-00003130: 4d75 6c74 6970 6c65 2074 7275 6520 6c61  Multiple true la
-00003140: 6265 6c20 636f 6c75 6d6e 7320 6361 6e20  bel columns can 
-00003150: 6265 2064 6566 696e 6564 2e20 5468 6973  be defined. This
-00003160: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
-00003170: 2020 2020 2020 2075 7365 6675 6c20 666f         useful fo
-00003180: 7220 696e 7374 616e 6365 2069 6e20 7369  r instance in si
-00003190: 7475 6174 696f 6e73 2077 6865 6e20 7765  tuations when we
-000031a0: 2068 6176 6520 6269 6e61 7279 206c 6162   have binary lab
-000031b0: 656c 7320 2869 6e64 6963 6174 6f72 7320  els (indicators 
-000031c0: 6f66 2061 6e20 6576 656e 7429 2063 616c  of an event) cal
-000031d0: 6375 6c61 7465 6420 6f76 6572 0a20 2020  culated over.   
-000031e0: 2020 2020 2020 2020 2020 2020 6469 6666              diff
-000031f0: 6572 656e 7420 7469 6d65 2077 696e 646f  erent time windo
-00003200: 7773 2e20 496e 2076 616c 7565 7320 756e  ws. In values un
-00003210: 6465 7220 6561 6368 206b 6579 2c20 6d65  der each key, me
-00003220: 7472 6963 7320 746f 2062 6520 6576 616c  trics to be eval
-00003230: 7561 7465 6420 6172 6520 6465 6669 6e65  uated are define
-00003240: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-00003250: 2020 2045 7861 6d70 6c65 3a0a 2020 2020     Example:.    
-00003260: 2020 2020 2020 2020 2020 2065 7661 6c75             evalu
-00003270: 6174 655f 7065 7266 6f72 6d61 6e63 6520  ate_performance 
-00003280: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00003290: 2020 2020 2020 2027 6c61 6265 6c5f 334d         'label_3M
-000032a0: 273a 2027 4155 4327 2c0a 2020 2020 2020  ': 'AUC',.      
-000032b0: 2020 2020 2020 2020 2020 2020 2027 6c61               'la
-000032c0: 6265 6c5f 3132 4d27 3a20 5b27 4155 4327  bel_12M': ['AUC'
-000032d0: 2c20 2747 494e 4927 5d0a 2020 2020 2020  , 'GINI'].      
-000032e0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000032f0: 2020 203a 7265 7475 726e 3a20 4469 6374     :return: Dict
-00003300: 696f 6e61 7279 2077 6974 6820 6361 6c63  ionary with calc
-00003310: 756c 6174 6564 2070 6572 666f 726d 616e  ulated performan
-00003320: 6365 206d 6574 7269 6373 2e0a 2020 2020  ce metrics..    
-00003330: 2020 2020 4e7a 7f45 7661 6c75 6174 696e      Nz.Evaluatin
-00003340: 6720 6d6f 6465 6c20 7065 7266 6f72 6d61  g model performa
-00003350: 6e63 653a 2043 6f6c 756d 6e20 6e61 6d65  nce: Column name
-00003360: 2077 6974 6820 7361 6d70 6c65 2074 7970   with sample typ
-00003370: 6520 7761 7320 6e6f 7420 7072 6f76 6964  e was not provid
-00003380: 6564 2e20 416c 6c20 6f62 7365 7276 6174  ed. All observat
-00003390: 696f 6e73 2077 696c 6c20 6265 2074 7265  ions will be tre
-000033a0: 6174 6564 2061 7320 7472 6169 6e69 6e67  ated as training
-000033b0: 2064 6174 612e a901 722a 0000 00da 0574   data...r*.....t
-000033c0: 7261 696e 7a45 4576 616c 7561 7469 6e67  rainzEEvaluating
-000033d0: 206d 6f64 656c 2070 6572 666f 726d 616e   model performan
-000033e0: 6365 3a20 5072 6f76 6964 6564 2063 6f6c  ce: Provided col
-000033f0: 756d 6e20 6e61 6d65 2077 6974 6820 7361  umn name with sa
-00003400: 6d70 6c65 2074 7970 6520 27fa 4c27 2064  mple type '.L' d
-00003410: 6f65 7320 6e6f 7420 6578 6973 7420 696e  oes not exist in
-00003420: 2064 6174 612e 2041 6c6c 206f 6273 6572   data. All obser
-00003430: 7661 7469 6f6e 7320 7769 6c6c 2062 6520  vations will be 
-00003440: 7472 6561 7465 6420 6173 2074 7261 696e  treated as train
-00003450: 696e 6720 6461 7461 2e29 02da 0341 5543  ing data.)...AUC
-00003460: 5a04 4749 4e49 7a12 5265 7175 6573 7465  Z.GINIz.Requeste
-00003470: 6420 6d65 7472 6963 2027 7a1f 2720 6973  d metric 'z.' is
-00003480: 206e 6f74 2073 7570 706f 7274 6564 2e20   not supported. 
-00003490: 5661 6c75 6520 666f 7220 277a 3a27 2077  Value for 'z:' w
-000034a0: 696c 6c20 6e6f 7420 6265 2073 746f 7265  ill not be store
-000034b0: 642e 2053 7570 706f 7274 6564 2070 6572  d. Supported per
-000034c0: 666f 726d 616e 6365 206d 6574 7269 6365  formance metrice
-000034d0: 7320 6172 653a 2072 3600 0000 2903 da06  s are: r6...)...
-000034e0: 7461 7267 6574 da06 7361 6d70 6c65 da0b  target..sample..
-000034f0: 7065 7266 6f72 6d61 6e63 6529 0d72 3e00  performance).r>.
-00003500: 0000 723f 0000 00da 215f 6765 6e65 7261  ..r?....!_genera
-00003510: 7465 5f73 616d 706c 655f 7479 7065 5f63  te_sample_type_c
-00003520: 6f6c 756d 6e5f 6e61 6d65 7249 0000 0072  olumn_namerI...r
-00003530: 8c00 0000 728d 0000 00da 0675 6e69 7175  ....r......uniqu
-00003540: 65da 0569 7465 6d73 7263 0000 00da 0373  e..itemsrc.....s
-00003550: 7472 da05 7570 7065 7272 4000 0000 da06  tr..upperr@.....
-00003560: 6170 7065 6e64 290f 721e 0000 0072 2a00  append).r....r*.
-00003570: 0000 7231 0000 0072 3300 0000 7234 0000  ..r1...r3...r4..
-00003580: 005a 1f69 6d70 6c65 6d65 6e74 6564 5f70  .Z.implemented_p
-00003590: 6572 666f 726d 616e 6365 5f6d 6574 7269  erformance_metri
-000035a0: 6373 7294 0000 00da 1569 6e63 6c75 6465  csr......include
-000035b0: 645f 7361 6d70 6c65 5f74 7970 6573 728a  d_sample_typesr.
-000035c0: 0000 00da 076d 6574 7269 6373 7293 0000  .....metricsr...
-000035d0: 00da 046d 6173 6b5a 1570 6572 666f 726d  ...maskZ.perform
-000035e0: 616e 6365 5f62 795f 6d65 7472 6963 da06  ance_by_metric..
-000035f0: 6d65 7472 6963 5a0c 6d65 7472 6963 5f76  metricZ.metric_v
-00003600: 616c 7565 7221 0000 0072 2100 0000 7222  aluer!...r!...r"
-00003610: 0000 0072 4a00 0000 3101 0000 7342 0000  ...rJ...1...sB..
-00003620: 0008 1c04 0102 0104 ff0c 040a 010a 0104  ................
-00003630: 010a 0104 ff0c 0408 010e 0204 020c 0110  ................
-00003640: 010a 0106 0108 020c 0104 0108 010c 0104  ................
-00003650: 011a 0106 ff0a 0414 0104 ff0e 0318 0202  ................
-00003660: f204 107a 3745 7870 6f72 7450 7265 6469  ...z7ExportPredi
-00003670: 6374 6976 654d 6f64 656c 2e5f 6765 745f  ctiveModel._get_
-00003680: 7072 6564 6963 7469 7665 5f6d 6f64 656c  predictive_model
-00003690: 5f70 6572 666f 726d 616e 6365 6301 0000  _performancec...
-000036a0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-000036b0: 0043 0000 0073 4000 0000 6401 7c00 6a00  .C...s@...d.|.j.
-000036c0: 7601 7207 6401 5300 7401 6402 6403 8302  v.r.d.S.t.d.d...
-000036d0: 4400 5d11 7d01 6404 7c01 9b00 9d02 7c00  D.].}.d.|.....|.
-000036e0: 6a00 7601 721d 6404 7c01 9b00 9d02 0200  j.v.r.d.|.......
-000036f0: 0100 5300 710c 6405 5300 2906 4e72 9300  ..S.q.d.S.).Nr..
-00003700: 0000 7284 0000 0069 1027 0000 da07 7361  ..r....i.'....sa
-00003710: 6d70 6c65 5f5a 1763 6f6c 756d 6e5f 7769  mple_Z.column_wi
-00003720: 7468 5f73 616d 706c 655f 7479 7065 2902  th_sample_type).
-00003730: 7249 0000 00da 0572 616e 6765 2902 722a  rI.....range).r*
-00003740: 0000 00da 0169 7221 0000 0072 2100 0000  .....ir!...r!...
-00003750: 7222 0000 0072 9500 0000 7601 0000 730e  r"...r....v...s.
-00003760: 0000 000a 0204 010e 0210 010e 0102 ff04  ................
-00003770: 027a 3745 7870 6f72 7450 7265 6469 6374  .z7ExportPredict
-00003780: 6976 654d 6f64 656c 2e5f 6765 6e65 7261  iveModel._genera
-00003790: 7465 5f73 616d 706c 655f 7479 7065 5f63  te_sample_type_c
-000037a0: 6f6c 756d 6e5f 6e61 6d65 723a 0000 0063  olumn_namer:...c
-000037b0: 0500 0000 0000 0000 0000 0000 0e00 0000  ................
-000037c0: 0a00 0000 4300 0000 73f8 0100 007c 0364  ....C...s....|.d
-000037d0: 0175 0072 1474 00a0 0164 02a1 0101 007c  .u.r.t...d.....|
-000037e0: 006a 027c 0164 038d 017d 0364 047c 017c  .j.|.d...}.d.|.|
-000037f0: 033c 006e 187c 037c 016a 0376 0172 2c74  .<.n.|.|.j.v.r,t
-00003800: 00a0 0164 057c 039b 0064 069d 03a1 0101  ...d.|...d......
-00003810: 007c 006a 027c 0164 038d 017d 0364 047c  .|.j.|.d...}.d.|
-00003820: 017c 033c 0064 077d 057c 0464 0175 0072  .|.<.d.}.|.d.u.r
-00003830: 3a74 00a0 0164 08a1 0101 0064 097d 056e  :t...d.....d.}.n
-00003840: 2a7c 047c 016a 0376 0172 4b74 00a0 0164  *|.|.j.v.rKt...d
-00003850: 0a7c 049b 0064 0b9d 03a1 0101 0064 097d  .|...d.......d.}
-00003860: 056e 197c 017c 0419 006a 0464 0c6b 0372  .n.|.|...j.d.k.r
-00003870: 6474 0564 0a7c 049b 0064 0d7c 017c 0419  dt.d.|...d.|.|..
-00003880: 006a 04a0 06a1 009b 0064 0e9d 0583 0101  .j.......d......
-00003890: 0064 097d 0564 077d 0664 077d 077c 0264  .d.}.d.}.d.}.|.d
-000038a0: 0175 0072 7474 00a0 0164 0fa1 0101 0064  .u.rtt...d.....d
-000038b0: 097d 066e 1b7c 027c 016a 0376 0172 8574  .}.n.|.|.j.v.r.t
-000038c0: 00a0 0164 107c 029b 0064 119d 03a1 0101  ...d.|...d......
-000038d0: 0064 097d 066e 0a7c 017c 0219 00a0 07a1  .d.}.n.|.|......
-000038e0: 0064 126b 0372 8f64 097d 077c 017c 0319  .d.k.r.d.}.|.|..
-000038f0: 00a0 08a1 007d 0867 007d 097c 0844 005d  .....}.g.}.|.D.]
-00003900: 607d 0a64 137c 0aa0 09a1 0069 017d 0b7c  `}.d.|.....i.}.|
-00003910: 017c 0319 007c 0a6b 027d 0c74 0a7c 017c  .|...|.k.}.t.|.|
-00003920: 0c19 0083 017c 0b64 143c 007c 0572 cd7c  .....|.d.<.|.r.|
-00003930: 017c 0c19 007c 0419 00a0 0ba1 006a 0c64  .|...|.......j.d
-00003940: 1564 168d 017c 0b64 173c 007c 017c 0c19  .d...|.d.<.|.|..
-00003950: 007c 0419 00a0 0da1 006a 0c64 1564 168d  .|.......j.d.d..
-00003960: 017c 0b64 183c 007c 0672 f47c 0772 f467  .|.d.<.|.r.|.r.g
-00003970: 007c 0b64 193c 007c 017c 0219 00a0 08a1  .|.d.<.|.|......
-00003980: 00a0 0ea1 0044 005d 167d 0d7c 0b64 1919  .....D.].}.|.d..
-00003990: 00a0 0f7c 0d74 0a7c 017c 0c7c 017c 0219  ...|.t.|.|.|.|..
-000039a0: 007c 0d6b 0240 0019 0083 0164 1a9c 02a1  .|.k.@.....d....
-000039b0: 0101 0071 dd7c 09a0 0f7c 0ba1 0101 0071  ...q.|...|.....q
-000039c0: 997c 0953 0029 1b61 3203 0000 0a20 2020  .|.S.).a2....   
-000039d0: 2020 2020 2046 756e 6374 696f 6e20 6576       Function ev
-000039e0: 616c 7561 7465 7320 6469 6666 6572 656e  aluates differen
-000039f0: 7420 6465 7363 7269 7074 6976 6520 696e  t descriptive in
-00003a00: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
-00003a10: 6d6f 6465 6c20 6465 7665 6c6f 706d 656e  model developmen
-00003a20: 7420 6461 7461 2073 616d 706c 652c 2073  t data sample, s
-00003a30: 7563 6820 6173 2077 6861 7420 7469 6d65  uch as what time
-00003a40: 2072 616e 6765 0a20 2020 2020 2020 2077   range.        w
-00003a50: 6173 2075 7365 642c 2077 6861 7420 6172  as used, what ar
-00003a60: 6520 7468 6520 6672 6571 7565 6e63 6965  e the frequencie
-00003a70: 7320 6f66 206c 6162 656c 2063 6c61 7373  s of label class
-00003a80: 6573 2061 6e64 206f 7468 6572 2e0a 0a20  es and other... 
-00003a90: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
-00003aa0: 7461 3a20 4461 7461 7365 7420 746f 2062  ta: Dataset to b
-00003ab0: 6520 7573 6564 2066 6f72 2064 6573 6372  e used for descr
-00003ac0: 6970 7469 7665 2069 6e66 6f20 6576 616c  iptive info eval
-00003ad0: 7561 7469 6f6e 2e0a 2020 2020 2020 2020  uation..        
-00003ae0: 3a70 6172 616d 2063 6f6c 756d 6e5f 6e61  :param column_na
-00003af0: 6d65 5f6c 6162 656c 3a20 4e61 6d65 206f  me_label: Name o
-00003b00: 6620 7468 6520 636f 6c75 6d6e 2069 6e73  f the column ins
-00003b10: 6964 6520 2764 6174 6127 2074 6861 7420  ide 'data' that 
-00003b20: 7374 6f72 6573 206c 6162 656c 732e 0a20  stores labels.. 
-00003b30: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
-00003b40: 6c75 6d6e 5f6e 616d 655f 7361 6d70 6c65  lumn_name_sample
-00003b50: 3a20 4e61 6d65 206f 6620 7468 6520 636f  : Name of the co
-00003b60: 6c75 6d6e 2069 6e73 6964 6520 2764 6174  lumn inside 'dat
-00003b70: 6127 2074 6861 7420 6469 7374 696e 6775  a' that distingu
-00003b80: 6973 6865 7320 7479 7065 206f 6620 6461  ishes type of da
-00003b90: 7461 2073 616d 706c 6573 2e20 436f 6c75  ta samples. Colu
-00003ba0: 6d6e 2063 616e 0a20 2020 2020 2020 2020  mn can.         
-00003bb0: 2020 2020 2020 636f 6e74 6169 6e20 666f        contain fo
-00003bc0: 7220 696e 7374 616e 6365 2076 616c 7565  r instance value
-00003bd0: 7320 2774 7261 696e 272c 2027 7661 6c69  s 'train', 'vali
-00003be0: 6427 2c20 2774 6573 7427 2e20 5468 6973  d', 'test'. This
-00003bf0: 2077 696c 6c20 6465 6669 6e65 2077 6869   will define whi
-00003c00: 6368 206f 6273 6572 7661 7469 6f6e 7320  ch observations 
-00003c10: 6265 6c6f 6e67 2074 6f20 7472 6169 6e0a  belong to train.
-00003c20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003c30: 6574 2c20 7661 6c69 6461 7469 6f6e 2073  et, validation s
-00003c40: 6574 2061 6e64 2074 6573 7420 7365 742e  et and test set.
-00003c50: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00003c60: 636f 6c75 6d6e 5f6e 616d 655f 6461 7465  column_name_date
-00003c70: 3a20 4e61 6d65 206f 6620 7468 6520 636f  : Name of the co
-00003c80: 6c75 6d6e 2069 6e73 6964 6520 2764 6174  lumn inside 'dat
-00003c90: 6127 2074 6861 7420 7374 6f72 6573 2064  a' that stores d
-00003ca0: 6174 6573 2072 656c 6174 6564 2074 6f20  ates related to 
-00003cb0: 6f62 7365 7276 6174 696f 6e73 2e0a 2020  observations..  
-00003cc0: 2020 2020 2020 3a72 6574 7572 6e3a 2044        :return: D
-00003cd0: 6963 7469 6f6e 6172 7920 7769 7468 2064  ictionary with d
-00003ce0: 6573 6372 6970 7469 7665 2069 6e66 6f20  escriptive info 
-00003cf0: 6461 7461 2e0a 2020 2020 2020 2020 4e7a  data..        Nz
-00003d00: 8050 7265 7061 7269 6e67 2073 616d 706c  .Preparing sampl
-00003d10: 6520 6465 7363 7269 7074 696f 6e73 3a20  e descriptions: 
-00003d20: 436f 6c75 6d6e 206e 616d 6520 7769 7468  Column name with
-00003d30: 2073 616d 706c 6520 7479 7065 2077 6173   sample type was
-00003d40: 206e 6f74 2070 726f 7669 6465 642e 2041   not provided. A
-00003d50: 6c6c 206f 6273 6572 7661 7469 6f6e 7320  ll observations 
-00003d60: 7769 6c6c 2062 6520 7472 6561 7465 6420  will be treated 
-00003d70: 6173 2074 7261 696e 696e 6720 6461 7461  as training data
-00003d80: 2e72 8e00 0000 728f 0000 007a 4650 7265  .r....r....zFPre
-00003d90: 7061 7269 6e67 2073 616d 706c 6520 6465  paring sample de
-00003da0: 7363 7269 7074 696f 6e73 3a20 5072 6f76  scriptions: Prov
-00003db0: 6964 6564 2063 6f6c 756d 6e20 6e61 6d65  ided column name
-00003dc0: 2077 6974 6820 7361 6d70 6c65 2074 7970   with sample typ
-00003dd0: 6520 2772 9000 0000 547a 6244 6174 6520  e 'r....TzbDate 
-00003de0: 636f 6c75 6d6e 206e 616d 6520 2863 6f6c  column name (col
-00003df0: 756d 6e5f 6e61 6d65 5f64 6174 6529 2077  umn_name_date) w
-00003e00: 6173 206e 6f74 2070 726f 7669 6465 642e  as not provided.
-00003e10: 2054 696d 6520 7265 6c61 7465 6420 6d65   Time related me
-00003e20: 7461 6461 7461 2077 696c 6c20 6e6f 7420  tadata will not 
-00003e30: 6265 2065 7661 6c75 6174 6564 2e46 7a1b  be evaluated.Fz.
-00003e40: 5072 6f76 6964 6564 2064 6174 6520 636f  Provided date co
-00003e50: 6c75 6d6e 206e 616d 6520 277a 4627 2064  lumn name 'zF' d
-00003e60: 6f65 7320 6e6f 7420 6578 6973 7420 696e  oes not exist in
-00003e70: 2064 6174 612e 2054 696d 6520 7265 6c61   data. Time rela
-00003e80: 7465 6420 6d65 7461 6461 7461 2077 696c  ted metadata wil
-00003e90: 6c20 6e6f 7420 6265 2065 7661 6c75 6174  l not be evaluat
-00003ea0: 6564 2e7a 073c 4d38 5b6e 735d 7a0d 2720  ed.z.<M8[ns]z.' 
-00003eb0: 6973 206f 6620 7479 7065 207a 492e 2052  is of type zI. R
-00003ec0: 6571 7569 7265 6420 7479 7065 2069 7320  equired type is 
-00003ed0: 273c 4d38 5b6e 735d 2e20 5469 6d65 2072  '<M8[ns]. Time r
-00003ee0: 656c 6174 6564 206d 6574 6164 6174 6120  elated metadata 
-00003ef0: 7769 6c6c 206e 6f74 2062 6520 6576 616c  will not be eval
-00003f00: 7561 7465 642e 7a51 4c61 6265 6c20 636f  uated.zQLabel co
-00003f10: 6c75 6d6e 206e 616d 6520 7761 7320 6e6f  lumn name was no
-00003f20: 7420 7072 6f76 6964 6564 2e20 4c61 6265  t provided. Labe
-00003f30: 6c20 7265 6c61 7465 6420 6d65 7461 6461  l related metada
-00003f40: 7461 2077 696c 6c20 6e6f 7420 6265 2065  ta will not be e
-00003f50: 7661 6c75 6174 6564 2e7a 1c50 726f 7669  valuated.z.Provi
-00003f60: 6465 6420 6c61 6265 6c20 636f 6c75 6d6e  ded label column
-00003f70: 206e 616d 6520 277a 4727 2064 6f65 7320   name 'zG' does 
-00003f80: 6e6f 7420 6578 6973 7420 696e 2064 6174  not exist in dat
-00003f90: 612e 204c 6162 656c 2072 656c 6174 6564  a. Label related
-00003fa0: 206d 6574 6164 6174 6120 7769 6c6c 206e   metadata will n
-00003fb0: 6f74 2062 6520 6576 616c 7561 7465 642e  ot be evaluated.
-00003fc0: 7285 0000 00da 0b73 616d 706c 655f 7479  r......sample_ty
-00003fd0: 7065 da16 6e75 6d62 6572 5f6f 665f 6f62  pe..number_of_ob
-00003fe0: 7365 7276 6174 696f 6e73 7a08 2559 2d25  servationsz.%Y-%
-00003ff0: 6d2d 2564 2901 da06 666f 726d 6174 5a0a  m-%d)...formatZ.
-00004000: 6669 7273 745f 6461 7465 5a09 6c61 7374  first_dateZ.last
-00004010: 5f64 6174 655a 156c 6162 656c 5f63 6c61  _dateZ.label_cla
-00004020: 7373 5f66 7265 7175 656e 6379 2902 da0b  ss_frequency)...
-00004030: 6c61 6265 6c5f 636c 6173 7372 a300 0000  label_classr....
-00004040: 2910 723e 0000 0072 3f00 0000 7295 0000  ).r>...r?...r...
-00004050: 0072 4900 0000 da05 6474 7970 65da 0570  .rI.....dtype..p
-00004060: 7269 6e74 da07 5f5f 7374 725f 5fda 076e  rint..__str__..n
-00004070: 756e 6971 7565 7296 0000 0072 9900 0000  uniquer....r....
-00004080: 7247 0000 00da 036d 696e da08 7374 7266  rG.....min..strf
-00004090: 7469 6d65 da03 6d61 78da 0674 6f6c 6973  time..max..tolis
-000040a0: 7472 9a00 0000 290e 721e 0000 0072 2a00  tr....).r....r*.
-000040b0: 0000 723a 0000 0072 3100 0000 7232 0000  ..r:...r1...r2..
-000040c0: 005a 0e64 6174 655f 6176 6169 6c61 626c  .Z.date_availabl
-000040d0: 655a 0f6c 6162 656c 5f61 7661 696c 6162  eZ.label_availab
-000040e0: 6c65 5a0c 6c61 6265 6c5f 6269 6e61 7279  leZ.label_binary
-000040f0: 729b 0000 00da 0672 6573 756c 7472 a200  r......resultr..
-00004100: 0000 5a0b 7361 6d70 6c65 5f6d 6574 6172  ..Z.sample_metar
-00004110: 9d00 0000 72a5 0000 0072 2100 0000 7221  ....r....r!...r!
-00004120: 0000 0072 2200 0000 7248 0000 0080 0100  ...r"...rH......
-00004130: 0073 7600 0000 0813 0401 0201 04ff 0c03  .sv.............
-00004140: 0a01 0a01 0401 0a01 04ff 0c03 0801 0402  ................
-00004150: 0801 0401 0201 04ff 0603 0a01 0401 0a01  ................
-00004160: 04ff 0603 0e01 0201 1a01 04ff 0403 0402  ................
-00004170: 0401 0801 0a01 0601 0a01 0401 0a01 04ff  ................
-00004180: 0603 1001 0401 0c02 0402 0801 0c01 0c01  ................
-00004190: 1001 0402 1c01 1c01 0802 0801 1401 0801  ................
-000041a0: 0202 1601 04fe 06ff 0c06 0402 7a32 4578  ............z2Ex
-000041b0: 706f 7274 5072 6564 6963 7469 7665 4d6f  portPredictiveMo
-000041c0: 6465 6c2e 5f67 6574 5f64 6174 615f 7361  del._get_data_sa
-000041d0: 6d70 6c65 5f64 6573 6372 6970 7469 6f6e  mple_description
-000041e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000041f0: 0003 0000 0043 0000 0073 7200 0000 7400  .....C...sr...t.
-00004200: 7c01 7401 8302 720c 7402 a003 6401 a101  |.t...r.t...d...
-00004210: 0100 6402 5300 7400 7c01 7404 8302 7218  ..d.S.t.|.t...r.
-00004220: 7402 a003 6403 a101 0100 6404 5300 7400  t...d.....d.S.t.
-00004230: 7c01 7405 8302 7224 7402 a003 6405 a101  |.t...r$t...d...
-00004240: 0100 6406 5300 7400 7c01 7406 6a07 8302  ..d.S.t.|.t.j...
-00004250: 7231 7402 a003 6407 a101 0100 6408 5300  r1t...d.....d.S.
-00004260: 7408 6409 7c00 6a09 9b00 9d02 8301 8201  t.d.|.j.........
-00004270: 290a 4e7a 3641 7574 6f6d 6174 6963 616c  ).Nz6Automatical
-00004280: 6c79 2061 7373 6967 6e65 6420 6d6f 6465  ly assigned mode
-00004290: 6c20 7479 7065 204c 4f47 4953 5449 435f  l type LOGISTIC_
-000042a0: 5245 4752 4553 5349 4f4e 2e72 1600 0000  REGRESSION.r....
-000042b0: 7a2d 4175 746f 6d61 7469 6361 6c6c 7920  z-Automatically 
-000042c0: 6164 6465 6420 6d6f 6465 6c20 7479 7065  added model type
-000042d0: 2052 414e 444f 4d5f 464f 5245 5354 2e72   RANDOM_FOREST.r
-000042e0: 1700 0000 7a23 4175 746f 6d61 7469 6361  ....z#Automatica
-000042f0: 6c6c 7920 6164 6465 6420 6d6f 6465 6c20  lly added model 
-00004300: 7479 7065 2058 4742 2e72 1500 0000 7a2c  type XGB.r....z,
-00004310: 4175 746f 6d61 7469 6361 6c6c 7920 6164  Automatically ad
-00004320: 6465 6420 6d6f 6465 6c20 7479 7065 2045  ded model type E
-00004330: 5850 4552 545f 5343 4f52 452e 7218 0000  XPERT_SCORE.r...
-00004340: 007a 5b4d 6f64 656c 2074 7970 6520 7761  .z[Model type wa
-00004350: 7320 6e6f 7420 7072 6f76 6964 6564 2061  s not provided a
-00004360: 6e64 206e 6569 7468 6572 2064 6574 6563  nd neither detec
-00004370: 7465 6420 6175 746f 6d61 7469 6361 6c6c  ted automaticall
-00004380: 792e 2041 7661 696c 6162 6c65 206d 6f64  y. Available mod
-00004390: 656c 2074 7970 6573 2061 7265 3a20 290a  el types are: ).
-000043a0: 7263 0000 0072 0c00 0000 723e 0000 0072  rc...r....r>...r
-000043b0: 5c00 0000 720b 0000 0072 0d00 0000 da02  \...r....r......
-000043c0: 7064 da09 4461 7461 4672 616d 65da 0954  pd..DataFrame..T
-000043d0: 7970 6545 7272 6f72 723d 0000 0029 0272  ypeErrorr=...).r
-000043e0: 1e00 0000 7226 0000 0072 2100 0000 7221  ....r&...r!...r!
-000043f0: 0000 0072 2200 0000 723c 0000 00d7 0100  ...r"...r<......
-00004400: 0073 1e00 0000 0a01 0a01 0401 0a01 0a01  .s..............
-00004410: 0401 0a01 0a01 0401 0c01 0a01 0401 0202  ................
-00004420: 0a01 04ff 7a25 4578 706f 7274 5072 6564  ....z%ExportPred
-00004430: 6963 7469 7665 4d6f 6465 6c2e 5f67 6574  ictiveModel._get
-00004440: 5f6d 6f64 656c 5f74 7970 6563 0100 0000  _model_typec....
-00004450: 0000 0000 0000 0000 0100 0000 0500 0000  ................
-00004460: 4300 0000 731e 0000 007c 00a0 00a1 009b  C...s....|......
-00004470: 0064 0174 016a 01a0 02a1 00a0 0364 02a1  .d.t.j.......d..
-00004480: 019b 009d 0353 0029 034e da01 5f7a 0c25  .....S.).N.._z.%
-00004490: 5925 6d25 6425 4825 4d25 5329 04da 056c  Y%m%d%H%M%S)...l
-000044a0: 6f77 6572 da08 6461 7465 7469 6d65 da03  ower..datetime..
-000044b0: 6e6f 7772 ab00 0000 7237 0000 0072 2100  nowr....r7...r!.
-000044c0: 0000 7221 0000 0072 2200 0000 7241 0000  ..r!...r"...rA..
-000044d0: 00e9 0100 0073 0200 0000 1e02 7a2a 4578  .....s......z*Ex
-000044e0: 706f 7274 5072 6564 6963 7469 7665 4d6f  portPredictiveMo
-000044f0: 6465 6c2e 5f67 656e 6572 6174 655f 6d6f  del._generate_mo
-00004500: 6465 6c5f 6e61 6d65 6306 0000 0000 0000  del_namec.......
-00004510: 0000 0000 000a 0000 000a 0000 0043 0000  .............C..
-00004520: 0073 4401 0000 6700 7d06 6700 7d07 7c03  .sD...g.}.g.}.|.
-00004530: 6401 6b02 7242 7a1c 7400 7c02 7c00 7c01  d.k.rBz.t.|.|.|.
-00004540: 6402 8d03 7d08 7c07 a001 6403 6404 6405  d...}.|...d.d.d.
-00004550: 9c02 a101 0100 7c06 a001 6403 7c08 6406  ......|...d.|.d.
-00004560: 9c02 a101 0100 5700 7c06 7c07 6602 5300  ......W.|.|.f.S.
-00004570: 0400 7402 7941 0100 7d09 0100 7a11 7403  ..t.yA..}...z.t.
-00004580: a004 6407 7c09 9b00 9d02 a101 0100 5700  ..d.|.........W.
-00004590: 5900 6400 7d09 7e09 7c06 7c07 6602 5300  Y.d.}.~.|.|.f.S.
-000045a0: 6400 7d09 7e09 7701 7700 7c03 6408 6b02  d.}.~.w.w.|.d.k.
-000045b0: 7282 7405 7c02 7c00 7c01 6402 8d03 7d08  r.t.|.|.|.d...}.
-000045c0: 7c07 a001 6403 6404 6405 9c02 a101 0100  |...d.d.d.......
-000045d0: 7c06 a001 6403 7c08 6406 9c02 a101 0100  |...d.|.d.......
-000045e0: 7c05 6400 7501 727e 7406 7c05 8301 6409  |.d.u.r~t.|...d.
-000045f0: 6b04 727e 7407 7c02 7c05 6400 640a 8d03  k.r~t.|.|.d.d...
-00004600: 7d08 7c07 a001 640b 640c 6405 9c02 a101  }.|...d.d.d.....
-00004610: 0100 7c06 a001 640b 7c08 6406 9c02 a101  ..|...d.|.d.....
-00004620: 0100 7c06 7c07 6602 5300 7c03 640d 6b02  ..|.|.f.S.|.d.k.
-00004630: 729e 7408 7c02 7c00 7c01 7c04 640e 8d04  r.t.|.|.|.|.d...
-00004640: 7d08 7c07 a001 6403 6404 6405 9c02 a101  }.|...d.d.d.....
-00004650: 0100 7c06 a001 6403 7c08 6406 9c02 a101  ..|...d.|.d.....
-00004660: 0100 7c06 7c07 6602 5300 290f 4e72 1600  ..|.|.f.S.).Nr..
-00004670: 0000 2903 7226 0000 0072 2a00 0000 7227  ..).r&...r*...r'
-00004680: 0000 007a 1073 6861 705f 7375 6d6d 6172  ...z.shap_summar
-00004690: 792e 7376 675a 0c73 6861 705f 7375 6d6d  y.svgZ.shap_summ
-000046a0: 6172 7929 0272 5000 0000 da04 7479 7065  ary).rP.....type
-000046b0: 2902 7250 0000 0072 7600 0000 7a26 4661  ).rP...rv...z&Fa
-000046c0: 696c 6564 2074 6f20 6765 6e65 7261 7465  iled to generate
-000046d0: 2053 6861 7020 7375 6d6d 6172 7920 706c   Shap summary pl
-000046e0: 6f74 3a20 7215 0000 0072 0100 0000 2903  ot: r....r....).
-000046f0: 7226 0000 005a 1265 7661 6c75 6174 696f  r&...Z.evaluatio
-00004700: 6e73 5f72 6573 756c 7472 9e00 0000 7a13  ns_resultr....z.
-00004710: 6c65 6172 6e69 6e67 5f63 7572 7665 732e  learning_curves.
-00004720: 7376 675a 0f6c 6561 726e 696e 675f 6375  svgZ.learning_cu
-00004730: 7276 6573 7217 0000 0029 0472 2600 0000  rvesr....).r&...
-00004740: 722a 0000 0072 2700 0000 722c 0000 0029  r*...r'...r,...)
-00004750: 0972 0f00 0000 729a 0000 00da 0945 7863  .r....r......Exc
-00004760: 6570 7469 6f6e 723e 0000 0072 3f00 0000  eptionr>...r?...
-00004770: 7210 0000 0072 4700 0000 7212 0000 0072  r....rG...r....r
-00004780: 1100 0000 290a 722a 0000 0072 2700 0000  ....).r*...r'...
-00004790: 7226 0000 0072 2900 0000 722c 0000 0072  r&...r)...r,...r
-000047a0: 3500 0000 724d 0000 0072 4e00 0000 7281  5...rM...rN...r.
-000047b0: 0000 00da 0165 7221 0000 0072 2100 0000  .....er!...r!...
-000047c0: 7222 0000 0072 4b00 0000 ed01 0000 733a  r"...rK.......s:
-000047d0: 0000 0004 0904 0108 0102 010e 0110 0112  ................
-000047e0: 0108 130e ee1a 0108 1108 8002 ee08 020e  ................
-000047f0: 0110 0110 0114 020e 0110 0110 0108 0808  ................
-00004800: f902 0108 0106 ff10 0310 0108 027a 2645  .............z&E
-00004810: 7870 6f72 7450 7265 6469 6374 6976 654d  xportPredictiveM
-00004820: 6f64 656c 2e5f 6765 6e65 7261 7465 5f69  odel._generate_i
-00004830: 6d61 6765 7329 0272 2300 0000 4e29 0f4e  mages).r#...N).N
-00004840: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 7224  NNNNNNNNNNNNNNr$
-00004850: 0000 0029 034e 4e4e 2902 4e4e 2920 da08  ...).NNN).NN) ..
-00004860: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00004870: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00004880: 5f5f 723d 0000 0072 9800 0000 721d 0000  __r=...r....r...
-00004890: 0072 2500 0000 7204 0000 0072 0c00 0000  .r%...r....r....
-000048a0: 720b 0000 0072 0d00 0000 72af 0000 0072  r....r....r....r
-000048b0: b000 0000 7202 0000 0072 0500 0000 7203  ....r....r....r.
-000048c0: 0000 0072 0700 0000 7206 0000 0072 4f00  ...r....r....rO.
-000048d0: 0000 7262 0000 00da 0c73 7461 7469 636d  ..rb.....staticm
-000048e0: 6574 686f 6472 5e00 0000 da05 666c 6f61  ethodr^.....floa
-000048f0: 7472 8c00 0000 728d 0000 0072 4a00 0000  tr....r....rJ...
-00004900: 7295 0000 0072 4800 0000 723c 0000 0072  r....rH...r<...r
-00004910: 4100 0000 724b 0000 00da 0d5f 5f63 6c61  A...rK.....__cla
-00004920: 7373 6365 6c6c 5f5f 7221 0000 0072 2100  sscell__r!...r!.
-00004930: 0000 721f 0000 0072 2200 0000 7214 0000  ..r....r"...r...
-00004940: 0021 0000 0073 fe00 0000 0800 0801 1a02  .!...s..........
-00004950: 0a03 0208 0201 0201 0201 0201 0201 0201  ................
-00004960: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00004970: 04ee 1002 02fe 0603 02fd 0604 02fc 0605  ................
-00004980: 02fb 0806 02fa 0607 02f9 0608 02f8 0609  ................
-00004990: 02f7 0e0a 02f6 060b 02f5 0e0d 02f3 060e  ................
-000049a0: 02f2 060f 02f1 0610 02f0 1a11 02ef 0612  ................
-000049b0: 02ee 1e13 0aed 007f 0246 04ff 0201 02ff  .........F......
-000049c0: 1201 02ff 0202 0afe 0216 0202 04ff 0201  ................
-000049d0: 02ff 0201 02ff 0201 02ff 1201 02ff 0202  ................
-000049e0: 0cfe 021c 1001 0e0b 0203 0402 02fe 0603  ................
-000049f0: 02fd 0204 02fc 1605 02fb 1206 0afa 0245  ...............E
-00004a00: 1601 020c 0201 0201 04fb 0402 02fe 0603  ................
-00004a10: 02fd 0604 02fc 0605 02fb 0e06 0afa 1257  ...............W
-00004a20: 0212 1401 0203 0206 0201 04fa 0401 02ff  ................
-00004a30: 0602 02fe 0203 02fd 0204 02fc 0605 02fb  ................
-00004a40: 0606 02fa 1207 14f9 7214 0000 0029 2872  ........r....)(r
-00004a50: b400 0000 7259 0000 005a 0973 7472 7563  ....rY...Z.struc
-00004a60: 746c 6f67 7244 0000 0072 6400 0000 7242  tlogrD...rd...rB
-00004a70: 0000 0072 7800 0000 da06 7479 7069 6e67  ...rx.....typing
-00004a80: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
-00004a90: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
-00004aa0: 0000 0072 0900 0000 7282 0000 0072 0a00  ...r....r....r..
-00004ab0: 0000 da10 736b 6c65 6172 6e2e 656e 7365  ....sklearn.ense
-00004ac0: 6d62 6c65 720b 0000 00da 1473 6b6c 6561  mbler......sklea
-00004ad0: 726e 2e6c 696e 6561 725f 6d6f 6465 6c72  rn.linear_modelr
-00004ae0: 0c00 0000 5a07 7867 626f 6f73 7472 0d00  ....Z.xgboostr..
-00004af0: 0000 da0f 736b 6c65 6172 6e2e 6d65 7472  ....sklearn.metr
-00004b00: 6963 7372 0e00 0000 726a 0000 00da 0670  icsr....rj.....p
-00004b10: 616e 6461 7372 af00 0000 5a3d 7461 7261  andasr....Z=tara
-00004b20: 6e64 6d5f 616e 616c 7974 6963 732e 6578  ndm_analytics.ex
-00004b30: 706f 7274 5f70 7265 6469 6374 6976 655f  port_predictive_
-00004b40: 6d6f 6465 6c2e 6d6f 6465 6c5f 7669 7375  model.model_visu
-00004b50: 616c 697a 6174 696f 6e72 0f00 0000 7210  alizationr....r.
-00004b60: 0000 0072 1100 0000 7212 0000 005a 2374  ...r....r....Z#t
-00004b70: 6172 616e 646d 5f61 6e61 6c79 7469 6373  arandm_analytics
-00004b80: 2e74 6172 616e 646d 5f61 6e61 6c79 7469  .tarandm_analyti
-00004b90: 6373 7213 0000 00da 0a67 6574 5f6c 6f67  csr......get_log
-00004ba0: 6765 7272 b900 0000 723e 0000 0072 1400  gerr....r>...r..
-00004bb0: 0000 7221 0000 0072 2100 0000 7221 0000  ..r!...r!...r!..
-00004bc0: 0072 2200 0000 da08 3c6d 6f64 756c 653e  .r".....<module>
-00004bd0: 0100 0000 7328 0000 0008 0008 0208 0108  ....s(..........
-00004be0: 0208 0108 0108 0120 0110 020c 010c 010c  ....... ........
-00004bf0: 010c 010c 0108 0108 0218 020c 060a 0214  ................
-00004c00: 03                                       .
+00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6401 6c08 5a08 6400 6402 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
+00000080: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
+00000090: 6d0f 5a0f 0100 6400 6403 6c02 6d10 5a10  m.Z...d.d.l.m.Z.
+000000a0: 6d11 5a11 0100 6400 6404 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
+000000b0: 0100 6400 6405 6c14 6d15 5a15 0100 6400  ..d.d.l.m.Z...d.
+000000c0: 6406 6c16 6d17 5a17 0100 6400 6407 6c18  d.l.m.Z...d.d.l.
+000000d0: 6d19 5a19 0100 6400 6408 6c1a 6d1b 5a1b  m.Z...d.d.l.m.Z.
+000000e0: 0100 6400 6409 6c1c 6d1d 5a1d 0100 6400  ..d.d.l.m.Z...d.
+000000f0: 6401 6c1e 5a1e 6400 6401 6c1f 5a20 6400  d.l.Z.d.d.l.Z d.
+00000100: 640a 6c21 6d22 5a22 6d23 5a23 6d24 5a24  d.l!m"Z"m#Z#m$Z$
+00000110: 6d25 5a25 0100 6400 640b 6c26 6d27 5a27  m%Z%..d.d.l&m'Z'
+00000120: 0100 6504 a028 6529 a101 5a2a 4700 640c  ..e..(e)..Z*G.d.
+00000130: 640d 8400 640d 6527 8303 5a2b 6401 5300  d...d.e'..Z+d.S.
+00000140: 290e e900 0000 004e 2906 da04 4c69 7374  )......N)...List
+00000150: da04 4469 6374 da05 556e 696f 6eda 084f  ..Dict..Union..O
+00000160: 7074 696f 6e61 6cda 0341 6e79 da05 5475  ptional..Any..Tu
+00000170: 706c 6529 02da 0d43 6c69 656e 7454 696d  ple)...ClientTim
+00000180: 656f 7574 da0d 436c 6965 6e74 5365 7373  eout..ClientSess
+00000190: 696f 6e29 01da 0450 6174 6829 01da 0d48  ion)...Path)...H
+000001a0: 5454 5042 6173 6963 4175 7468 2901 da16  TTPBasicAuth)...
+000001b0: 5261 6e64 6f6d 466f 7265 7374 436c 6173  RandomForestClas
+000001c0: 7369 6669 6572 2901 da12 4c6f 6769 7374  sifier)...Logist
+000001d0: 6963 5265 6772 6573 7369 6f6e 2901 da07  icRegression)...
+000001e0: 426f 6f73 7465 7229 01da 0d72 6f63 5f61  Booster)...roc_a
+000001f0: 7563 5f73 636f 7265 2904 da25 7368 6170  uc_score)..%shap
+00000200: 5f73 756d 6d61 7279 5f70 6c6f 745f 6c6f  _summary_plot_lo
+00000210: 6769 7374 6963 5f72 6567 7265 7373 696f  gistic_regressio
+00000220: 6eda 1973 6861 705f 7375 6d6d 6172 795f  n..shap_summary_
+00000230: 706c 6f74 5f78 6762 6f6f 7374 da1f 7368  plot_xgboost..sh
+00000240: 6170 5f73 756d 6d61 7279 5f70 6c6f 745f  ap_summary_plot_
+00000250: 7261 6e64 6f6d 5f66 6f72 6573 74da 146c  random_forest..l
+00000260: 6561 726e 696e 675f 6375 7276 6573 5f70  earning_curves_p
+00000270: 6c6f 7429 01da 1054 6172 616e 444d 416e  lot)...TaranDMAn
+00000280: 616c 7974 6963 7363 0000 0000 0000 0000  alyticsc........
+00000290: 0000 0000 0000 0000 2800 0000 0000 0000  ........(.......
+000002a0: 73d8 0200 0065 005a 0164 005a 0267 0064  s....e.Z.d.Z.g.d
+000002b0: 01a2 015a 0364 0265 0464 0365 0464 0465  ...Z.d.e.d.e.d.e
+000002c0: 0466 0687 0066 0164 0564 0684 0c5a 0564  .f...f.d.d...Z.d
+000002d0: 3764 0964 0a84 045a 0609 0809 0809 0809  7d.d...Z........
+000002e0: 0809 0809 0809 0809 0809 0809 0809 0809  ................
+000002f0: 0809 0809 0809 0864 3864 0b65 0765 0865  .......d8d.e.e.e
+00000300: 0965 0a65 0b6a 0c66 0419 0064 0c65 0d65  .e.e.j.f...d.e.e
+00000310: 0419 0064 0d65 0e65 0419 0064 0e65 0e65  ...d.e.e...d.e.e
+00000320: 0419 0064 0f65 0e65 0b6a 0c19 0064 1065  ...d.e.e.j...d.e
+00000330: 0e65 0419 0064 1165 0e65 0419 0064 1265  .e...d.e.e...d.e
+00000340: 0e65 0f19 0064 1365 0e65 0f65 0465 0466  .e...d.e.e.e.e.f
+00000350: 0219 0019 0064 1465 0e65 0f19 0064 1565  .....d.e.e...d.e
+00000360: 0e65 0f65 0465 0466 0219 0019 0064 1665  .e.e.e.f.....d.e
+00000370: 0e65 0419 0064 1765 0e65 0419 0064 1865  .e...d.e.e...d.e
+00000380: 0e65 0419 0064 1965 0e65 0f65 0465 0765  .e...d.e.e.e.e.e
+00000390: 0465 0d65 0419 0066 0219 0066 0219 0019  .e.e...f...f....
+000003a0: 0064 1a65 0e65 0f19 0064 0765 1065 0f65  .d.e.e...d.e.e.e
+000003b0: 0465 1166 0219 0065 0d65 0f65 0465 1166  .e.f...e.e.e.e.f
+000003c0: 0219 0019 0066 0219 0066 2264 1b64 1c84  .....f...f"d.d..
+000003d0: 055a 1209 0864 3964 1d65 0f65 0465 1166  .Z...d9d.e.e.e.f
+000003e0: 0219 0064 1e65 0464 1f65 0e65 0d65 0f65  ...d.e.d.e.e.e.e
+000003f0: 0465 1166 0219 0019 0019 0064 0764 0866  .e.f.......d.d.f
+00000400: 0864 2064 2184 055a 1365 1409 0864 3964  .d d!..Z.e...d9d
+00000410: 2265 0464 2365 0464 1e65 0464 1f65 0e65  "e.d#e.d.e.d.e.e
+00000420: 0d65 0f65 0465 1166 0219 0019 0019 0064  .e.e.e.f.......d
+00000430: 0764 0866 0a64 2464 2584 0583 015a 1565  .d.f.d$d%....Z.e
+00000440: 1464 0765 1666 0264 2664 2784 0483 015a  .d.e.f.d&d'....Z
+00000450: 1764 0765 1666 0264 2864 2984 045a 1864  .d.e.f.d(d)..Z.d
+00000460: 0f65 0b6a 0c64 1665 0e65 0419 0064 1865  .e.j.d.e.e...d.e
+00000470: 0464 1965 0f65 0465 0765 0465 0d65 0419  .d.e.e.e.e.e.e..
+00000480: 0066 0219 0066 0219 0064 0765 0e65 0d65  .f...f...d.e.e.e
+00000490: 0f65 0465 1166 0219 0019 0019 0066 0a64  .e.e.f.......f.d
+000004a0: 2a64 2b84 045a 1965 1464 0f65 0b6a 0c64  *d+..Z.e.d.e.j.d
+000004b0: 0765 0466 0464 2c64 2d84 0483 015a 1a09  .e.f.d,d-....Z..
+000004c0: 0809 0809 0864 3a64 0f65 0b6a 0c64 2e65  .....d:d.e.j.d.e
+000004d0: 0e65 0419 0064 1665 0e65 0419 0064 1765  .e...d.e.e...d.e
+000004e0: 0e65 0419 0064 0765 0d65 0f65 0465 1166  .e...d.e.e.e.e.f
+000004f0: 0219 0019 0066 0a64 2f64 3084 055a 1b64  .....f.d/d0..Z.d
+00000500: 0b65 1164 0765 0466 0464 3164 3284 045a  .e.d.e.f.d1d2..Z
+00000510: 1c65 1464 0e65 0464 0765 0466 0464 3364  .e.d.e.d.e.f.d3d
+00000520: 3484 0483 015a 1d65 1409 0809 0864 3b64  4....Z.e.....d;d
+00000530: 0f65 0b6a 0c64 0c65 0d65 0419 0064 0b65  .e.j.d.e.e...d.e
+00000540: 1164 0e65 0464 1165 0e65 0419 0064 1a65  .d.e.d.e.e...d.e
+00000550: 0e65 0f19 0064 0765 1065 0d65 0f19 0065  .e...d.e.e.e...e
+00000560: 0d65 0f19 0066 0219 0066 0e64 3564 3684  .e...f...f.d5d6.
+00000570: 0583 015a 1e87 0004 005a 1f53 0029 3cda  ...Z.....Z.S.)<.
+00000580: 1545 7870 6f72 7450 7265 6469 6374 6976  .ExportPredictiv
+00000590: 654d 6f64 656c 2904 da03 5847 42da 134c  eModel)...XGB..L
+000005a0: 4f47 4953 5449 435f 5245 4752 4553 5349  OGISTIC_REGRESSI
+000005b0: 4f4e da0d 5241 4e44 4f4d 5f46 4f52 4553  ON..RANDOM_FORES
+000005c0: 54da 0c45 5850 4552 545f 5343 4f52 45da  T..EXPERT_SCORE.
+000005d0: 0c65 6e64 706f 696e 745f 7572 6cda 0875  .endpoint_url..u
+000005e0: 7365 726e 616d 65da 0870 6173 7377 6f72  sername..passwor
+000005f0: 6463 0400 0000 0000 0000 0000 0000 0400  dc..............
+00000600: 0000 0500 0000 0300 0000 7316 0000 0074  ..........s....t
+00000610: 0083 006a 017c 017c 027c 0364 018d 0301  ...j.|.|.|.d....
+00000620: 0064 0053 0029 024e 2903 721a 0000 0072  .d.S.).N).r....r
+00000630: 1b00 0000 721c 0000 0029 02da 0573 7570  ....r....)...sup
+00000640: 6572 da08 5f5f 696e 6974 5f5f 2904 da04  er..__init__)...
+00000650: 7365 6c66 721a 0000 0072 1b00 0000 721c  selfr....r....r.
+00000660: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+00000670: a900 fa81 433a 5c57 6f72 6b5c 5461 7261  ....C:\Work\Tara
+00000680: 6e5c 4769 745c 5461 7261 6e44 4d5c 416e  n\Git\TaranDM\An
+00000690: 616c 7974 6963 735c 7072 6564 6963 7469  alytics\predicti
+000006a0: 7665 2d6d 6f64 656c 2d73 7570 706f 7274  ve-model-support
+000006b0: 5c74 6172 616e 646d 5f61 6e61 6c79 7469  \tarandm_analyti
+000006c0: 6373 5c65 7870 6f72 745f 7072 6564 6963  cs\export_predic
+000006d0: 7469 7665 5f6d 6f64 656c 5c63 7265 6174  tive_model\creat
+000006e0: 655f 7072 6564 6963 7469 7665 5f6d 6f64  e_predictive_mod
+000006f0: 656c 2e70 7972 1e00 0000 2700 0000 7302  el.pyr....'...s.
+00000700: 0000 0016 017a 1e45 7870 6f72 7450 7265  .....z.ExportPre
+00000710: 6469 6374 6976 654d 6f64 656c 2e5f 5f69  dictiveModel.__i
+00000720: 6e69 745f 5fda 0672 6574 7572 6e4e 6301  nit__..returnNc.
+00000730: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000740: 0000 00c3 0000 0073 0600 0000 8101 6400  .......s......d.
+00000750: 5300 a901 4e72 2200 0000 2901 721f 0000  S...Nr"...).r...
+00000760: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
+00000770: da16 7661 6c69 6461 7465 5f61 6e61 6c79  ..validate_analy
+00000780: 7469 6373 5f75 726c 2a00 0000 7304 0000  tics_url*...s...
+00000790: 0002 8004 027a 2c45 7870 6f72 7450 7265  .....z,ExportPre
+000007a0: 6469 6374 6976 654d 6f64 656c 2e76 616c  dictiveModel.val
+000007b0: 6964 6174 655f 616e 616c 7974 6963 735f  idate_analytics_
+000007c0: 7572 6cda 056d 6f64 656c da0a 6174 7472  url..model..attr
+000007d0: 6962 7574 6573 da0a 6d6f 6465 6c5f 6e61  ibutes..model_na
+000007e0: 6d65 da0a 6d6f 6465 6c5f 7479 7065 da04  me..model_type..
+000007f0: 6461 7461 da0a 6c61 6265 6c5f 6e61 6d65  data..label_name
+00000800: da0c 7461 7267 6574 5f63 6c61 7373 da11  ..target_class..
+00000810: 6174 7472 6962 7574 655f 6269 6e6e 696e  attribute_binnin
+00000820: 67da 1861 7474 7269 6275 7465 5f74 7261  g..attribute_tra
+00000830: 6e73 666f 726d 6174 696f 6eda 0f68 7970  nsformation..hyp
+00000840: 6572 7061 7261 6d65 7465 7273 da15 6174  erparameters..at
+00000850: 7472 6962 7574 655f 6465 7363 7269 7074  tribute_descript
+00000860: 696f 6eda 1263 6f6c 756d 6e5f 6e61 6d65  ion..column_name
+00000870: 5f73 616d 706c 65da 1063 6f6c 756d 6e5f  _sample..column_
+00000880: 6e61 6d65 5f64 6174 65da 1663 6f6c 756d  name_date..colum
+00000890: 6e5f 6e61 6d65 5f70 7265 6469 6374 696f  n_name_predictio
+000008a0: 6eda 1465 7661 6c75 6174 655f 7065 7266  n..evaluate_perf
+000008b0: 6f72 6d61 6e63 65da 146c 6561 726e 696e  ormance..learnin
+000008c0: 675f 6375 7276 6573 5f64 6174 6163 1200  g_curves_datac..
+000008d0: 0000 0000 0000 0000 0000 1a00 0000 0800  ................
+000008e0: 0000 4300 0000 73f2 0100 007c 0b64 0175  ..C...s....|.d.u
+000008f0: 0072 0669 007d 0b7c 0464 0175 0072 117c  .r.i.}.|.d.u.r.|
+00000900: 006a 007c 0164 028d 017d 126e 1e7c 047c  .j.|.d...}.n.|.|
+00000910: 006a 0176 0172 2d74 02a0 0364 037c 049b  .j.v.r-t...d.|..
+00000920: 0064 0464 05a0 047c 006a 01a1 019b 0064  .d.d...|.j.....d
+00000930: 069d 05a1 0101 007c 006a 007c 0164 028d  .......|.j.|.d..
+00000940: 017d 126e 027c 047d 127c 0364 0175 0072  .}.n.|.}.|.d.u.r
+00000950: 437c 006a 057c 1264 078d 017d 1374 02a0  C|.j.|.d...}.t..
+00000960: 0364 087c 139b 0064 099d 03a1 0101 006e  .d.|...d.......n
+00000970: 027c 037d 1374 06a0 077c 01a1 017d 1474  .|.}.t...|...}.t
+00000980: 08a0 097c 14a1 017d 157c 15a0 0a64 0aa1  ...|...}.|...d..
+00000990: 017d 167c 167c 027c 137c 1264 0b9c 047d  .}.|.|.|.|.d...}
+000009a0: 177c 0564 0175 0072 6574 02a0 0364 0ca1  .|.d.u.ret...d..
+000009b0: 0101 006e 1774 0b7c 0583 0164 0d6b 0272  ...n.t.|...d.k.r
+000009c0: 7174 02a0 0364 0ea1 0101 006e 0b7c 006a  qt...d.....n.|.j
+000009d0: 0c7c 057c 067c 0d7c 0e64 0f8d 047c 1764  .|.|.|.|.d...|.d
+000009e0: 103c 007c 0b72 827c 0b7c 1764 113c 007c  .<.|.r.|.|.d.<.|
+000009f0: 0a72 887c 0a7c 1764 123c 007c 0672 8e7c  .r.|.|.d.<.|.r.|
+00000a00: 067c 1764 133c 007c 0772 947c 077c 1764  .|.d.<.|.r.|.|.d
+00000a10: 143c 007c 0872 9a7c 087c 1764 153c 007c  .<.|.r.|.|.d.<.|
+00000a20: 0972 a07c 097c 1764 163c 007c 0c72 a67c  .r.|.|.d.<.|.r.|
+00000a30: 0c7c 1764 173c 007c 1064 0175 0172 e47c  .|.d.<.|.d.u.r.|
+00000a40: 0564 0175 0072 b474 02a0 0364 18a1 0101  .d.u.r.t...d....
+00000a50: 006e 3074 0b7c 0583 0164 0d6b 0272 c074  .n0t.|...d.k.r.t
+00000a60: 02a0 0364 19a1 0101 006e 247c 0f64 0175  ...d.....n$|.d.u
+00000a70: 0072 ca74 02a0 0364 1aa1 0101 006e 1a7c  .r.t...d.....n.|
+00000a80: 0f7c 056a 0d76 0172 d974 02a0 0364 1b7c  .|.j.v.r.t...d.|
+00000a90: 0f9b 0064 1c9d 03a1 0101 006e 0b7c 006a  ...d.......n.|.j
+00000aa0: 0e7c 057c 0d7c 0f7c 1064 1d8d 047c 1764  .|.|.|.|.d...|.d
+00000ab0: 1e3c 007c 006a 0f7c 057c 027c 017c 127c  .<.|.j.|.|.|.|.|
+00000ac0: 077c 1164 1f8d 065c 027d 187d 197c 197c  .|.d...\.}.}.|.|
+00000ad0: 1764 203c 007c 177c 1866 0253 0029 2161  .d <.|.|.f.S.)!a
+00000ae0: 0a12 0000 4675 6e63 7469 6f6e 2070 7265  ....Function pre
+00000af0: 7061 7265 7320 696e 7075 7420 6461 7461  pares input data
+00000b00: 2066 6f72 2062 7569 6c64 206d 6f64 656c   for build model
+00000b10: 207a 6970 2066 696c 652c 2074 6861 7420   zip file, that 
+00000b20: 6973 2072 6561 6479 2074 6f20 6265 2069  is ready to be i
+00000b30: 6d70 6c65 6d65 6e74 6564 2069 6e20 5461  mplemented in Ta
+00000b40: 7261 6e44 4d20 736f 6674 7761 7265 2e0a  ranDM software..
+00000b50: 2020 2020 2020 2020 4372 6561 7465 6420          Created 
+00000b60: 696e 7075 7420 6461 7461 2077 696c 6c20  input data will 
+00000b70: 6265 2073 656e 7420 746f 2074 6865 2054  be sent to the T
+00000b80: 6172 616e 444d 2065 6e64 706f 696e 742c  aranDM endpoint,
+00000b90: 2074 6872 6f75 6768 2077 6869 6368 2066   through which f
+00000ba0: 696e 616c 206d 6f64 656c 207a 6970 2066  inal model zip f
+00000bb0: 696c 6520 6973 2072 6574 7572 6e65 642e  ile is returned.
+00000bc0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00000bd0: 206d 6f64 656c 3a20 5472 6169 6e65 6420   model: Trained 
+00000be0: 7072 6564 6963 7469 7665 206d 6f64 656c  predictive model
+00000bf0: 2e20 4f6e 6520 6f66 2066 726f 6d20 2273  . One of from "s
+00000c00: 6b6c 6561 726e 2e65 6e73 656d 626c 652e  klearn.ensemble.
+00000c10: 5261 6e64 6f6d 466f 7265 7374 436c 6173  RandomForestClas
+00000c20: 7369 6669 6572 222c 0a20 2020 2020 2020  sifier",.       
+00000c30: 2022 736b 6c65 6172 6e2e 6c69 6e65 6172   "sklearn.linear
+00000c40: 5f6d 6f64 656c 2e4c 6f67 6973 7469 6352  _model.LogisticR
+00000c50: 6567 7265 7373 696f 6e22 2c20 2278 6762  egression", "xgb
+00000c60: 6f6f 7374 2e42 6f6f 7374 6572 222c 2022  oost.Booster", "
+00000c70: 7064 2e44 6174 6146 7261 6d65 222e 2022  pd.DataFrame". "
+00000c80: 7064 2e44 6174 6146 7261 6d65 2220 7265  pd.DataFrame" re
+00000c90: 7072 6573 656e 7473 2065 7870 6572 740a  presents expert.
+00000ca0: 2020 2020 2020 2020 7363 6f72 6563 6172          scorecar
+00000cb0: 6420 6d6f 6465 6c2c 2077 6865 7265 2075  d model, where u
+00000cc0: 7365 7220 6d61 6e75 616c 6c79 2064 6566  ser manually def
+00000cd0: 696e 6573 2076 616c 7565 7320 666f 7220  ines values for 
+00000ce0: 7072 6564 6963 746f 7220 6269 6e73 2e0a  predictor bins..
+00000cf0: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
+00000d00: 7474 7269 6275 7465 733a 204c 6973 7420  ttributes: List 
+00000d10: 6f66 206d 6f64 656c 2070 7265 6469 6374  of model predict
+00000d20: 6f72 732e 0a20 2020 2020 2020 203a 7061  ors..        :pa
+00000d30: 7261 6d20 6d6f 6465 6c5f 6e61 6d65 3a20  ram model_name: 
+00000d40: 4e61 6d65 206f 6620 7468 6520 6d6f 6465  Name of the mode
+00000d50: 6c20 2877 696c 6c20 6265 2076 6973 6962  l (will be visib
+00000d60: 6c65 2069 6e20 5461 7261 6e44 4d20 4755  le in TaranDM GU
+00000d70: 4929 2e0a 2020 2020 2020 2020 3a70 6172  I)..        :par
+00000d80: 616d 206d 6f64 656c 5f74 7970 653a 2054  am model_type: T
+00000d90: 7970 6520 6f66 2074 6865 206d 6f64 656c  ype of the model
+00000da0: 2e20 4f6e 6520 6f66 2022 5847 4222 2c20  . One of "XGB", 
+00000db0: 224c 4f47 4953 5449 435f 5245 4752 4553  "LOGISTIC_REGRES
+00000dc0: 5349 4f4e 222c 2022 5241 4e44 4f4d 5f46  SION", "RANDOM_F
+00000dd0: 4f52 4553 5422 2c20 2245 5850 4552 545f  OREST", "EXPERT_
+00000de0: 5343 4f52 4522 2e0a 2020 2020 2020 2020  SCORE"..        
+00000df0: 3a70 6172 616d 2064 6174 613a 2044 6174  :param data: Dat
+00000e00: 6173 6574 2075 7365 6420 666f 7220 6d6f  aset used for mo
+00000e10: 6465 6c20 7472 6169 6e69 6e67 2e20 5265  del training. Re
+00000e20: 7175 6972 6564 2074 6f20 6361 6c63 756c  quired to calcul
+00000e30: 6174 6520 6d6f 6465 6c20 7065 7266 6f72  ate model perfor
+00000e40: 6d61 6e63 652c 2061 6e64 2064 6573 6372  mance, and descr
+00000e50: 6970 7469 7665 2073 7461 7469 7374 6963  iptive statistic
+00000e60: 730a 2020 2020 2020 2020 6162 6f75 7420  s.        about 
+00000e70: 6465 7665 6c6f 706d 656e 7420 7361 6d70  development samp
+00000e80: 6c65 2e0a 2020 2020 2020 2020 3a70 6172  le..        :par
+00000e90: 616d 206c 6162 656c 5f6e 616d 653a 204e  am label_name: N
+00000ea0: 616d 6520 6f66 2074 6865 2074 6172 6765  ame of the targe
+00000eb0: 7420 7661 7269 6162 6c65 2e20 5368 6f75  t variable. Shou
+00000ec0: 6c64 2062 6520 696e 636c 7564 6564 2069  ld be included i
+00000ed0: 6e20 6461 7461 2074 6f20 7072 6f70 6572  n data to proper
+00000ee0: 6c79 2065 7661 6c75 6174 6520 6d6f 6465  ly evaluate mode
+00000ef0: 6c20 7065 7266 6f72 6d61 6e63 652e 0a20  l performance.. 
+00000f00: 2020 2020 2020 203a 7061 7261 6d20 7461         :param ta
+00000f10: 7267 6574 5f63 6c61 7373 3a20 5461 7267  rget_class: Targ
+00000f20: 6574 2063 6c61 7373 2070 7265 6469 6374  et class predict
+00000f30: 6564 2062 7920 7468 6520 6d6f 6465 6c2e  ed by the model.
+00000f40: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000f50: 6174 7472 6962 7574 655f 6269 6e6e 696e  attribute_binnin
+00000f60: 673a 2041 7474 7269 6275 7465 2062 696e  g: Attribute bin
+00000f70: 6e69 6e67 2028 6966 2061 7070 6c69 6564  ning (if applied
+00000f80: 292e 2049 6e20 696e 6665 7265 6e63 6520  ). In inference 
+00000f90: 7068 6173 652c 2077 6520 6669 7273 7420  phase, we first 
+00000fa0: 6170 706c 7920 7072 6564 6963 746f 720a  apply predictor.
+00000fb0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+00000fc0: 6d61 7469 6f6e 2028 6966 2064 6566 696e  mation (if defin
+00000fd0: 6564 2920 616e 6420 7468 656e 2062 696e  ed) and then bin
+00000fe0: 6e69 6e67 2e20 5265 7375 6c74 696e 6720  ning. Resulting 
+00000ff0: 7661 6c75 6520 6973 2070 6173 7365 6420  value is passed 
+00001000: 746f 206d 6f64 656c 2070 7265 6469 6374  to model predict
+00001010: 206d 6574 686f 642e 0a0a 2020 2020 2020   method...      
+00001020: 2020 4269 6e6e 696e 6720 7368 6f75 6c64    Binning should
+00001030: 2062 6520 7072 6f76 6964 6564 2061 7320   be provided as 
+00001040: 6120 6469 6374 696f 6e61 7279 2077 6974  a dictionary wit
+00001050: 6820 666f 6c6c 6f77 696e 6720 7374 7275  h following stru
+00001060: 6374 7572 653a 0a20 2020 2020 2020 2062  cture:.        b
+00001070: 696e 6e69 6e67 203d 207b 0a20 2020 2020  inning = {.     
+00001080: 2020 2020 2020 2027 6e75 6d65 7269 6361         'numerica
+00001090: 6c5f 7072 6564 6963 746f 7231 273a 207b  l_predictor1': {
+000010a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010b0: 2027 6474 7970 6527 3a20 274e 554d 4552   'dtype': 'NUMER
+000010c0: 4943 414c 272c 0a20 2020 2020 2020 2020  ICAL',.         
+000010d0: 2020 2020 2020 2027 6269 6e73 273a 205b         'bins': [
+000010e0: 2d6e 702e 696e 662c 2032 302c 2033 352c  -np.inf, 20, 35,
+000010f0: 2035 302c 206e 702e 696e 665d 2c0a 2020   50, np.inf],.  
+00001100: 2020 2020 2020 2020 2020 2020 2020 2762                'b
+00001110: 696e 5f76 616c 7327 3a20 5b31 2c20 322c  in_vals': [1, 2,
+00001120: 2033 2c20 342c 2031 3030 305d 2c0a 2020   3, 4, 1000],.  
+00001130: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+00001140: 756c 6c5f 7661 6c27 3a20 300a 2020 2020  ull_val': 0.    
+00001150: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001160: 2020 2020 2020 2027 6361 7465 676f 7269         'categori
+00001170: 6361 6c5f 7072 6564 6963 746f 7231 273a  cal_predictor1':
+00001180: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001190: 2020 2027 6474 7970 6527 3a20 2743 4154     'dtype': 'CAT
+000011a0: 4547 4f52 4943 414c 272c 0a20 2020 2020  EGORICAL',.     
+000011b0: 2020 2020 2020 2020 2020 2027 6269 6e73             'bins
+000011c0: 273a 205b 5b27 4d27 5d2c 205b 2746 275d  ': [['M'], ['F']
+000011d0: 5d27 2c0a 2020 2020 2020 2020 2020 2020  ]',.            
+000011e0: 2020 2020 2762 696e 5f76 616c 7327 3a20      'bin_vals': 
+000011f0: 5b31 2c20 322c 2033 2c20 342c 2031 3030  [1, 2, 3, 4, 100
+00001200: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+00001210: 2020 2020 276e 756c 6c5f 7661 6c27 3a20      'null_val': 
+00001220: 300a 2020 2020 2020 2020 2020 2020 7d2c  0.            },
+00001230: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00001240: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00001250: 2020 204b 6579 7320 6f66 2070 726f 7669     Keys of provi
+00001260: 6465 6420 6469 6374 696f 6e61 7279 2061  ded dictionary a
+00001270: 7265 206e 616d 6573 206f 6620 7468 6520  re names of the 
+00001280: 7072 6564 6963 746f 7273 2e20 5461 7261  predictors. Tara
+00001290: 6e44 4d20 7375 7070 6f72 7473 2027 4e55  nDM supports 'NU
+000012a0: 4d45 5249 4341 4c27 2061 6e64 2027 4341  MERICAL' and 'CA
+000012b0: 5445 474f 5249 4341 4c27 2064 6174 610a  TEGORICAL' data.
+000012c0: 2020 2020 2020 2020 7479 7065 7320 6f66          types of
+000012d0: 2070 7265 6469 6374 6f72 732e 2046 6f72   predictors. For
+000012e0: 206e 756d 6572 6963 616c 2070 7265 6469   numerical predi
+000012f0: 6374 6f72 732c 2062 696e 6e69 6e67 2069  ctors, binning i
+00001300: 7320 6465 6669 6e65 6420 6279 2070 726f  s defined by pro
+00001310: 7669 6469 6e67 206c 6973 7420 6f66 2062  viding list of b
+00001320: 696e 2062 6f72 6465 7273 2e20 466f 720a  in borders. For.
+00001330: 2020 2020 2020 2020 6361 7465 676f 7269          categori
+00001340: 6361 6c20 7072 6564 6963 746f 7273 2c20  cal predictors, 
+00001350: 6269 6e6e 696e 6720 6973 2064 6566 696e  binning is defin
+00001360: 6564 2062 7920 7072 6f76 6964 696e 6720  ed by providing 
+00001370: 6c69 7374 206f 6620 6c69 7374 732e 2049  list of lists. I
+00001380: 6e6e 6572 206c 6973 7473 2064 6566 696e  nner lists defin
+00001390: 6520 7661 6c75 6573 2074 6861 7420 6265  e values that be
+000013a0: 6c6f 6e67 0a20 2020 2020 2020 2074 6f20  long.        to 
+000013b0: 6561 6368 2067 726f 7570 2e20 426f 7468  each group. Both
+000013c0: 2027 4e55 4d45 5249 4341 4c27 2061 6e64   'NUMERICAL' and
+000013d0: 2027 4341 5445 474f 5249 4341 4c27 2064   'CATEGORICAL' d
+000013e0: 6174 6120 7479 7065 7320 636f 6e74 6169  ata types contai
+000013f0: 6e20 6174 7472 6962 7574 6573 2027 6269  n attributes 'bi
+00001400: 6e5f 7661 6c73 2720 616e 640a 2020 2020  n_vals' and.    
+00001410: 2020 2020 276e 756c 6c5f 7661 6c27 2e20      'null_val'. 
+00001420: 5468 6f73 6520 6172 6520 7661 6c75 6573  Those are values
+00001430: 2075 7365 6420 666f 7220 656e 636f 6469   used for encodi
+00001440: 6e67 2074 6865 2062 696e 732e 2027 6e75  ng the bins. 'nu
+00001450: 6c6c 5f76 616c 2720 6973 2061 6e20 656e  ll_val' is an en
+00001460: 636f 6469 6e67 2076 616c 7565 2066 6f72  coding value for
+00001470: 206e 756c 6c20 7661 6c75 6573 0a20 2020   null values.   
+00001480: 2020 2020 2028 6d69 7373 696e 6773 292e       (missings).
+00001490: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000014a0: 2061 7474 7269 6275 7465 5f74 7261 6e73   attribute_trans
+000014b0: 666f 726d 6174 696f 6e3a 2054 7261 6e73  formation: Trans
+000014c0: 666f 726d 6174 696f 6e20 6f66 2074 6865  formation of the
+000014d0: 2070 7265 6469 6374 6f72 732e 2054 7261   predictors. Tra
+000014e0: 6e73 666f 726d 6174 696f 6e20 6973 2061  nsformation is a
+000014f0: 7070 6c69 6564 2062 6566 6f72 6520 6269  pplied before bi
+00001500: 6e6e 696e 672e 2049 6620 626f 7468 0a20  nning. If both. 
+00001510: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00001520: 6174 696f 6e20 616e 6420 6269 6e6e 696e  ation and binnin
+00001530: 6720 6172 6520 6465 6669 6e65 642c 2070  g are defined, p
+00001540: 7265 6469 6374 6f72 2069 7320 6669 7273  redictor is firs
+00001550: 7420 7472 616e 7366 6f72 6d65 6420 616e  t transformed an
+00001560: 6420 6269 6e6e 696e 6720 6973 2061 7070  d binning is app
+00001570: 6c69 6564 206f 7665 7220 7661 6c75 6573  lied over values
+00001580: 0a20 2020 2020 2020 206f 6274 6169 6e65  .        obtaine
+00001590: 6420 6166 7465 7220 7472 616e 7366 6f72  d after transfor
+000015a0: 6d61 7469 6f6e 2e0a 0a20 2020 2020 2020  mation...       
+000015b0: 2054 7261 6e73 666f 726d 6174 696f 6e20   Transformation 
+000015c0: 7368 6f75 6c64 2062 6520 7072 6f76 6964  should be provid
+000015d0: 6564 2061 7320 6120 6469 6374 696f 6e61  ed as a dictiona
+000015e0: 7279 2077 6974 6820 666f 6c6c 6f77 696e  ry with followin
+000015f0: 6720 7374 7275 6374 7572 653a 0a20 2020  g structure:.   
+00001600: 2020 2020 2074 7261 6e73 666f 726d 6174       transformat
+00001610: 696f 6e20 3d20 7b0a 2020 2020 2020 2020  ion = {.        
+00001620: 2020 2020 276e 756d 6572 6963 616c 5f70      'numerical_p
+00001630: 7265 6469 6374 6f72 3127 3a20 277b 6e75  redictor1': '{nu
+00001640: 6d65 7269 6361 6c5f 7072 6564 6963 746f  merical_predicto
+00001650: 7231 7d20 2b20 3127 0a20 2020 2020 2020  r1} + 1'.       
+00001660: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+00001670: 207d 0a20 2020 2020 2020 2049 6e20 7472   }.        In tr
+00001680: 616e 7366 6f72 6d61 7469 6f6e 2066 6f72  ansformation for
+00001690: 6d75 6c61 2c20 616e 7974 6869 6e67 2069  mula, anything i
+000016a0: 6e20 227b 7d22 2069 7320 636f 6e73 6964  n "{}" is consid
+000016b0: 6572 6564 2061 7320 7072 6564 6963 746f  ered as predicto
+000016c0: 7220 616e 6420 7769 6c6c 2062 6520 7265  r and will be re
+000016d0: 706c 6163 6564 2077 6974 6820 7072 6564  placed with pred
+000016e0: 6963 746f 7220 7661 6c75 650a 2020 2020  ictor value.    
+000016f0: 2020 2020 6475 7269 6e67 2066 6f72 6d75      during formu
+00001700: 6c61 2065 7661 6c75 6174 696f 6e2e 0a0a  la evaluation...
+00001710: 2020 2020 2020 2020 3a70 6172 616d 2068          :param h
+00001720: 7970 6572 7061 7261 6d65 7465 7273 3a20  yperparameters: 
+00001730: 4d6f 6465 6c20 6879 7065 7270 6172 616d  Model hyperparam
+00001740: 6574 6572 732e 0a20 2020 2020 2020 203a  eters..        :
+00001750: 7061 7261 6d20 6765 6e65 7261 6c5f 6e6f  param general_no
+00001760: 7465 733a 2044 6963 7469 6f6e 6172 7920  tes: Dictionary 
+00001770: 6f66 2067 656e 6572 616c 206e 6f74 6573  of general notes
+00001780: 2061 626f 7574 2074 6865 206d 6f64 656c   about the model
+00001790: 2e20 4e6f 7465 7320 7769 6c6c 2062 6520  . Notes will be 
+000017a0: 6469 7370 6c61 7965 6420 696e 2047 5549  displayed in GUI
+000017b0: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000017c0: 2061 7474 7269 6275 7465 5f64 6573 6372   attribute_descr
+000017d0: 6970 7469 6f6e 3a20 4469 6374 696f 6e61  iption: Dictiona
+000017e0: 7279 2077 6974 6820 6465 7363 7269 7074  ry with descript
+000017f0: 696f 6e20 6f66 2070 7265 6469 6374 6f72  ion of predictor
+00001800: 732e 0a20 2020 2020 2020 203a 7061 7261  s..        :para
+00001810: 6d20 636f 6c75 6d6e 5f6e 616d 655f 7361  m column_name_sa
+00001820: 6d70 6c65 3a20 4e61 6d65 206f 6620 7468  mple: Name of th
+00001830: 6520 636f 6c75 6d6e 2069 6e20 6461 7461  e column in data
+00001840: 2c20 7468 6174 2064 6566 696e 6573 2064  , that defines d
+00001850: 6966 6665 7265 6e74 2064 6174 6120 7361  ifferent data sa
+00001860: 6d70 6c65 2074 7970 6573 2028 7472 6169  mple types (trai
+00001870: 6e2c 2074 6573 742c 2065 7463 2e29 2e0a  n, test, etc.)..
+00001880: 2020 2020 2020 2020 4966 2070 726f 7669          If provi
+00001890: 6465 642c 2073 616d 706c 6520 7374 6174  ded, sample stat
+000018a0: 6973 7469 6373 2077 696c 6c20 6265 2073  istics will be s
+000018b0: 746f 7265 6420 696e 206d 6f64 656c 206d  tored in model m
+000018c0: 6574 6164 6174 612e 0a20 2020 2020 2020  etadata..       
+000018d0: 203a 7061 7261 6d20 636f 6c75 6d6e 5f6e   :param column_n
+000018e0: 616d 655f 6461 7465 3a20 4e61 6d65 206f  ame_date: Name o
+000018f0: 6620 7468 6520 636f 6c75 6d6e 2069 6e20  f the column in 
+00001900: 6461 7461 2c20 7468 6174 2064 6566 696e  data, that defin
+00001910: 6573 2074 696d 6520 6469 6d65 6e73 696f  es time dimensio
+00001920: 6e2e 2049 6620 7072 6f76 6964 6564 2c20  n. If provided, 
+00001930: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00001940: 740a 2020 2020 2020 2020 7469 6d65 2072  t.        time r
+00001950: 616e 6765 2075 7365 6420 696e 2064 6576  ange used in dev
+00001960: 656c 6f70 6d65 6e74 2073 616d 706c 6520  elopment sample 
+00001970: 6461 7461 2077 696c 6c20 6265 2073 746f  data will be sto
+00001980: 7265 6420 696e 206d 6f64 656c 206d 6574  red in model met
+00001990: 6164 6174 612e 0a20 2020 2020 2020 203a  adata..        :
+000019a0: 7061 7261 6d20 636f 6c75 6d6e 5f6e 616d  param column_nam
+000019b0: 655f 7072 6564 6963 7469 6f6e 3a20 4e61  e_prediction: Na
+000019c0: 6d65 206f 6620 7468 6520 636f 6c75 6d6e  me of the column
+000019d0: 2069 6e20 6461 7461 2c20 7468 6174 2068   in data, that h
+000019e0: 6f6c 6473 206d 6f64 656c 2070 7265 6469  olds model predi
+000019f0: 6374 696f 6e2e 2054 6869 7320 636f 6c75  ction. This colu
+00001a00: 6d6e 2069 7320 7573 6564 2074 6f0a 2020  mn is used to.  
+00001a10: 2020 2020 2020 6576 616c 7561 7465 206d        evaluate m
+00001a20: 6f64 656c 2070 6572 666f 726d 616e 6365  odel performance
+00001a30: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00001a40: 2065 7661 6c75 6174 655f 7065 7266 6f72   evaluate_perfor
+00001a50: 6d61 6e63 653a 2044 6963 7469 6f6e 6172  mance: Dictionar
+00001a60: 7920 7468 6174 2064 6566 696e 6573 2070  y that defines p
+00001a70: 6572 666f 726d 616e 6365 2074 6f20 6265  erformance to be
+00001a80: 2065 7661 6c75 6174 6564 202d 2077 6869   evaluated - whi
+00001a90: 6368 2074 6172 6765 7420 616e 6420 6f76  ch target and ov
+00001aa0: 6572 2077 6869 6368 0a20 2020 2020 2020  er which.       
+00001ab0: 2073 616d 706c 6520 7479 7065 732e 2055   sample types. U
+00001ac0: 7365 2066 6f6c 6c6f 7769 6e67 2073 7472  se following str
+00001ad0: 7563 7475 7265 3a0a 0a20 2020 2020 2020  ucture:..       
+00001ae0: 2065 7661 6c75 6174 655f 7065 7266 6f72   evaluate_perfor
+00001af0: 6d61 6e63 6520 3d20 7b0a 2020 2020 2020  mance = {.      
+00001b00: 2020 7d0a 2020 2020 2020 2020 3a70 6172    }.        :par
+00001b10: 616d 206c 6561 726e 696e 675f 6375 7276  am learning_curv
+00001b20: 6573 5f64 6174 613a 2044 6174 6120 666f  es_data: Data fo
+00001b30: 7220 706c 6f74 7469 6e67 206c 6561 726e  r plotting learn
+00001b40: 696e 6720 6375 7276 6573 2070 6c6f 7420  ing curves plot 
+00001b50: 696e 2066 6f6c 6c6f 7769 6e67 2073 7472  in following str
+00001b60: 7563 7475 7265 3a0a 0a20 2020 2020 2020  ucture:..       
+00001b70: 206c 6561 726e 696e 675f 6375 7276 6573   learning_curves
+00001b80: 5f64 6174 6120 3d20 7b0a 2020 2020 2020  _data = {.      
+00001b90: 2020 2020 2020 2773 616d 706c 6531 273a        'sample1':
+00001ba0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001bb0: 2020 2027 6d65 7472 6963 3127 3a20 5b0a     'metric1': [.
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bd0: 2020 2020 302e 352c 0a20 2020 2020 2020      0.5,.       
+00001be0: 2020 2020 2020 2020 2020 2020 2030 2e34               0.4
+00001bf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001c00: 2020 2020 2020 302e 330a 2020 2020 2020        0.3.      
+00001c10: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00001c20: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001c30: 2020 2020 2020 2027 7361 6d70 6c65 3227         'sample2'
+00001c40: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001c50: 2020 2020 276d 6574 7269 6331 273a 205b      'metric1': [
+00001c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c70: 2020 2020 2030 2e36 2c0a 2020 2020 2020       0.6,.      
+00001c80: 2020 2020 2020 2020 2020 2020 2020 302e                0.
+00001c90: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
+00001ca0: 2020 2020 2020 2030 2e34 0a20 2020 2020         0.4.     
+00001cb0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00001cc0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001cd0: 2020 207d 0a20 2020 2020 2020 203a 7265     }.        :re
+00001ce0: 7475 726e 3a0a 2020 2020 2020 2020 4e29  turn:.        N)
+00001cf0: 0172 2700 0000 7a0c 4d6f 6465 6c20 7479  .r'...z.Model ty
+00001d00: 7065 2027 7a29 2720 6973 2069 6e76 616c  pe 'z)' is inval
+00001d10: 6964 2e20 5375 7070 6f72 7465 6420 6d6f  id. Supported mo
+00001d20: 6465 6c20 7479 7065 7320 6172 653a 20fa  del types are: .
+00001d30: 022c 207a 2e2e 2057 696c 6c20 7472 7920  ., z.. Will try 
+00001d40: 746f 2064 6574 6563 7420 6d6f 6465 6c20  to detect model 
+00001d50: 7479 7065 2061 7574 6f6d 6174 6963 616c  type automatical
+00001d60: 6c79 2ea9 0172 2a00 0000 7a34 4d6f 6465  ly...r*...z4Mode
+00001d70: 6c20 6e61 6d65 2077 6173 206e 6f74 2070  l name was not p
+00001d80: 726f 7669 6465 642e 2047 656e 6572 6174  rovided. Generat
+00001d90: 6564 206d 6f64 656c 206e 616d 653a 2027  ed model name: '
+00001da0: 7a02 272e da05 6173 6369 6929 0472 2700  z.'...ascii).r'.
+00001db0: 0000 5a0a 7072 6564 6963 746f 7273 7229  ..Z.predictorsr)
+00001dc0: 0000 0072 2a00 0000 7a41 4e6f 2064 6174  ...r*...zANo dat
+00001dd0: 6173 6574 2077 6173 2070 726f 7669 6465  aset was provide
+00001de0: 642e 2043 616e 6e6f 7420 6576 616c 7561  d. Cannot evalua
+00001df0: 7465 2073 616d 706c 6520 6465 7363 7269  te sample descri
+00001e00: 7074 696f 6e20 6461 7461 2e72 0100 0000  ption data.r....
+00001e10: 7a4d 5072 6f76 6964 6564 2064 6174 6173  zMProvided datas
+00001e20: 6574 2068 6173 2030 206f 6273 6572 7661  et has 0 observa
+00001e30: 7469 6f6e 732e 2043 616e 6e6f 7420 6576  tions. Cannot ev
+00001e40: 616c 7561 7465 2073 616d 706c 6520 6465  aluate sample de
+00001e50: 7363 7269 7074 696f 6e20 6461 7461 2e29  scription data.)
+00001e60: 0472 2b00 0000 da11 636f 6c75 6d6e 5f6e  .r+.....column_n
+00001e70: 616d 655f 6c61 6265 6c72 3200 0000 7233  ame_labelr2...r3
+00001e80: 0000 005a 1773 616d 706c 655f 6465 7363  ...Z.sample_desc
+00001e90: 7269 7074 696f 6e5f 6461 7461 da0d 6765  ription_data..ge
+00001ea0: 6e65 7261 6c5f 6e6f 7465 7372 3000 0000  neral_notesr0...
+00001eb0: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
+00001ec0: 2f00 0000 7231 0000 007a 3b4e 6f20 6461  /...r1...z;No da
+00001ed0: 7461 7365 7420 7761 7320 7072 6f76 6964  taset was provid
+00001ee0: 6564 2e20 4361 6e6e 6f74 2065 7661 6c75  ed. Cannot evalu
+00001ef0: 6174 6520 6d6f 6465 6c20 7065 7266 6f72  ate model perfor
+00001f00: 6d61 6e63 652e 7a47 5072 6f76 6964 6564  mance.zGProvided
+00001f10: 2064 6174 6173 6574 2068 6173 2030 206f   dataset has 0 o
+00001f20: 6273 6572 7661 7469 6f6e 732e 2043 616e  bservations. Can
+00001f30: 6e6f 7420 6576 616c 7561 7465 206d 6f64  not evaluate mod
+00001f40: 656c 2070 6572 666f 726d 616e 6365 2e7a  el performance.z
+00001f50: 784e 616d 6520 6f66 2074 6865 2063 6f6c  xName of the col
+00001f60: 756d 6e73 2074 6861 7420 686f 6c64 7320  umns that holds 
+00001f70: 7072 6564 6963 7469 6f6e 7320 2863 6f6c  predictions (col
+00001f80: 756d 6e5f 6e61 6d65 5f70 7265 6469 6374  umn_name_predict
+00001f90: 696f 6e29 2077 6173 206e 6f74 2070 726f  ion) was not pro
+00001fa0: 7669 6465 642e 2043 616e 6e6f 7420 6576  vided. Cannot ev
+00001fb0: 616c 7561 7465 206d 6f64 656c 2070 6572  aluate model per
+00001fc0: 666f 726d 616e 6365 2e7a 3550 726f 7669  formance.z5Provi
+00001fd0: 6465 6420 6e61 6d65 206f 6620 7468 6520  ded name of the 
+00001fe0: 636f 6c75 6d6e 7320 7468 6174 2068 6f6c  columns that hol
+00001ff0: 6473 2070 7265 6469 6374 696f 6e73 2027  ds predictions '
+00002000: 7a34 2720 6973 206e 6f74 2069 6e20 6461  z4' is not in da
+00002010: 7461 2e20 4361 6e6e 6f74 2065 7661 6c75  ta. Cannot evalu
+00002020: 6174 6520 6d6f 6465 6c20 7065 7266 6f72  ate model perfor
+00002030: 6d61 6e63 652e 2904 722b 0000 0072 3200  mance.).r+...r2.
+00002040: 0000 7234 0000 0072 3500 0000 5a11 6d6f  ..r4...r5...Z.mo
+00002050: 6465 6c5f 7065 7266 6f72 6d61 6e63 6529  del_performance)
+00002060: 0672 2b00 0000 7228 0000 0072 2700 0000  .r+...r(...r'...
+00002070: 722a 0000 0072 2d00 0000 7236 0000 005a  r*...r-...r6...Z
+00002080: 0f61 7474 6163 6865 645f 696d 6167 6573  .attached_images
+00002090: 2910 da0f 5f67 6574 5f6d 6f64 656c 5f74  )..._get_model_t
+000020a0: 7970 65da 1573 7570 706f 7274 6564 5f6d  ype..supported_m
+000020b0: 6f64 656c 5f74 7970 6573 da06 6c6f 6767  odel_types..logg
+000020c0: 6572 da07 7761 726e 696e 67da 046a 6f69  er..warning..joi
+000020d0: 6eda 145f 6765 6e65 7261 7465 5f6d 6f64  n.._generate_mod
+000020e0: 656c 5f6e 616d 65da 0670 6963 6b6c 65da  el_name..pickle.
+000020f0: 0564 756d 7073 da06 6261 7365 3634 da09  .dumps..base64..
+00002100: 6236 3465 6e63 6f64 65da 0664 6563 6f64  b64encode..decod
+00002110: 65da 036c 656e da1c 5f67 6574 5f64 6174  e..len.._get_dat
+00002120: 615f 7361 6d70 6c65 5f64 6573 6372 6970  a_sample_descrip
+00002130: 7469 6f6e da07 636f 6c75 6d6e 73da 215f  tion..columns.!_
+00002140: 6765 745f 7072 6564 6963 7469 7665 5f6d  get_predictive_m
+00002150: 6f64 656c 5f70 6572 666f 726d 616e 6365  odel_performance
+00002160: da10 5f67 656e 6572 6174 655f 696d 6167  .._generate_imag
+00002170: 6573 291a 721f 0000 0072 2700 0000 7228  es).r....r'...r(
+00002180: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+00002190: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
+000021a0: 0072 2f00 0000 7230 0000 0072 3b00 0000  .r/...r0...r;...
+000021b0: 7231 0000 0072 3200 0000 7233 0000 0072  r1...r2...r3...r
+000021c0: 3400 0000 7235 0000 0072 3600 0000 5a10  4...r5...r6...Z.
+000021d0: 6d6f 6465 6c5f 7479 7065 5f66 696e 616c  model_type_final
+000021e0: 5a10 6d6f 6465 6c5f 6e61 6d65 5f66 696e  Z.model_name_fin
+000021f0: 616c 5a0c 6d6f 6465 6c5f 6269 6e61 7279  alZ.model_binary
+00002200: 5a14 6d6f 6465 6c5f 6269 6e61 7279 5f65  Z.model_binary_e
+00002210: 6e63 6f64 6564 5a1b 6d6f 6465 6c5f 6269  ncodedZ.model_bi
+00002220: 6e61 7279 5f65 6e63 6f64 6564 5f73 7472  nary_encoded_str
+00002230: 696e 67da 0c72 6571 7565 7374 5f64 6174  ing..request_dat
+00002240: 61da 0669 6d61 6765 73da 0b69 6d61 6765  a..images..image
+00002250: 735f 6d65 7461 7222 0000 0072 2200 0000  s_metar"...r"...
+00002260: 7223 0000 00da 1d70 7265 7061 7265 5f70  r#.....prepare_p
+00002270: 7265 6469 6374 6976 655f 6d6f 6465 6c5f  redictive_model_
+00002280: 6461 7461 2e00 0000 739a 0000 0008 6904  data....s.....i.
+00002290: 0108 010e 010a 0104 0108 010a 0106 ff04  ................
+000022a0: ff0e 0404 0208 020c 0114 0104 020a 020a  ................
+000022b0: 010a 0102 0202 0102 0102 0106 fc08 070c  ................
+000022c0: 010c 010c 0104 0202 0102 0102 0102 010a  ................
+000022d0: fc04 0708 0104 0108 0104 0108 0104 0108  ................
+000022e0: 0104 0108 0104 0108 0104 0108 0108 0208  ................
+000022f0: 010c 010c 010c 0108 0104 0102 0106 ff0a  ................
+00002300: 0404 010a 0106 ff04 0502 0102 0102 0102  ................
+00002310: 010a fc04 0702 0102 0102 0102 0102 0102  ................
+00002320: 010a fa08 0808 027a 3345 7870 6f72 7450  .......z3ExportP
+00002330: 7265 6469 6374 6976 654d 6f64 656c 2e70  redictiveModel.p
+00002340: 7265 7061 7265 5f70 7265 6469 6374 6976  repare_predictiv
+00002350: 655f 6d6f 6465 6c5f 6461 7461 724c 0000  e_model_datarL..
+00002360: 00da 0866 696c 656e 616d 6572 4d00 0000  ...filenamerM...
+00002370: 6304 0000 0000 0000 0000 0000 0009 0000  c...............
+00002380: 0006 0000 0043 0000 0073 7000 0000 7c03  .....C...sp...|.
+00002390: 6400 7500 7206 6700 7d03 7c00 6a00 6401  d.u.r.g.}.|.j.d.
+000023a0: 1700 7d04 7401 6a02 7c04 7c01 7403 7c00  ..}.t.j.|.|.t.|.
+000023b0: 6a04 7c00 6a05 8302 6402 8d03 7d05 7c05  j.|.j...d...}.|.
+000023c0: 6a06 6403 6b02 7226 7407 a008 6404 a101  j.d.k.r&t...d...
+000023d0: 0100 7c05 a009 a100 7d06 7c06 6405 1900  ..|.....}.|.d...
+000023e0: 7d07 7c06 6406 1900 7d08 7c00 a00a 7c07  }.|.d...}.|...|.
+000023f0: 7c08 7c02 7c03 a104 0100 6400 5300 2907  |.|.|.....d.S.).
+00002400: 4e7a 2061 6e61 6c79 7469 6373 2f62 7569  Nz analytics/bui
+00002410: 6c64 5f70 7265 6469 6374 6976 655f 6d6f  ld_predictive_mo
+00002420: 6465 6c29 03da 0375 726c da04 6a73 6f6e  del)...url..json
+00002430: 5a04 6175 7468 e9c8 0000 007a 4053 7563  Z.auth.....z@Suc
+00002440: 6365 7373 6675 6c6c 7920 6361 6c6c 6564  cessfully called
+00002450: 2027 616e 616c 7974 6963 732f 6275 696c   'analytics/buil
+00002460: 645f 7072 6564 6963 7469 7665 5f6d 6f64  d_predictive_mod
+00002470: 656c 2720 656e 6470 6f69 6e74 2e5a 1e65  el' endpoint.Z.e
+00002480: 7874 656e 6465 645f 7072 6564 6963 7469  xtended_predicti
+00002490: 7665 5f6d 6f64 656c 5f79 616d 6cda 1365  ve_model_yaml..e
+000024a0: 7874 6572 6e61 6c5f 6d6f 6465 6c5f 6a73  xternal_model_js
+000024b0: 6f6e 290b 721a 0000 00da 0872 6571 7565  on).r......reque
+000024c0: 7374 73da 0470 6f73 7472 0b00 0000 721b  sts..postr....r.
+000024d0: 0000 0072 1c00 0000 5a0b 7374 6174 7573  ...r....Z.status
+000024e0: 5f63 6f64 6572 3e00 0000 da04 696e 666f  _coder>.....info
+000024f0: 7252 0000 00da 0b73 6176 655f 746f 5f7a  rR.....save_to_z
+00002500: 6970 2909 721f 0000 0072 4c00 0000 7250  ip).r....rL...rP
+00002510: 0000 0072 4d00 0000 7251 0000 00da 0872  ...rM...rQ.....r
+00002520: 6573 706f 6e73 655a 0d72 6573 706f 6e73  esponseZ.respons
+00002530: 655f 6461 7461 da13 6578 7465 6e64 6564  e_data..extended
+00002540: 5f6d 6f64 656c 5f79 616d 6c72 5400 0000  _model_yamlrT...
+00002550: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
+00002560: 1662 7569 6c64 5f70 7265 6469 6374 6976  .build_predictiv
+00002570: 655f 6d6f 6465 6cf2 0000 0073 1400 0000  e_model....s....
+00002580: 0803 0401 0a02 1a01 0a02 0a01 0801 0805  ................
+00002590: 0801 1402 7a2c 4578 706f 7274 5072 6564  ....z,ExportPred
+000025a0: 6963 7469 7665 4d6f 6465 6c2e 6275 696c  ictiveModel.buil
+000025b0: 645f 7072 6564 6963 7469 7665 5f6d 6f64  d_predictive_mod
+000025c0: 656c 725a 0000 0072 5400 0000 6304 0000  elrZ...rT...c...
+000025d0: 0000 0000 0000 0000 000a 0000 0008 0000  ................
+000025e0: 0043 0000 0073 e800 0000 7c03 6400 7500  .C...s....|.d.u.
+000025f0: 7206 6700 7d03 6401 6402 8400 7d04 7400  r.g.}.d.d...}.t.
+00002600: a001 a100 7d05 7402 6a03 7c05 6403 7402  ....}.t.j.|.d.t.
+00002610: 6a04 6404 8d03 8f29 7d06 7c04 7c06 7400  j.d....)}.|.|.t.
+00002620: a005 7c00 a101 6405 8303 0100 7c04 7c06  ..|...d.....|.|.
+00002630: 7400 a005 7c01 a101 6406 8303 0100 7c03  t...|...d.....|.
+00002640: 4400 5d0c 7d07 7c04 7c06 7c07 6407 1900  D.].}.|.|.|.d...
+00002650: 7c07 6408 1900 8303 0100 712c 5700 6400  |.d.......q,W.d.
+00002660: 0400 0400 8303 0100 6e08 3100 7343 7701  ........n.1.sCw.
+00002670: 0100 0100 0100 5900 0100 7406 7c02 8301  ......Y...t.|...
+00002680: 7d08 7c08 a007 6409 a101 7355 7c08 6409  }.|...d...sU|.d.
+00002690: 3700 7d08 7408 7c08 640a 8302 8f10 7d09  7.}.t.|.d.....}.
+000026a0: 7c09 a009 7c05 a00a a100 a101 0100 5700  |...|.........W.
+000026b0: 6400 0400 0400 8303 0100 6400 5300 3100  d.........d.S.1.
+000026c0: 736d 7701 0100 0100 0100 5900 0100 6400  smw.......Y...d.
+000026d0: 5300 290b 4e63 0300 0000 0000 0000 0000  S.).Nc..........
+000026e0: 0000 0300 0000 0500 0000 5300 0000 7354  ..........S...sT
+000026f0: 0000 0074 007c 0174 016a 0283 0272 147c  ...t.|.t.j...r.|
+00002700: 01a0 0364 01a1 0101 0074 01a0 047c 01a0  ...d.....t...|..
+00002710: 05a1 00a0 06a1 00a1 017d 017c 01a0 0364  .........}.|...d
+00002720: 0174 076a 08a1 0201 007c 01a0 0364 01a1  .t.j.....|...d..
+00002730: 0101 007c 00a0 097c 027c 01a0 0aa1 00a1  ...|...|.|......
+00002740: 0201 0064 0053 0029 024e 7201 0000 0029  ...d.S.).Nr....)
+00002750: 0bda 0a69 7369 6e73 7461 6e63 65da 0269  ...isinstance..i
+00002760: 6fda 0853 7472 696e 6749 4fda 0473 6565  o..StringIO..see
+00002770: 6bda 0742 7974 6573 494f da04 7265 6164  k..BytesIO..read
+00002780: da06 656e 636f 6465 da02 6f73 da08 5345  ..encode..os..SE
+00002790: 454b 5f45 4e44 da08 7772 6974 6573 7472  EK_END..writestr
+000027a0: da08 6765 7476 616c 7565 2903 da07 6172  ..getvalue)...ar
+000027b0: 6368 6976 65da 0662 7566 6665 72da 046e  chive..buffer..n
+000027c0: 616d 6572 2200 0000 7222 0000 0072 2300  amer"...r"...r#.
+000027d0: 0000 da08 6164 645f 6669 6c65 0e01 0000  ....add_file....
+000027e0: 730c 0000 000c 010a 0112 010e 010a 0114  s...............
+000027f0: 017a 3345 7870 6f72 7450 7265 6469 6374  .z3ExportPredict
+00002800: 6976 654d 6f64 656c 2e73 6176 655f 746f  iveModel.save_to
+00002810: 5f7a 6970 2e3c 6c6f 6361 6c73 3e2e 6164  _zip.<locals>.ad
+00002820: 645f 6669 6c65 da01 7729 03da 0466 696c  d_file..w)...fil
+00002830: 65da 046d 6f64 65da 0b63 6f6d 7072 6573  e..mode..compres
+00002840: 7369 6f6e 7a13 6578 7465 6e64 6564 5f6d  sionz.extended_m
+00002850: 6f64 656c 2e79 616d 6c7a 1365 7874 6572  odel.yamlz.exter
+00002860: 6e61 6c5f 6d6f 6465 6c2e 6a73 6f6e da05  nal_model.json..
+00002870: 696d 6167 6572 5000 0000 7a04 2e7a 6970  imagerP...z..zip
+00002880: da02 7762 290b 725d 0000 0072 6000 0000  ..wb).r]...r`...
+00002890: da07 7a69 7066 696c 65da 075a 6970 4669  ..zipfile..ZipFi
+000028a0: 6c65 da0c 5a49 505f 4445 464c 4154 4544  le..ZIP_DEFLATED
+000028b0: 725e 0000 0072 0a00 0000 da08 656e 6473  r^...r......ends
+000028c0: 7769 7468 da04 6f70 656e da05 7772 6974  with..open..writ
+000028d0: 65da 0967 6574 6275 6666 6572 290a 725a  e..getbuffer).rZ
+000028e0: 0000 0072 5400 0000 7250 0000 0072 4d00  ...rT...rP...rM.
+000028f0: 0000 726a 0000 00da 036f 7574 da02 7a66  ..rj.....out..zf
+00002900: da03 696d 67da 0470 6174 68da 0166 7222  ..img..path..fr"
+00002910: 0000 0072 2200 0000 7223 0000 0072 5800  ...r"...r#...rX.
+00002920: 0000 0701 0000 7322 0000 0008 0404 0108  ......s"........
+00002930: 0208 0814 0112 0112 0108 0116 0102 ff1c  ................
+00002940: fd08 060a 0108 010c 0210 0122 ff7a 2145  ...........".z!E
+00002950: 7870 6f72 7450 7265 6469 6374 6976 654d  xportPredictiveM
+00002960: 6f64 656c 2e73 6176 655f 746f 5f7a 6970  odel.save_to_zip
+00002970: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00002980: 0005 0000 0043 0000 0073 4c00 0000 7400  .....C...sL...t.
+00002990: 7401 7c00 8301 8301 6401 6b02 720c 7402  t.|.....d.k.r.t.
+000029a0: 6402 8301 8201 7400 7401 7c00 8301 8301  d.....t.t.|.....
+000029b0: 6403 6b04 7220 7402 6404 7400 7401 7c00  d.k.r t.d.t.t.|.
+000029c0: 8301 8301 9b00 6405 9d03 8301 8201 7403  ......d.......t.
+000029d0: 7c00 7c01 6406 8d02 5300 2907 4ee9 0100  |.|.d...S.).N...
+000029e0: 0000 7a4c 4f6e 6c79 206f 6e65 2063 6c61  ..zLOnly one cla
+000029f0: 7373 2070 7265 7365 6e74 2069 6e20 795f  ss present in y_
+00002a00: 7472 7565 2e20 524f 4320 4155 4320 7363  true. ROC AUC sc
+00002a10: 6f72 6520 6973 206e 6f74 2064 6566 696e  ore is not defin
+00002a20: 6564 2069 6e20 7468 6174 2063 6173 652e  ed in that case.
+00002a30: e902 0000 007a 4441 5543 2065 7661 6c75  .....zDAUC evalu
+00002a40: 6174 696f 6e20 7375 7070 6f72 7473 206f  ation supports o
+00002a50: 6e6c 7920 6269 6e61 7279 206c 6162 656c  nly binary label
+00002a60: 732e 2050 726f 7669 6465 6420 6c61 6265  s. Provided labe
+00002a70: 6c20 636f 6e74 6169 6e73 207a 0e20 756e  l contains z. un
+00002a80: 6971 7565 2076 616c 7565 7329 02da 0679  ique values)...y
+00002a90: 5f74 7275 65da 0779 5f73 636f 7265 2904  _true..y_score).
+00002aa0: 7247 0000 00da 0373 6574 da0a 5661 6c75  rG.....set..Valu
+00002ab0: 6545 7272 6f72 720f 0000 0029 02da 056c  eErrorr....)...l
+00002ac0: 6162 656c da0a 7072 6564 6963 7469 6f6e  abel..prediction
+00002ad0: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
+00002ae0: 0d5f 6576 616c 7561 7465 5f61 7563 2401  ._evaluate_auc$.
+00002af0: 0000 730e 0000 0010 0208 0110 0102 0112  ..s.............
+00002b00: 0104 ff0c 057a 2345 7870 6f72 7450 7265  .....z#ExportPre
+00002b10: 6469 6374 6976 654d 6f64 656c 2e5f 6576  dictiveModel._ev
+00002b20: 616c 7561 7465 5f61 7563 6303 0000 0000  aluate_aucc.....
+00002b30: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
+00002b40: 0000 0073 1400 0000 6401 7c00 a000 7c01  ...s....d.|...|.
+00002b50: 7c02 a102 1400 6402 1800 5300 2903 4e72  |.....d...S.).Nr
+00002b60: 7e00 0000 727d 0000 0029 0172 8500 0000  ~...r}...).r....
+00002b70: 2903 721f 0000 0072 8300 0000 7284 0000  ).r....r....r...
+00002b80: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
+00002b90: da0e 5f65 7661 6c75 6174 655f 6769 6e69  .._evaluate_gini
+00002ba0: 3001 0000 7302 0000 0014 017a 2445 7870  0...s......z$Exp
+00002bb0: 6f72 7450 7265 6469 6374 6976 654d 6f64  ortPredictiveMod
+00002bc0: 656c 2e5f 6576 616c 7561 7465 5f67 696e  el._evaluate_gin
+00002bd0: 6963 0500 0000 0000 0000 0000 0000 0f00  ic..............
+00002be0: 0000 0d00 0000 4300 0000 7334 0100 007c  ......C...s4...|
+00002bf0: 0264 0175 0072 1474 00a0 0164 02a1 0101  .d.u.r.t...d....
+00002c00: 007c 006a 027c 0164 038d 017d 0264 047c  .|.j.|.d...}.d.|
+00002c10: 017c 023c 006e 187c 027c 016a 0376 0172  .|.<.n.|.|.j.v.r
+00002c20: 2c74 00a0 0164 057c 029b 0064 069d 03a1  ,t...d.|...d....
+00002c30: 0101 007c 006a 027c 0164 038d 017d 0264  ...|.j.|.d...}.d
+00002c40: 047c 017c 023c 007c 006a 047c 006a 0564  .|.|.<.|.j.|.j.d
+00002c50: 079c 027d 0567 007d 067c 017c 0219 00a0  ...}.g.}.|.|....
+00002c60: 06a1 007d 077c 04a0 07a1 0044 005d 585c  ...}.|.....D.]X\
+00002c70: 027d 087d 0974 087c 0974 0983 0272 4b7c  .}.}.t.|.t...rK|
+00002c80: 0967 017d 097c 0744 005d 497d 0a7c 017c  .g.}.|.D.]I}.|.|
+00002c90: 0219 007c 0a6b 027d 0b69 007d 0c7c 0944  ...|.k.}.i.}.|.D
+00002ca0: 005d 317d 0d7c 0da0 0aa1 007c 0576 0172  .]1}.|.....|.v.r
+00002cb0: 7374 00a0 0164 087c 0d9b 0064 097c 0d9b  st...d.|...d.|..
+00002cc0: 0064 0a64 0ba0 0b7c 05a1 019b 009d 06a1  .d.d...|........
+00002cd0: 0101 0071 597c 057c 0da0 0aa1 0019 007c  ...qY|.|.......|
+00002ce0: 017c 0b19 007c 0819 007c 017c 0b19 007c  .|...|...|.|...|
+00002cf0: 0319 0083 027d 0e7c 0e7c 0c7c 0da0 0aa1  .....}.|.|.|....
+00002d00: 003c 0071 597c 06a0 0c7c 087c 0aa0 0aa1  .<.qY|...|.|....
+00002d10: 007c 0c64 0c9c 03a1 0101 0071 4d71 3f7c  .|.d.......qMq?|
+00002d20: 0653 0029 0d61 f704 0000 0a20 2020 2020  .S.).a.....     
+00002d30: 2020 2046 756e 6374 696f 6e20 6361 6c63     Function calc
+00002d40: 756c 6174 6573 2064 6966 6665 7265 6e74  ulates different
+00002d50: 2070 6572 666f 726d 616e 6365 206d 6574   performance met
+00002d60: 7269 6373 206f 6620 7072 6564 6963 7469  rics of predicti
+00002d70: 7665 206d 6f64 656c 2e0a 0a20 2020 2020  ve model...     
+00002d80: 2020 203a 7061 7261 6d20 6461 7461 3a20     :param data: 
+00002d90: 4461 7461 7365 7420 746f 2062 6520 7573  Dataset to be us
+00002da0: 6564 2066 6f72 2065 7661 6c75 6174 696e  ed for evaluatin
+00002db0: 6720 7065 7266 6f72 6d61 6e63 652e 0a20  g performance.. 
+00002dc0: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+00002dd0: 6c75 6d6e 5f6e 616d 655f 7361 6d70 6c65  lumn_name_sample
+00002de0: 3a20 4e61 6d65 206f 6620 7468 6520 636f  : Name of the co
+00002df0: 6c75 6d6e 2069 6e73 6964 6520 2764 6174  lumn inside 'dat
+00002e00: 6127 2074 6861 7420 6469 7374 696e 6775  a' that distingu
+00002e10: 6973 6865 7320 7479 7065 206f 6620 6461  ishes type of da
+00002e20: 7461 2073 616d 706c 6573 2e20 436f 6c75  ta samples. Colu
+00002e30: 6d6e 2063 616e 0a20 2020 2020 2020 2020  mn can.         
+00002e40: 2020 2020 2020 636f 6e74 6169 6e20 666f        contain fo
+00002e50: 7220 696e 7374 616e 6365 2076 616c 7565  r instance value
+00002e60: 7320 2774 7261 696e 272c 2027 7661 6c69  s 'train', 'vali
+00002e70: 6427 2c20 2774 6573 7427 2e20 5468 6973  d', 'test'. This
+00002e80: 2077 696c 6c20 6465 6669 6e65 2077 6869   will define whi
+00002e90: 6368 206f 6273 6572 7661 7469 6f6e 7320  ch observations 
+00002ea0: 6265 6c6f 6e67 2074 6f20 7472 6169 6e0a  belong to train.
+00002eb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002ec0: 6574 2c20 7661 6c69 6461 7469 6f6e 2073  et, validation s
+00002ed0: 6574 2061 6e64 2074 6573 7420 7365 742e  et and test set.
+00002ee0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00002ef0: 636f 6c75 6d6e 5f6e 616d 655f 7072 6564  column_name_pred
+00002f00: 6963 7469 6f6e 3a20 4e61 6d65 206f 6620  iction: Name of 
+00002f10: 7468 6520 636f 6c75 6d6e 2069 6e73 6964  the column insid
+00002f20: 6520 2764 6174 6127 2074 6861 7420 686f  e 'data' that ho
+00002f30: 6c64 7320 7661 6c75 6573 206f 6620 7072  lds values of pr
+00002f40: 6564 6963 7469 7665 206d 6f64 656c 2070  edictive model p
+00002f50: 7265 6469 6374 696f 6e2e 0a20 2020 2020  rediction..     
+00002f60: 2020 203a 7061 7261 6d20 6576 616c 7561     :param evalua
+00002f70: 7465 5f70 6572 666f 726d 616e 6365 3a20  te_performance: 
+00002f80: 4469 6374 696f 6e61 7279 2074 6861 7420  Dictionary that 
+00002f90: 6465 6669 6e65 7320 7768 6174 206d 6574  defines what met
+00002fa0: 7269 6373 2073 686f 756c 6420 6265 2065  rics should be e
+00002fb0: 7661 6c75 6174 6564 2e20 4b65 7973 2069  valuated. Keys i
+00002fc0: 6e20 6469 6374 696f 6e61 7279 206d 7573  n dictionary mus
+00002fd0: 7420 7265 6665 720a 2020 2020 2020 2020  t refer.        
+00002fe0: 2020 2020 2020 2074 6f20 636f 6c75 6d6e         to column
+00002ff0: 7320 696e 2027 6461 7461 2720 7468 6174  s in 'data' that
+00003000: 2077 696c 6c20 6265 2075 7365 6420 6173   will be used as
+00003010: 2074 7275 6520 6c61 6265 6c2e 204d 756c   true label. Mul
+00003020: 7469 706c 6520 7472 7565 206c 6162 656c  tiple true label
+00003030: 2063 6f6c 756d 6e73 2063 616e 2062 6520   columns can be 
+00003040: 6465 6669 6e65 642e 2054 6869 7320 6361  defined. This ca
+00003050: 6e20 6265 0a20 2020 2020 2020 2020 2020  n be.           
+00003060: 2020 2020 7573 6566 756c 2066 6f72 2069      useful for i
+00003070: 6e73 7461 6e63 6520 696e 2073 6974 7561  nstance in situa
+00003080: 7469 6f6e 7320 7768 656e 2077 6520 6861  tions when we ha
+00003090: 7665 2062 696e 6172 7920 6c61 6265 6c73  ve binary labels
+000030a0: 2028 696e 6469 6361 746f 7273 206f 6620   (indicators of 
+000030b0: 616e 2065 7665 6e74 2920 6361 6c63 756c  an event) calcul
+000030c0: 6174 6564 206f 7665 720a 2020 2020 2020  ated over.      
+000030d0: 2020 2020 2020 2020 2064 6966 6665 7265           differe
+000030e0: 6e74 2074 696d 6520 7769 6e64 6f77 732e  nt time windows.
+000030f0: 2049 6e20 7661 6c75 6573 2075 6e64 6572   In values under
+00003100: 2065 6163 6820 6b65 792c 206d 6574 7269   each key, metri
+00003110: 6373 2074 6f20 6265 2065 7661 6c75 6174  cs to be evaluat
+00003120: 6564 2061 7265 2064 6566 696e 6564 2e0a  ed are defined..
+00003130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003140: 4578 616d 706c 653a 0a20 2020 2020 2020  Example:.       
+00003150: 2020 2020 2020 2020 6576 616c 7561 7465          evaluate
+00003160: 5f70 6572 666f 726d 616e 6365 203d 207b  _performance = {
+00003170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003180: 2020 2020 276c 6162 656c 5f33 4d27 3a20      'label_3M': 
+00003190: 2741 5543 272c 0a20 2020 2020 2020 2020  'AUC',.         
+000031a0: 2020 2020 2020 2020 2020 276c 6162 656c            'label
+000031b0: 5f31 324d 273a 205b 2741 5543 272c 2027  _12M': ['AUC', '
+000031c0: 4749 4e49 275d 0a20 2020 2020 2020 2020  GINI'].         
+000031d0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000031e0: 3a72 6574 7572 6e3a 2044 6963 7469 6f6e  :return: Diction
+000031f0: 6172 7920 7769 7468 2063 616c 6375 6c61  ary with calcula
+00003200: 7465 6420 7065 7266 6f72 6d61 6e63 6520  ted performance 
+00003210: 6d65 7472 6963 732e 0a20 2020 2020 2020  metrics..       
+00003220: 204e 7a7f 4576 616c 7561 7469 6e67 206d   Nz.Evaluating m
+00003230: 6f64 656c 2070 6572 666f 726d 616e 6365  odel performance
+00003240: 3a20 436f 6c75 6d6e 206e 616d 6520 7769  : Column name wi
+00003250: 7468 2073 616d 706c 6520 7479 7065 2077  th sample type w
+00003260: 6173 206e 6f74 2070 726f 7669 6465 642e  as not provided.
+00003270: 2041 6c6c 206f 6273 6572 7661 7469 6f6e   All observation
+00003280: 7320 7769 6c6c 2062 6520 7472 6561 7465  s will be treate
+00003290: 6420 6173 2074 7261 696e 696e 6720 6461  d as training da
+000032a0: 7461 2ea9 0172 2b00 0000 da05 7472 6169  ta...r+.....trai
+000032b0: 6e7a 4545 7661 6c75 6174 696e 6720 6d6f  nzEEvaluating mo
+000032c0: 6465 6c20 7065 7266 6f72 6d61 6e63 653a  del performance:
+000032d0: 2050 726f 7669 6465 6420 636f 6c75 6d6e   Provided column
+000032e0: 206e 616d 6520 7769 7468 2073 616d 706c   name with sampl
+000032f0: 6520 7479 7065 2027 fa4c 2720 646f 6573  e type '.L' does
+00003300: 206e 6f74 2065 7869 7374 2069 6e20 6461   not exist in da
+00003310: 7461 2e20 416c 6c20 6f62 7365 7276 6174  ta. All observat
+00003320: 696f 6e73 2077 696c 6c20 6265 2074 7265  ions will be tre
+00003330: 6174 6564 2061 7320 7472 6169 6e69 6e67  ated as training
+00003340: 2064 6174 612e 2902 5a03 4155 435a 0447   data.).Z.AUCZ.G
+00003350: 494e 497a 1252 6571 7565 7374 6564 206d  INIz.Requested m
+00003360: 6574 7269 6320 277a 1f27 2069 7320 6e6f  etric 'z.' is no
+00003370: 7420 7375 7070 6f72 7465 642e 2056 616c  t supported. Val
+00003380: 7565 2066 6f72 2027 7a3a 2720 7769 6c6c  ue for 'z:' will
+00003390: 206e 6f74 2062 6520 7374 6f72 6564 2e20   not be stored. 
+000033a0: 5375 7070 6f72 7465 6420 7065 7266 6f72  Supported perfor
+000033b0: 6d61 6e63 6520 6d65 7472 6963 6573 2061  mance metrices a
+000033c0: 7265 3a20 7237 0000 0029 03da 0674 6172  re: r7...)...tar
+000033d0: 6765 74da 0673 616d 706c 65da 0b70 6572  get..sample..per
+000033e0: 666f 726d 616e 6365 290d 723e 0000 0072  formance).r>...r
+000033f0: 3f00 0000 da21 5f67 656e 6572 6174 655f  ?....!_generate_
+00003400: 7361 6d70 6c65 5f74 7970 655f 636f 6c75  sample_type_colu
+00003410: 6d6e 5f6e 616d 6572 4900 0000 7285 0000  mn_namerI...r...
+00003420: 0072 8600 0000 da06 756e 6971 7565 da05  .r......unique..
+00003430: 6974 656d 7372 5c00 0000 da03 7374 72da  itemsr\.....str.
+00003440: 0575 7070 6572 7240 0000 00da 0661 7070  .upperr@.....app
+00003450: 656e 6429 0f72 1f00 0000 722b 0000 0072  end).r....r+...r
+00003460: 3200 0000 7234 0000 0072 3500 0000 5a1f  2...r4...r5...Z.
+00003470: 696d 706c 656d 656e 7465 645f 7065 7266  implemented_perf
+00003480: 6f72 6d61 6e63 655f 6d65 7472 6963 7372  ormance_metricsr
+00003490: 8c00 0000 da15 696e 636c 7564 6564 5f73  ......included_s
+000034a0: 616d 706c 655f 7479 7065 7372 8300 0000  ample_typesr....
+000034b0: da07 6d65 7472 6963 7372 8b00 0000 da04  ..metricsr......
+000034c0: 6d61 736b 5a15 7065 7266 6f72 6d61 6e63  maskZ.performanc
+000034d0: 655f 6279 5f6d 6574 7269 63da 066d 6574  e_by_metric..met
+000034e0: 7269 635a 0c6d 6574 7269 635f 7661 6c75  ricZ.metric_valu
+000034f0: 6572 2200 0000 7222 0000 0072 2300 0000  er"...r"...r#...
+00003500: 724a 0000 0033 0100 0073 4200 0000 081c  rJ...3...sB.....
+00003510: 0401 0201 04ff 0c04 0a01 0a01 0401 0a01  ................
+00003520: 04ff 0c04 0801 0e02 0402 0c01 1001 0a01  ................
+00003530: 0601 0802 0c01 0401 0801 0c01 0401 1a01  ................
+00003540: 06ff 0a04 1401 04ff 0e03 1802 02f2 0410  ................
+00003550: 7a37 4578 706f 7274 5072 6564 6963 7469  z7ExportPredicti
+00003560: 7665 4d6f 6465 6c2e 5f67 6574 5f70 7265  veModel._get_pre
+00003570: 6469 6374 6976 655f 6d6f 6465 6c5f 7065  dictive_model_pe
+00003580: 7266 6f72 6d61 6e63 6563 0100 0000 0000  rformancec......
+00003590: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+000035a0: 0000 7340 0000 0064 017c 006a 0076 0172  ..s@...d.|.j.v.r
+000035b0: 0764 0153 0074 0164 0264 0383 0244 005d  .d.S.t.d.d...D.]
+000035c0: 117d 0164 047c 019b 009d 027c 006a 0076  .}.d.|.....|.j.v
+000035d0: 0172 1d64 047c 019b 009d 0202 0001 0053  .r.d.|.........S
+000035e0: 0071 0c64 0553 0029 064e 728b 0000 0072  .q.d.S.).Nr....r
+000035f0: 7d00 0000 6910 2700 00da 0773 616d 706c  }...i.'....sampl
+00003600: 655f 5a17 636f 6c75 6d6e 5f77 6974 685f  e_Z.column_with_
+00003610: 7361 6d70 6c65 5f74 7970 6529 0272 4900  sample_type).rI.
+00003620: 0000 da05 7261 6e67 6529 0272 2b00 0000  ....range).r+...
+00003630: da01 6972 2200 0000 7222 0000 0072 2300  ..ir"...r"...r#.
+00003640: 0000 728d 0000 0078 0100 0073 0e00 0000  ..r....x...s....
+00003650: 0a02 0401 0e02 1001 0e01 02ff 0402 7a37  ..............z7
+00003660: 4578 706f 7274 5072 6564 6963 7469 7665  ExportPredictive
+00003670: 4d6f 6465 6c2e 5f67 656e 6572 6174 655f  Model._generate_
+00003680: 7361 6d70 6c65 5f74 7970 655f 636f 6c75  sample_type_colu
+00003690: 6d6e 5f6e 616d 6572 3a00 0000 6305 0000  mn_namer:...c...
+000036a0: 0000 0000 0000 0000 000e 0000 000a 0000  ................
+000036b0: 0043 0000 0073 f801 0000 7c03 6401 7500  .C...s....|.d.u.
+000036c0: 7214 7400 a001 6402 a101 0100 7c00 6a02  r.t...d.....|.j.
+000036d0: 7c01 6403 8d01 7d03 6404 7c01 7c03 3c00  |.d...}.d.|.|.<.
+000036e0: 6e18 7c03 7c01 6a03 7601 722c 7400 a001  n.|.|.j.v.r,t...
+000036f0: 6405 7c03 9b00 6406 9d03 a101 0100 7c00  d.|...d.......|.
+00003700: 6a02 7c01 6403 8d01 7d03 6404 7c01 7c03  j.|.d...}.d.|.|.
+00003710: 3c00 6407 7d05 7c04 6401 7500 723a 7400  <.d.}.|.d.u.r:t.
+00003720: a001 6408 a101 0100 6409 7d05 6e2a 7c04  ..d.....d.}.n*|.
+00003730: 7c01 6a03 7601 724b 7400 a001 640a 7c04  |.j.v.rKt...d.|.
+00003740: 9b00 640b 9d03 a101 0100 6409 7d05 6e19  ..d.......d.}.n.
+00003750: 7c01 7c04 1900 6a04 640c 6b03 7264 7405  |.|...j.d.k.rdt.
+00003760: 640a 7c04 9b00 640d 7c01 7c04 1900 6a04  d.|...d.|.|...j.
+00003770: a006 a100 9b00 640e 9d05 8301 0100 6409  ......d.......d.
+00003780: 7d05 6407 7d06 6407 7d07 7c02 6401 7500  }.d.}.d.}.|.d.u.
+00003790: 7274 7400 a001 640f a101 0100 6409 7d06  rtt...d.....d.}.
+000037a0: 6e1b 7c02 7c01 6a03 7601 7285 7400 a001  n.|.|.j.v.r.t...
+000037b0: 6410 7c02 9b00 6411 9d03 a101 0100 6409  d.|...d.......d.
+000037c0: 7d06 6e0a 7c01 7c02 1900 a007 a100 6412  }.n.|.|.......d.
+000037d0: 6b03 728f 6409 7d07 7c01 7c03 1900 a008  k.r.d.}.|.|.....
+000037e0: a100 7d08 6700 7d09 7c08 4400 5d60 7d0a  ..}.g.}.|.D.]`}.
+000037f0: 6413 7c0a a009 a100 6901 7d0b 7c01 7c03  d.|.....i.}.|.|.
+00003800: 1900 7c0a 6b02 7d0c 740a 7c01 7c0c 1900  ..|.k.}.t.|.|...
+00003810: 8301 7c0b 6414 3c00 7c05 72cd 7c01 7c0c  ..|.d.<.|.r.|.|.
+00003820: 1900 7c04 1900 a00b a100 6a0c 6415 6416  ..|.......j.d.d.
+00003830: 8d01 7c0b 6417 3c00 7c01 7c0c 1900 7c04  ..|.d.<.|.|...|.
+00003840: 1900 a00d a100 6a0c 6415 6416 8d01 7c0b  ......j.d.d...|.
+00003850: 6418 3c00 7c06 72f4 7c07 72f4 6700 7c0b  d.<.|.r.|.r.g.|.
+00003860: 6419 3c00 7c01 7c02 1900 a008 a100 a00e  d.<.|.|.........
+00003870: a100 4400 5d16 7d0d 7c0b 6419 1900 a00f  ..D.].}.|.d.....
+00003880: 7c0d 740a 7c01 7c0c 7c01 7c02 1900 7c0d  |.t.|.|.|.|...|.
+00003890: 6b02 4000 1900 8301 641a 9c02 a101 0100  k.@.....d.......
+000038a0: 71dd 7c09 a00f 7c0b a101 0100 7199 7c09  q.|...|.....q.|.
+000038b0: 5300 291b 6132 0300 000a 2020 2020 2020  S.).a2....      
+000038c0: 2020 4675 6e63 7469 6f6e 2065 7661 6c75    Function evalu
+000038d0: 6174 6573 2064 6966 6665 7265 6e74 2064  ates different d
+000038e0: 6573 6372 6970 7469 7665 2069 6e66 6f72  escriptive infor
+000038f0: 6d61 7469 6f6e 2061 626f 7574 206d 6f64  mation about mod
+00003900: 656c 2064 6576 656c 6f70 6d65 6e74 2064  el development d
+00003910: 6174 6120 7361 6d70 6c65 2c20 7375 6368  ata sample, such
+00003920: 2061 7320 7768 6174 2074 696d 6520 7261   as what time ra
+00003930: 6e67 650a 2020 2020 2020 2020 7761 7320  nge.        was 
+00003940: 7573 6564 2c20 7768 6174 2061 7265 2074  used, what are t
+00003950: 6865 2066 7265 7175 656e 6369 6573 206f  he frequencies o
+00003960: 6620 6c61 6265 6c20 636c 6173 7365 7320  f label classes 
+00003970: 616e 6420 6f74 6865 722e 0a0a 2020 2020  and other...    
+00003980: 2020 2020 3a70 6172 616d 2064 6174 613a      :param data:
+00003990: 2044 6174 6173 6574 2074 6f20 6265 2075   Dataset to be u
+000039a0: 7365 6420 666f 7220 6465 7363 7269 7074  sed for descript
+000039b0: 6976 6520 696e 666f 2065 7661 6c75 6174  ive info evaluat
+000039c0: 696f 6e2e 0a20 2020 2020 2020 203a 7061  ion..        :pa
+000039d0: 7261 6d20 636f 6c75 6d6e 5f6e 616d 655f  ram column_name_
+000039e0: 6c61 6265 6c3a 204e 616d 6520 6f66 2074  label: Name of t
+000039f0: 6865 2063 6f6c 756d 6e20 696e 7369 6465  he column inside
+00003a00: 2027 6461 7461 2720 7468 6174 2073 746f   'data' that sto
+00003a10: 7265 7320 6c61 6265 6c73 2e0a 2020 2020  res labels..    
+00003a20: 2020 2020 3a70 6172 616d 2063 6f6c 756d      :param colum
+00003a30: 6e5f 6e61 6d65 5f73 616d 706c 653a 204e  n_name_sample: N
+00003a40: 616d 6520 6f66 2074 6865 2063 6f6c 756d  ame of the colum
+00003a50: 6e20 696e 7369 6465 2027 6461 7461 2720  n inside 'data' 
+00003a60: 7468 6174 2064 6973 7469 6e67 7569 7368  that distinguish
+00003a70: 6573 2074 7970 6520 6f66 2064 6174 6120  es type of data 
+00003a80: 7361 6d70 6c65 732e 2043 6f6c 756d 6e20  samples. Column 
+00003a90: 6361 6e0a 2020 2020 2020 2020 2020 2020  can.            
+00003aa0: 2020 2063 6f6e 7461 696e 2066 6f72 2069     contain for i
+00003ab0: 6e73 7461 6e63 6520 7661 6c75 6573 2027  nstance values '
+00003ac0: 7472 6169 6e27 2c20 2776 616c 6964 272c  train', 'valid',
+00003ad0: 2027 7465 7374 272e 2054 6869 7320 7769   'test'. This wi
+00003ae0: 6c6c 2064 6566 696e 6520 7768 6963 6820  ll define which 
+00003af0: 6f62 7365 7276 6174 696f 6e73 2062 656c  observations bel
+00003b00: 6f6e 6720 746f 2074 7261 696e 0a20 2020  ong to train.   
+00003b10: 2020 2020 2020 2020 2020 2020 7365 742c              set,
+00003b20: 2076 616c 6964 6174 696f 6e20 7365 7420   validation set 
+00003b30: 616e 6420 7465 7374 2073 6574 2e0a 2020  and test set..  
+00003b40: 2020 2020 2020 3a70 6172 616d 2063 6f6c        :param col
+00003b50: 756d 6e5f 6e61 6d65 5f64 6174 653a 204e  umn_name_date: N
+00003b60: 616d 6520 6f66 2074 6865 2063 6f6c 756d  ame of the colum
+00003b70: 6e20 696e 7369 6465 2027 6461 7461 2720  n inside 'data' 
+00003b80: 7468 6174 2073 746f 7265 7320 6461 7465  that stores date
+00003b90: 7320 7265 6c61 7465 6420 746f 206f 6273  s related to obs
+00003ba0: 6572 7661 7469 6f6e 732e 0a20 2020 2020  ervations..     
+00003bb0: 2020 203a 7265 7475 726e 3a20 4469 6374     :return: Dict
+00003bc0: 696f 6e61 7279 2077 6974 6820 6465 7363  ionary with desc
+00003bd0: 7269 7074 6976 6520 696e 666f 2064 6174  riptive info dat
+00003be0: 612e 0a20 2020 2020 2020 204e 7a80 5072  a..        Nz.Pr
+00003bf0: 6570 6172 696e 6720 7361 6d70 6c65 2064  eparing sample d
+00003c00: 6573 6372 6970 7469 6f6e 733a 2043 6f6c  escriptions: Col
+00003c10: 756d 6e20 6e61 6d65 2077 6974 6820 7361  umn name with sa
+00003c20: 6d70 6c65 2074 7970 6520 7761 7320 6e6f  mple type was no
+00003c30: 7420 7072 6f76 6964 6564 2e20 416c 6c20  t provided. All 
+00003c40: 6f62 7365 7276 6174 696f 6e73 2077 696c  observations wil
+00003c50: 6c20 6265 2074 7265 6174 6564 2061 7320  l be treated as 
+00003c60: 7472 6169 6e69 6e67 2064 6174 612e 7287  training data.r.
+00003c70: 0000 0072 8800 0000 7a46 5072 6570 6172  ...r....zFPrepar
+00003c80: 696e 6720 7361 6d70 6c65 2064 6573 6372  ing sample descr
+00003c90: 6970 7469 6f6e 733a 2050 726f 7669 6465  iptions: Provide
+00003ca0: 6420 636f 6c75 6d6e 206e 616d 6520 7769  d column name wi
+00003cb0: 7468 2073 616d 706c 6520 7479 7065 2027  th sample type '
+00003cc0: 7289 0000 0054 7a62 4461 7465 2063 6f6c  r....TzbDate col
+00003cd0: 756d 6e20 6e61 6d65 2028 636f 6c75 6d6e  umn name (column
+00003ce0: 5f6e 616d 655f 6461 7465 2920 7761 7320  _name_date) was 
+00003cf0: 6e6f 7420 7072 6f76 6964 6564 2e20 5469  not provided. Ti
+00003d00: 6d65 2072 656c 6174 6564 206d 6574 6164  me related metad
+00003d10: 6174 6120 7769 6c6c 206e 6f74 2062 6520  ata will not be 
+00003d20: 6576 616c 7561 7465 642e 467a 1b50 726f  evaluated.Fz.Pro
+00003d30: 7669 6465 6420 6461 7465 2063 6f6c 756d  vided date colum
+00003d40: 6e20 6e61 6d65 2027 7a46 2720 646f 6573  n name 'zF' does
+00003d50: 206e 6f74 2065 7869 7374 2069 6e20 6461   not exist in da
+00003d60: 7461 2e20 5469 6d65 2072 656c 6174 6564  ta. Time related
+00003d70: 206d 6574 6164 6174 6120 7769 6c6c 206e   metadata will n
+00003d80: 6f74 2062 6520 6576 616c 7561 7465 642e  ot be evaluated.
+00003d90: 7a07 3c4d 385b 6e73 5d7a 0d27 2069 7320  z.<M8[ns]z.' is 
+00003da0: 6f66 2074 7970 6520 7a49 2e20 5265 7175  of type zI. Requ
+00003db0: 6972 6564 2074 7970 6520 6973 2027 3c4d  ired type is '<M
+00003dc0: 385b 6e73 5d2e 2054 696d 6520 7265 6c61  8[ns]. Time rela
+00003dd0: 7465 6420 6d65 7461 6461 7461 2077 696c  ted metadata wil
+00003de0: 6c20 6e6f 7420 6265 2065 7661 6c75 6174  l not be evaluat
+00003df0: 6564 2e7a 514c 6162 656c 2063 6f6c 756d  ed.zQLabel colum
+00003e00: 6e20 6e61 6d65 2077 6173 206e 6f74 2070  n name was not p
+00003e10: 726f 7669 6465 642e 204c 6162 656c 2072  rovided. Label r
+00003e20: 656c 6174 6564 206d 6574 6164 6174 6120  elated metadata 
+00003e30: 7769 6c6c 206e 6f74 2062 6520 6576 616c  will not be eval
+00003e40: 7561 7465 642e 7a1c 5072 6f76 6964 6564  uated.z.Provided
+00003e50: 206c 6162 656c 2063 6f6c 756d 6e20 6e61   label column na
+00003e60: 6d65 2027 7a47 2720 646f 6573 206e 6f74  me 'zG' does not
+00003e70: 2065 7869 7374 2069 6e20 6461 7461 2e20   exist in data. 
+00003e80: 4c61 6265 6c20 7265 6c61 7465 6420 6d65  Label related me
+00003e90: 7461 6461 7461 2077 696c 6c20 6e6f 7420  tadata will not 
+00003ea0: 6265 2065 7661 6c75 6174 6564 2e72 7e00  be evaluated.r~.
+00003eb0: 0000 da0b 7361 6d70 6c65 5f74 7970 65da  ....sample_type.
+00003ec0: 166e 756d 6265 725f 6f66 5f6f 6273 6572  .number_of_obser
+00003ed0: 7661 7469 6f6e 737a 0825 592d 256d 2d25  vationsz.%Y-%m-%
+00003ee0: 6429 01da 0666 6f72 6d61 745a 0a66 6972  d)...formatZ.fir
+00003ef0: 7374 5f64 6174 655a 096c 6173 745f 6461  st_dateZ.last_da
+00003f00: 7465 5a15 6c61 6265 6c5f 636c 6173 735f  teZ.label_class_
+00003f10: 6672 6571 7565 6e63 7929 02da 0b6c 6162  frequency)...lab
+00003f20: 656c 5f63 6c61 7373 729b 0000 0029 1072  el_classr....).r
+00003f30: 3e00 0000 723f 0000 0072 8d00 0000 7249  >...r?...r....rI
+00003f40: 0000 00da 0564 7479 7065 da05 7072 696e  .....dtype..prin
+00003f50: 74da 075f 5f73 7472 5f5f da07 6e75 6e69  t..__str__..nuni
+00003f60: 7175 6572 8e00 0000 7291 0000 0072 4700  quer....r....rG.
+00003f70: 0000 da03 6d69 6eda 0873 7472 6674 696d  ....min..strftim
+00003f80: 65da 036d 6178 da06 746f 6c69 7374 7292  e..max..tolistr.
+00003f90: 0000 0029 0e72 1f00 0000 722b 0000 0072  ...).r....r+...r
+00003fa0: 3a00 0000 7232 0000 0072 3300 0000 5a0e  :...r2...r3...Z.
+00003fb0: 6461 7465 5f61 7661 696c 6162 6c65 5a0f  date_availableZ.
+00003fc0: 6c61 6265 6c5f 6176 6169 6c61 626c 655a  label_availableZ
+00003fd0: 0c6c 6162 656c 5f62 696e 6172 7972 9300  .label_binaryr..
+00003fe0: 0000 da06 7265 7375 6c74 729a 0000 005a  ....resultr....Z
+00003ff0: 0b73 616d 706c 655f 6d65 7461 7295 0000  .sample_metar...
+00004000: 0072 9d00 0000 7222 0000 0072 2200 0000  .r....r"...r"...
+00004010: 7223 0000 0072 4800 0000 8201 0000 7376  r#...rH.......sv
+00004020: 0000 0008 1304 0102 0104 ff0c 030a 010a  ................
+00004030: 0104 010a 0104 ff0c 0308 0104 0208 0104  ................
+00004040: 0102 0104 ff06 030a 0104 010a 0104 ff06  ................
+00004050: 030e 0102 011a 0104 ff04 0304 0204 0108  ................
+00004060: 010a 0106 010a 0104 010a 0104 ff06 0310  ................
+00004070: 0104 010c 0204 0208 010c 010c 0110 0104  ................
+00004080: 021c 011c 0108 0208 0114 0108 0102 0216  ................
+00004090: 0104 fe06 ff0c 0604 027a 3245 7870 6f72  .........z2Expor
+000040a0: 7450 7265 6469 6374 6976 654d 6f64 656c  tPredictiveModel
+000040b0: 2e5f 6765 745f 6461 7461 5f73 616d 706c  ._get_data_sampl
+000040c0: 655f 6465 7363 7269 7074 696f 6e63 0200  e_descriptionc..
+000040d0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000040e0: 0000 4300 0000 7372 0000 0074 007c 0174  ..C...sr...t.|.t
+000040f0: 0183 0272 0c74 02a0 0364 01a1 0101 0064  ...r.t...d.....d
+00004100: 0253 0074 007c 0174 0483 0272 1874 02a0  .S.t.|.t...r.t..
+00004110: 0364 03a1 0101 0064 0453 0074 007c 0174  .d.....d.S.t.|.t
+00004120: 0583 0272 2474 02a0 0364 05a1 0101 0064  ...r$t...d.....d
+00004130: 0653 0074 007c 0174 066a 0783 0272 3174  .S.t.|.t.j...r1t
+00004140: 02a0 0364 07a1 0101 0064 0853 0074 0864  ...d.....d.S.t.d
+00004150: 097c 006a 099b 009d 0283 0182 0129 0a4e  .|.j.........).N
+00004160: 7a36 4175 746f 6d61 7469 6361 6c6c 7920  z6Automatically 
+00004170: 6173 7369 676e 6564 206d 6f64 656c 2074  assigned model t
+00004180: 7970 6520 4c4f 4749 5354 4943 5f52 4547  ype LOGISTIC_REG
+00004190: 5245 5353 494f 4e2e 7217 0000 007a 2d41  RESSION.r....z-A
+000041a0: 7574 6f6d 6174 6963 616c 6c79 2061 6464  utomatically add
+000041b0: 6564 206d 6f64 656c 2074 7970 6520 5241  ed model type RA
+000041c0: 4e44 4f4d 5f46 4f52 4553 542e 7218 0000  NDOM_FOREST.r...
+000041d0: 007a 2341 7574 6f6d 6174 6963 616c 6c79  .z#Automatically
+000041e0: 2061 6464 6564 206d 6f64 656c 2074 7970   added model typ
+000041f0: 6520 5847 422e 7216 0000 007a 2c41 7574  e XGB.r....z,Aut
+00004200: 6f6d 6174 6963 616c 6c79 2061 6464 6564  omatically added
+00004210: 206d 6f64 656c 2074 7970 6520 4558 5045   model type EXPE
+00004220: 5254 5f53 434f 5245 2e72 1900 0000 7a5b  RT_SCORE.r....z[
+00004230: 4d6f 6465 6c20 7479 7065 2077 6173 206e  Model type was n
+00004240: 6f74 2070 726f 7669 6465 6420 616e 6420  ot provided and 
+00004250: 6e65 6974 6865 7220 6465 7465 6374 6564  neither detected
+00004260: 2061 7574 6f6d 6174 6963 616c 6c79 2e20   automatically. 
+00004270: 4176 6169 6c61 626c 6520 6d6f 6465 6c20  Available model 
+00004280: 7479 7065 7320 6172 653a 2029 0a72 5c00  types are: ).r\.
+00004290: 0000 720d 0000 0072 3e00 0000 7257 0000  ..r....r>...rW..
+000042a0: 0072 0c00 0000 720e 0000 00da 0270 64da  .r....r......pd.
+000042b0: 0944 6174 6146 7261 6d65 da09 5479 7065  .DataFrame..Type
+000042c0: 4572 726f 7272 3d00 0000 2902 721f 0000  Errorr=...).r...
+000042d0: 0072 2700 0000 7222 0000 0072 2200 0000  .r'...r"...r"...
+000042e0: 7223 0000 0072 3c00 0000 d901 0000 731e  r#...r<.......s.
+000042f0: 0000 000a 010a 0104 010a 010a 0104 010a  ................
+00004300: 010a 0104 010c 010a 0104 0102 020a 0104  ................
+00004310: ff7a 2545 7870 6f72 7450 7265 6469 6374  .z%ExportPredict
+00004320: 6976 654d 6f64 656c 2e5f 6765 745f 6d6f  iveModel._get_mo
+00004330: 6465 6c5f 7479 7065 6301 0000 0000 0000  del_typec.......
+00004340: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
+00004350: 0073 1e00 0000 7c00 a000 a100 9b00 6401  .s....|.......d.
+00004360: 7401 6a01 a002 a100 a003 6402 a101 9b00  t.j.......d.....
+00004370: 9d03 5300 2903 4eda 015f 7a0c 2559 256d  ..S.).N.._z.%Y%m
+00004380: 2564 2548 254d 2553 2904 da05 6c6f 7765  %d%H%M%S)...lowe
+00004390: 72da 0864 6174 6574 696d 65da 036e 6f77  r..datetime..now
+000043a0: 72a3 0000 0072 3800 0000 7222 0000 0072  r....r8...r"...r
+000043b0: 2200 0000 7223 0000 0072 4100 0000 eb01  "...r#...rA.....
+000043c0: 0000 7302 0000 001e 027a 2a45 7870 6f72  ..s......z*Expor
+000043d0: 7450 7265 6469 6374 6976 654d 6f64 656c  tPredictiveModel
+000043e0: 2e5f 6765 6e65 7261 7465 5f6d 6f64 656c  ._generate_model
+000043f0: 5f6e 616d 6563 0600 0000 0000 0000 0000  _namec..........
+00004400: 0000 0a00 0000 0a00 0000 4300 0000 7344  ..........C...sD
+00004410: 0100 0067 007d 0667 007d 077c 0364 016b  ...g.}.g.}.|.d.k
+00004420: 0272 427a 1c74 007c 027c 007c 0164 028d  .rBz.t.|.|.|.d..
+00004430: 037d 087c 07a0 0164 0364 0464 059c 02a1  .}.|...d.d.d....
+00004440: 0101 007c 06a0 0164 037c 0864 069c 02a1  ...|...d.|.d....
+00004450: 0101 0057 007c 067c 0766 0253 0004 0074  ...W.|.|.f.S...t
+00004460: 0279 4101 007d 0901 007a 1174 03a0 0464  .yA..}...z.t...d
+00004470: 077c 099b 009d 02a1 0101 0057 0059 0064  .|.........W.Y.d
+00004480: 007d 097e 097c 067c 0766 0253 0064 007d  .}.~.|.|.f.S.d.}
+00004490: 097e 0977 0177 007c 0364 086b 0272 8274  .~.w.w.|.d.k.r.t
+000044a0: 057c 027c 007c 0164 028d 037d 087c 07a0  .|.|.|.d...}.|..
+000044b0: 0164 0364 0464 059c 02a1 0101 007c 06a0  .d.d.d.......|..
+000044c0: 0164 037c 0864 069c 02a1 0101 007c 0564  .d.|.d.......|.d
+000044d0: 0075 0172 7e74 067c 0583 0164 096b 0472  .u.r~t.|...d.k.r
+000044e0: 7e74 077c 027c 0564 0064 0a8d 037d 087c  ~t.|.|.d.d...}.|
+000044f0: 07a0 0164 0b64 0c64 059c 02a1 0101 007c  ...d.d.d.......|
+00004500: 06a0 0164 0b7c 0864 069c 02a1 0101 007c  ...d.|.d.......|
+00004510: 067c 0766 0253 007c 0364 0d6b 0272 9e74  .|.f.S.|.d.k.r.t
+00004520: 087c 027c 007c 017c 0464 0e8d 047d 087c  .|.|.|.|.d...}.|
+00004530: 07a0 0164 0364 0464 059c 02a1 0101 007c  ...d.d.d.......|
+00004540: 06a0 0164 037c 0864 069c 02a1 0101 007c  ...d.|.d.......|
+00004550: 067c 0766 0253 0029 0f4e 7217 0000 0029  .|.f.S.).Nr....)
+00004560: 0372 2700 0000 722b 0000 0072 2800 0000  .r'...r+...r(...
+00004570: 7a10 7368 6170 5f73 756d 6d61 7279 2e73  z.shap_summary.s
+00004580: 7667 5a0c 7368 6170 5f73 756d 6d61 7279  vgZ.shap_summary
+00004590: 2902 7250 0000 00da 0474 7970 6529 0272  ).rP.....type).r
+000045a0: 5000 0000 726f 0000 007a 2646 6169 6c65  P...ro...z&Faile
+000045b0: 6420 746f 2067 656e 6572 6174 6520 5368  d to generate Sh
+000045c0: 6170 2073 756d 6d61 7279 2070 6c6f 743a  ap summary plot:
+000045d0: 2072 1600 0000 7201 0000 0029 0372 2700   r....r....).r'.
+000045e0: 0000 5a12 6576 616c 7561 7469 6f6e 735f  ..Z.evaluations_
+000045f0: 7265 7375 6c74 7296 0000 007a 136c 6561  resultr....z.lea
+00004600: 726e 696e 675f 6375 7276 6573 2e73 7667  rning_curves.svg
+00004610: 5a0f 6c65 6172 6e69 6e67 5f63 7572 7665  Z.learning_curve
+00004620: 7372 1800 0000 2904 7227 0000 0072 2b00  sr....).r'...r+.
+00004630: 0000 7228 0000 0072 2d00 0000 2909 7210  ..r(...r-...).r.
+00004640: 0000 0072 9200 0000 da09 4578 6365 7074  ...r......Except
+00004650: 696f 6e72 3e00 0000 723f 0000 0072 1100  ionr>...r?...r..
+00004660: 0000 7247 0000 0072 1300 0000 7212 0000  ..rG...r....r...
+00004670: 0029 0a72 2b00 0000 7228 0000 0072 2700  .).r+...r(...r'.
+00004680: 0000 722a 0000 0072 2d00 0000 7236 0000  ..r*...r-...r6..
+00004690: 0072 4d00 0000 724e 0000 0072 7a00 0000  .rM...rN...rz...
+000046a0: da01 6572 2200 0000 7222 0000 0072 2300  ..er"...r"...r#.
+000046b0: 0000 724b 0000 00ef 0100 0073 3a00 0000  ..rK.......s:...
+000046c0: 0409 0401 0801 0201 0e01 1001 1201 0813  ................
+000046d0: 0eee 1a01 0811 0880 02ee 0802 0e01 1001  ................
+000046e0: 1001 1402 0e01 1001 1001 0808 08f9 0201  ................
+000046f0: 0801 06ff 1003 1001 0802 7a26 4578 706f  ..........z&Expo
+00004700: 7274 5072 6564 6963 7469 7665 4d6f 6465  rtPredictiveMode
+00004710: 6c2e 5f67 656e 6572 6174 655f 696d 6167  l._generate_imag
+00004720: 6573 2902 7224 0000 004e 290f 4e4e 4e4e  es).r$...N).NNNN
+00004730: 4e4e 4e4e 4e4e 4e4e 4e4e 4e72 2500 0000  NNNNNNNNNNNr%...
+00004740: 2903 4e4e 4e29 024e 4e29 20da 085f 5f6e  ).NNN).NN) ..__n
+00004750: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00004760: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00004770: 3d00 0000 7290 0000 0072 1e00 0000 7226  =...r....r....r&
+00004780: 0000 0072 0400 0000 720d 0000 0072 0c00  ...r....r....r..
+00004790: 0000 720e 0000 0072 a700 0000 72a8 0000  ..r....r....r...
+000047a0: 0072 0200 0000 7205 0000 0072 0300 0000  .r....r....r....
+000047b0: 7207 0000 0072 0600 0000 724f 0000 0072  r....r....rO...r
+000047c0: 5b00 0000 da0c 7374 6174 6963 6d65 7468  [.....staticmeth
+000047d0: 6f64 7258 0000 00da 0566 6c6f 6174 7285  odrX.....floatr.
+000047e0: 0000 0072 8600 0000 724a 0000 0072 8d00  ...r....rJ...r..
+000047f0: 0000 7248 0000 0072 3c00 0000 7241 0000  ..rH...r<...rA..
+00004800: 0072 4b00 0000 da0d 5f5f 636c 6173 7363  .rK.....__classc
+00004810: 656c 6c5f 5f72 2200 0000 7222 0000 0072  ell__r"...r"...r
+00004820: 2000 0000 7223 0000 0072 1500 0000 2400   ...r#...r....$.
+00004830: 0000 7302 0100 0008 0008 011a 020a 0302  ..s.............
+00004840: 0802 0102 0102 0102 0102 0102 0102 0102  ................
+00004850: 0102 0102 0102 0102 0102 0102 0104 ee10  ................
+00004860: 0202 fe06 0302 fd06 0402 fc06 0502 fb08  ................
+00004870: 0602 fa06 0702 f906 0802 f806 0902 f70e  ................
+00004880: 0a02 f606 0b02 f50e 0d02 f306 0e02 f206  ................
+00004890: 0f02 f106 1002 f01a 1102 ef06 1202 ee1e  ................
+000048a0: 130a ed00 7f02 4604 ff0a 0102 ff02 0102  ......F.........
+000048b0: ff12 0102 ff02 020a fe02 1502 0204 ff02  ................
+000048c0: 0102 ff02 0102 ff02 0102 ff12 0102 ff02  ................
+000048d0: 020c fe02 1c10 010e 0b02 0304 0202 fe06  ................
+000048e0: 0302 fd02 0402 fc16 0502 fb12 060a fa02  ................
+000048f0: 4516 0102 0c02 0102 0104 fb04 0202 fe06  E...............
+00004900: 0302 fd06 0402 fc06 0502 fb0e 060a fa12  ................
+00004910: 5702 1214 0102 0302 0602 0104 fa04 0102  W...............
+00004920: ff06 0202 fe02 0302 fd02 0402 fc06 0502  ................
+00004930: fb06 0602 fa12 0714 f972 1500 0000 292c  .........r....),
+00004940: 72ac 0000 0072 5200 0000 5a07 6169 6f68  r....rR...Z.aioh
+00004950: 7474 7072 5500 0000 5a09 7374 7275 6374  ttprU...Z.struct
+00004960: 6c6f 6772 4400 0000 725d 0000 0072 4200  logrD...r]...rB.
+00004970: 0000 7271 0000 00da 0674 7970 696e 6772  ..rq.....typingr
+00004980: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
+00004990: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
+000049a0: 0000 7209 0000 0072 7b00 0000 720a 0000  ..r....r{...r...
+000049b0: 005a 0d72 6571 7565 7374 732e 6175 7468  .Z.requests.auth
+000049c0: 720b 0000 005a 1073 6b6c 6561 726e 2e65  r....Z.sklearn.e
+000049d0: 6e73 656d 626c 6572 0c00 0000 da14 736b  nsembler......sk
+000049e0: 6c65 6172 6e2e 6c69 6e65 6172 5f6d 6f64  learn.linear_mod
+000049f0: 656c 720d 0000 005a 0778 6762 6f6f 7374  elr....Z.xgboost
+00004a00: 720e 0000 00da 0f73 6b6c 6561 726e 2e6d  r......sklearn.m
+00004a10: 6574 7269 6373 720f 0000 0072 6300 0000  etricsr....rc...
+00004a20: da06 7061 6e64 6173 72a7 0000 005a 3d74  ..pandasr....Z=t
+00004a30: 6172 616e 646d 5f61 6e61 6c79 7469 6373  arandm_analytics
+00004a40: 2e65 7870 6f72 745f 7072 6564 6963 7469  .export_predicti
+00004a50: 7665 5f6d 6f64 656c 2e6d 6f64 656c 5f76  ve_model.model_v
+00004a60: 6973 7561 6c69 7a61 7469 6f6e 7210 0000  isualizationr...
+00004a70: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00004a80: 5a16 7461 7261 6e64 6d5f 616e 616c 7974  Z.tarandm_analyt
+00004a90: 6963 732e 6261 7365 7214 0000 00da 0a67  ics.baser......g
+00004aa0: 6574 5f6c 6f67 6765 7272 b100 0000 723e  et_loggerr....r>
+00004ab0: 0000 0072 1500 0000 7222 0000 0072 2200  ...r....r"...r".
+00004ac0: 0000 7222 0000 0072 2300 0000 da08 3c6d  ..r"...r#.....<m
+00004ad0: 6f64 756c 653e 0100 0000 732e 0000 0008  odule>....s.....
+00004ae0: 0008 0108 0208 0108 0108 0208 0108 0108  ................
+00004af0: 0120 0110 020c 010c 010c 010c 010c 010c  . ..............
+00004b00: 0108 0108 0218 020c 060a 0214 03         .............
```

### Comparing `tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc` & `tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/create_predictive_model.py` & `tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/create_predictive_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import datetime
-
-import aiohttp
+import requests
 import structlog
 
 import base64
 import io
 import pickle
 import zipfile
 from typing import List, Dict, Union, Optional, Any, Tuple
 
-from aiohttp import ClientTimeout, ClientSession
 from path import Path
+from requests.auth import HTTPBasicAuth
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.linear_model import LogisticRegression
 from xgboost import Booster
 from sklearn.metrics import roc_auc_score
 import os
 
 import pandas as pd
@@ -232,35 +231,33 @@
             target_class=target_class,
             learning_curves_data=learning_curves_data
         )
         request_data["attached_images"] = images_meta
 
         return request_data, images
 
-    async def build_predictive_model(
-        self, request_data, filename: str, images: Optional[List[Dict[str, Any]]] = None
+    def build_predictive_model(
+        self, request_data: Dict[str, Any], filename: str, images: Optional[List[Dict[str, Any]]] = None
     ) -> None:
         if images is None:
             images = []
 
         url = self.endpoint_url + "analytics/build_predictive_model"
-        authentication = aiohttp.BasicAuth(login=self.username, password=self.password)
-        async with ClientSession(auth=authentication, timeout=ClientTimeout(total=20)) as session:
-            response = await session.get(url=url, json=request_data)
-            if response.status == 200:
-                logger.info("Successfully called 'analytics/build_predictive_model' endpoint.")
-                response_data = await response.json()
-            else:
-                response_message = await response.json()
-                logger.error(f"Unable to call 'analytics/build_predictive_model' endpoint: {response_message['message']}")
-                return None
-            extended_model_yaml = response_data["extended_predictive_model_yaml"]
-            external_model_json = response_data["external_model_json"]
+        response = requests.post(url=url, json=request_data, auth=HTTPBasicAuth(self.username, self.password))
+
+        if response.status_code == 200:
+            logger.info("Successfully called 'analytics/build_predictive_model' endpoint.")
+            response_data = response.json()
+        else:
+            logger.error(f"Unable to call 'analytics/build_predictive_model' endpoint: {response.text}")
+            return None
+        extended_model_yaml = response_data["extended_predictive_model_yaml"]
+        external_model_json = response_data["external_model_json"]
 
-            self.save_to_zip(extended_model_yaml, external_model_json, filename, images)
+        self.save_to_zip(extended_model_yaml, external_model_json, filename, images)
 
     @staticmethod
     def save_to_zip(
         extended_model_yaml: str, external_model_json: str, filename: str, images: Optional[List[Dict[str, Any]]] = None
     ) -> None:
         if images is None:
             images = []
```

### Comparing `tarandm_analytics-0.0.4/tarandm_analytics/export_predictive_model/model_visualization.py` & `tarandm_analytics-0.0.5/tarandm_analytics/export_predictive_model/model_visualization.py`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.4/PKG-INFO` & `tarandm_analytics-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: tarandm-analytics
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package contains support functions for creating predictive models in format compatible with TaranDM software.
 Author: Marek Teller
 Author-email: mteller@taran.ai
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: aiohttp
 Requires-Dist: llvmlite
 Requires-Dist: matplotlib
 Requires-Dist: numba (==0.56.4)
 Requires-Dist: pandas
 Requires-Dist: path
+Requires-Dist: requests
 Requires-Dist: scikit-learn (==1.2.2)
 Requires-Dist: shap
 Requires-Dist: structlog
 Requires-Dist: xgboost
 Description-Content-Type: text/markdown
 
 # Predictive model support
```

