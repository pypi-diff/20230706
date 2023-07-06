# Comparing `tmp/axion-3.4.7-cp311-none-win_amd64.whl.zip` & `tmp/axion-3.4.8-cp311-none-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 626024 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-24 06:36 axion-3.4.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2415 b- defN 23-Jun-24 06:36 axion-3.4.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-24 06:36 axion-3.4.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-24 06:36 axion-3.4.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      376 b- defN 23-Jun-24 06:36 axion-3.4.7.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20992 b- defN 23-Jun-24 06:36 axion/__init__.pyd
--rw-rw-rw-  2.0 fat    80384 b- defN 23-Jun-24 06:36 axion/executor.pyd
--rw-rw-rw-  2.0 fat   261120 b- defN 23-Jun-24 06:36 axion/factory.pyd
--rw-rw-rw-  2.0 fat    78848 b- defN 23-Jun-24 06:36 axion/pipeline.pyd
--rw-rw-rw-  2.0 fat    53248 b- defN 23-Jun-24 06:36 axion/queues.pyd
--rw-rw-rw-  2.0 fat   208896 b- defN 23-Jun-24 06:36 axion/recorder.pyd
--rw-rw-rw-  2.0 fat    56320 b- defN 23-Jun-24 06:36 axion/scheduler.pyd
--rw-rw-rw-  2.0 fat    71168 b- defN 23-Jun-24 06:36 axion/service.pyd
--rw-rw-rw-  2.0 fat    67072 b- defN 23-Jun-24 06:36 axion/thread.pyd
--rw-rw-rw-  2.0 fat    22016 b- defN 23-Jun-24 06:36 axion/inst/__init__.pyd
--rw-rw-rw-  2.0 fat    49664 b- defN 23-Jun-24 06:36 axion/inst/ibase.pyd
--rw-rw-rw-  2.0 fat   221696 b- defN 23-Jun-24 06:36 axion/inst/nbase.pyd
--rw-rw-rw-  2.0 fat    88064 b- defN 23-Jun-24 06:36 axion/inst/sbase.pyd
--rw-rw-rw-  2.0 fat    63488 b- defN 23-Jun-24 06:36 axion/inst/tbase.pyd
--rw-rw-rw-  2.0 fat    61440 b- defN 23-Jun-24 06:36 axion/inst/utility.pyd
-20 files, 1408388 bytes uncompressed, 623620 bytes compressed:  55.7%
+Zip file size: 1496117 bytes, number of entries: 20
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jul-05 23:53 axion-3.4.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2362 b- defN 23-Jul-05 23:53 axion-3.4.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 23-Jul-05 23:53 axion-3.4.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-05 23:53 axion-3.4.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      376 b- defN 23-Jul-05 23:53 axion-3.4.8.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   122763 b- defN 23-Jul-05 23:52 axion/__init__.so
+-rwxr-xr-x  2.0 unx   309099 b- defN 23-Jul-05 23:52 axion/executor.so
+-rwxr-xr-x  2.0 unx   863962 b- defN 23-Jul-05 23:52 axion/factory.so
+-rwxr-xr-x  2.0 unx   292267 b- defN 23-Jul-05 23:52 axion/pipeline.so
+-rwxr-xr-x  2.0 unx   219465 b- defN 23-Jul-05 23:52 axion/queues.so
+-rwxr-xr-x  2.0 unx   731275 b- defN 23-Jul-05 23:52 axion/recorder.so
+-rwxr-xr-x  2.0 unx   220716 b- defN 23-Jul-05 23:52 axion/scheduler.so
+-rwxr-xr-x  2.0 unx   275562 b- defN 23-Jul-05 23:52 axion/service.so
+-rwxr-xr-x  2.0 unx   273129 b- defN 23-Jul-05 23:52 axion/thread.so
+-rwxr-xr-x  2.0 unx   122987 b- defN 23-Jul-05 23:53 axion/inst/__init__.so
+-rwxr-xr-x  2.0 unx   217992 b- defN 23-Jul-05 23:52 axion/inst/ibase.so
+-rwxr-xr-x  2.0 unx   733160 b- defN 23-Jul-05 23:53 axion/inst/nbase.so
+-rwxr-xr-x  2.0 unx   329192 b- defN 23-Jul-05 23:53 axion/inst/sbase.so
+-rwxr-xr-x  2.0 unx   240760 b- defN 23-Jul-05 23:53 axion/inst/tbase.so
+-rwxr-xr-x  2.0 unx   274282 b- defN 23-Jul-05 23:53 axion/inst/utility.so
+20 files, 5230522 bytes uncompressed, 1493743 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -1,61 +1,61 @@
-Filename: axion-3.4.7.dist-info/LICENSE
+Filename: axion-3.4.8.dist-info/LICENSE
 Comment: 
 
-Filename: axion-3.4.7.dist-info/METADATA
+Filename: axion-3.4.8.dist-info/METADATA
 Comment: 
 
-Filename: axion-3.4.7.dist-info/WHEEL
+Filename: axion-3.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: axion-3.4.7.dist-info/top_level.txt
+Filename: axion-3.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: axion-3.4.7.dist-info/RECORD
+Filename: axion-3.4.8.dist-info/RECORD
 Comment: 
 
-Filename: axion/__init__.pyd
+Filename: axion/__init__.so
 Comment: 
 
-Filename: axion/executor.pyd
+Filename: axion/executor.so
 Comment: 
 
-Filename: axion/factory.pyd
+Filename: axion/factory.so
 Comment: 
 
-Filename: axion/pipeline.pyd
+Filename: axion/pipeline.so
 Comment: 
 
-Filename: axion/queues.pyd
+Filename: axion/queues.so
 Comment: 
 
-Filename: axion/recorder.pyd
+Filename: axion/recorder.so
 Comment: 
 
-Filename: axion/scheduler.pyd
+Filename: axion/scheduler.so
 Comment: 
 
-Filename: axion/service.pyd
+Filename: axion/service.so
 Comment: 
 
-Filename: axion/thread.pyd
+Filename: axion/thread.so
 Comment: 
 
-Filename: axion/inst/__init__.pyd
+Filename: axion/inst/__init__.so
 Comment: 
 
-Filename: axion/inst/ibase.pyd
+Filename: axion/inst/ibase.so
 Comment: 
 
-Filename: axion/inst/nbase.pyd
+Filename: axion/inst/nbase.so
 Comment: 
 
-Filename: axion/inst/sbase.pyd
+Filename: axion/inst/sbase.so
 Comment: 
 
-Filename: axion/inst/tbase.pyd
+Filename: axion/inst/tbase.so
 Comment: 
 
-Filename: axion/inst/utility.pyd
+Filename: axion/inst/utility.so
 Comment: 
 
 Zip file comment:
```

## Comparing `axion-3.4.7.dist-info/METADATA` & `axion-3.4.8.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-Metadata-Version: 2.1
-Name: axion
-Version: 3.4.7
-Summary: Dream It Possible!
-Author-email: YL <fengyl@pku.edu.cn>
-License: MIT License
-        
-        Copyright (c) 2021 YL
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://gitee.com
-Project-URL: documentation, https://gitee.com
-Project-URL: bugs, https://gitee.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy (>=1.20.0)
-Requires-Dist: h5py (>=3.0.0)
-Requires-Dist: psutil (>=5.8.0)
-Requires-Dist: srpc (>=4.2.8)
-Requires-Dist: zee (>=0.0.3)
-Requires-Dist: dill (>=0.3.4)
-Requires-Dist: networkx (>=2.5.0)
-Requires-Dist: pyparsing (>3.0.0)
-
+Metadata-Version: 2.1
+Name: axion
+Version: 3.4.8
+Summary: Dream It Possible!
+Author-email: YL <fengyl@pku.edu.cn>
+License: MIT License
+        
+        Copyright (c) 2021 YL
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://gitee.com
+Project-URL: documentation, https://gitee.com
+Project-URL: bugs, https://gitee.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy (>=1.20.0)
+Requires-Dist: h5py (>=3.0.0)
+Requires-Dist: psutil (>=5.8.0)
+Requires-Dist: srpc (>=4.2.8)
+Requires-Dist: zee (>=0.0.3)
+Requires-Dist: dill (>=0.3.4)
+Requires-Dist: networkx (>=2.5.0)
+Requires-Dist: pyparsing (>3.0.0)
+
```

