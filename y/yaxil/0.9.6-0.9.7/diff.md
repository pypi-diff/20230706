# Comparing `tmp/yaxil-0.9.6-py2.py3-none-any.whl.zip` & `tmp/yaxil-0.9.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 30410 bytes, number of entries: 19
--rw-r--r--  2.0 unx    46800 b- defN 23-Jun-21 15:18 yaxil/__init__.py
--rw-r--r--  2.0 unx      232 b- defN 23-Jun-26 17:34 yaxil/__version__.py
--rw-r--r--  2.0 unx       84 b- defN 23-Jun-08 16:34 yaxil/assessments/__init__.py
--rw-r--r--  2.0 unx    22420 b- defN 23-Jun-08 16:34 yaxil/assessments/neuroinfo/__init__.py
--rw-r--r--  2.0 unx     7117 b- defN 23-Jun-08 16:34 yaxil/assessments/neuroinfo/legacy/__init__.py
--rw-r--r--  2.0 unx      699 b- defN 23-Jun-08 16:34 yaxil/assessments/neuroinfo/session/__init__.py
--rw-r--r--  2.0 unx    16280 b- defN 23-Jun-08 16:34 yaxil/bids/__init__.py
--rw-r--r--  2.0 unx     2805 b- defN 23-Jun-08 16:34 yaxil/commons/__init__.py
--rw-r--r--  2.0 unx     1656 b- defN 23-Jun-08 16:34 yaxil/dicom/__init__.py
--rw-r--r--  2.0 unx      625 b- defN 23-Jun-08 16:34 yaxil/exceptions/__init__.py
--rw-r--r--  2.0 unx      783 b- defN 23-Jun-08 16:34 yaxil/functools/__init__.py
--rw-r--r--  2.0 unx     1477 b- defN 23-Jun-08 16:34 yaxil/session/__init__.py
--rwxr-xr-x  2.0 unx     9426 b- defN 23-Jun-26 17:35 yaxil-0.9.6.data/scripts/ArcGet.py
--rwxr-xr-x  2.0 unx     4114 b- defN 23-Jun-26 17:35 yaxil-0.9.6.data/scripts/xnat_auth
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      387 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1586 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/RECORD
-19 files, 118148 bytes uncompressed, 27814 bytes compressed:  76.5%
+Zip file size: 30660 bytes, number of entries: 19
+-rw-r--r--  2.0 unx    46800 b- defN 23-Jul-06 18:06 yaxil/__init__.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-06 18:09 yaxil/__version__.py
+-rw-r--r--  2.0 unx       84 b- defN 23-Jul-06 18:06 yaxil/assessments/__init__.py
+-rw-r--r--  2.0 unx    25532 b- defN 23-Jul-06 18:06 yaxil/assessments/neuroinfo/__init__.py
+-rw-r--r--  2.0 unx     7117 b- defN 23-Jul-06 18:06 yaxil/assessments/neuroinfo/legacy/__init__.py
+-rw-r--r--  2.0 unx      699 b- defN 23-Jul-06 18:06 yaxil/assessments/neuroinfo/session/__init__.py
+-rw-r--r--  2.0 unx    16280 b- defN 23-Jul-06 18:06 yaxil/bids/__init__.py
+-rw-r--r--  2.0 unx     2805 b- defN 23-Jul-06 18:06 yaxil/commons/__init__.py
+-rw-r--r--  2.0 unx     1656 b- defN 23-Jul-06 18:06 yaxil/dicom/__init__.py
+-rw-r--r--  2.0 unx      625 b- defN 23-Jul-06 18:06 yaxil/exceptions/__init__.py
+-rw-r--r--  2.0 unx      783 b- defN 23-Jul-06 18:06 yaxil/functools/__init__.py
+-rw-r--r--  2.0 unx     1477 b- defN 23-Jul-06 18:06 yaxil/session/__init__.py
+-rwxr-xr-x  2.0 unx     9426 b- defN 23-Jul-06 18:13 yaxil-0.9.7.data/scripts/ArcGet.py
+-rwxr-xr-x  2.0 unx     4114 b- defN 23-Jul-06 18:13 yaxil-0.9.7.data/scripts/xnat_auth
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jul-06 18:13 yaxil-0.9.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      387 b- defN 23-Jul-06 18:13 yaxil-0.9.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-06 18:13 yaxil-0.9.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-06 18:13 yaxil-0.9.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1586 b- defN 23-Jul-06 18:13 yaxil-0.9.7.dist-info/RECORD
+19 files, 121260 bytes uncompressed, 28064 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -30,29 +30,29 @@
 
 Filename: yaxil/functools/__init__.py
 Comment: 
 
 Filename: yaxil/session/__init__.py
 Comment: 
 
-Filename: yaxil-0.9.6.data/scripts/ArcGet.py
+Filename: yaxil-0.9.7.data/scripts/ArcGet.py
 Comment: 
 
-Filename: yaxil-0.9.6.data/scripts/xnat_auth
+Filename: yaxil-0.9.7.data/scripts/xnat_auth
 Comment: 
 
-Filename: yaxil-0.9.6.dist-info/LICENSE
+Filename: yaxil-0.9.7.dist-info/LICENSE
 Comment: 
 
-Filename: yaxil-0.9.6.dist-info/METADATA
+Filename: yaxil-0.9.7.dist-info/METADATA
 Comment: 
 
-Filename: yaxil-0.9.6.dist-info/WHEEL
+Filename: yaxil-0.9.7.dist-info/WHEEL
 Comment: 
 
-Filename: yaxil-0.9.6.dist-info/top_level.txt
+Filename: yaxil-0.9.7.dist-info/top_level.txt
 Comment: 
 
-Filename: yaxil-0.9.6.dist-info/RECORD
+Filename: yaxil-0.9.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yaxil/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'yaxil'
 __description__ = 'Yet another XNAT interface libary'
 __url__ = 'https://github.com/harvard-nrg/yaxil'
-__version__ = '0.9.6'
+__version__ = '0.9.7'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## yaxil/assessments/neuroinfo/__init__.py

```diff
@@ -457,14 +457,92 @@
     'neuroinfo:anatqc/manual/spike': 'manual_spike',
     'neuroinfo:anatqc/manual/art_brain': 'manual_art_brain',
     'neuroinfo:anatqc/manual/art_out': 'manual_art_out',
     'neuroinfo:anatqc/manual/inhom': 'manual_inhom',
     'neuroinfo:anatqc/manual/overall': 'manual_overall'
 }
 
+def dwiqc(auth, label=None, scan_ids=None, project=None, aid=None):
+    '''
+    Get DwiQC data as a sequence of dictionaries.
+
+    Example:
+        >>> import json
+        >>> import yaxil.assessments.neuroinfo as neuroinfo
+        >>> auth = yaxil.auth('doctest')
+        >>> for qc in neuroinfo.dwiqc(auth, 'TestSession01'):
+        ...   print(json.dumps(qc, indent=2))
+        {
+          "id": "TestSession01_DWI_30_DWIQC",
+          ...
+        }
+
+    :param auth: XNAT authentication object
+    :type auth: :mod:`yaxil.XnatAuth`
+    :param label: XNAT MR Session label
+    :type label: str
+    :param scan_ids: Scan numbers to include
+    :type scan_ids: list
+    :param project: XNAT MR Session project
+    :type project: str
+    :param aid: XNAT MR Session Accession ID
+    :type aid: str
+    :returns: Generator of DwiQC data dictionaries
+    :rtype: :mod:`dict`
+    '''
+
+    if not aid:
+        aid = yaxil.accession(auth, label, project)
+    experiment_details = yaxil.__experiment_details(auth, aid)
+    path = '/data/experiments'
+    params = {
+        'xsiType': 'neuroinfo:dwiqc',
+        'columns': ','.join(dwiqc.columns.keys())
+    }
+    if project:
+        params['project'] = project
+    params['xnat:mrSessionData/ID'] = aid
+    _,result = yaxil._get(auth, path, 'json', autobox=True, params=params)
+    for result in result['ResultSet']['Result']:
+        if scan_ids == None or result['neuroinfo:dwiqc/dwi_scan_id'] in scan_ids:
+            data = dict()
+            for k,v in iter(dwiqc.columns.items()):
+                data[v] = result[k]
+            files = __files(auth, result['neuroinfo:dwiqc/id'])
+            data.update(experiment_details)
+            data['files'] = files
+            yield data
+dwiqc.columns = {
+    'neuroinfo:dwiQC/id': 'ID',
+    'neuroinfo:dwiQC/id': 'id',
+    'neuroinfo:dwiQC/date': 'date',
+    'neuroinfo:dwiQC/time': 'time',
+    'neuroinfo:dwiQC/imagesession_id': 'session_id',
+    'neuroinfo:dwiQC/dwi_scan_id': 'dwi_scan_id',
+    'neuroinfo:dwiQC/ap_fmap_scan_id': 'ap_fmap_scan_id',
+    'neuroinfo:dwiQC/pa_fmap_scan_id': 'pa_fmap_scan_id',    
+    'neuroinfo:dwiQC/session_label': 'session_label',
+    'neuroinfo:dwiQC/eddy_quad/Average_abs_motion_mm': 'Average_abs_motion_mm',
+    'neuroinfo:dwiQC/eddy_quad/Average_rel_motion_mm': 'Average_rel_motion_mm',
+    'neuroinfo:dwiQC/eddy_quad/Average_x_translation_motion_mm': 'Average_x_translation_mm',
+    'neuroinfo:dwiQC/eddy_quad/Average_y_translation_motion_mm': 'Average_y_translation_mm',
+    'neuroinfo:dwiQC/eddy_quad/Average_z_translation_motion_mm': 'Average_z_translation_mm',
+    'neuroinfo:dwiQC/eddy_quad/Average_SNR_B0': 'Average_SNR_B0',
+    'neuroinfo:dwiQC/manual/wrap': 'manual_wrap',
+    'neuroinfo:dwiQC/manual/motion': 'manual_motion',
+    'neuroinfo:dwiQC/manual/cover': 'manual_cover',
+    'neuroinfo:dwiQC/manual/ghost_brain': 'manual_ghost_brain',
+    'neuroinfo:dwiQC/manual/ghost_out': 'manual_ghost_out',
+    'neuroinfo:dwiQC/manual/spike': 'manual_spike',
+    'neuroinfo:dwiQC/manual/inhom': 'manual_inhom',
+    'neuroinfo:dwiQC/manual/overall': 'manual_overall'
+}
+
+
+
 def __files(auth, aid):
     path = f'/data/experiments/{aid}/files'
     _,result = yaxil._get(auth, path, 'json', autobox=True)
     files = dict()
     for result in result['ResultSet']['Result']:
         name = result['URI'].split('/')[-2]
         files[name] = result
```

## Comparing `yaxil-0.9.6.data/scripts/ArcGet.py` & `yaxil-0.9.7.data/scripts/ArcGet.py`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.6.data/scripts/xnat_auth` & `yaxil-0.9.7.data/scripts/xnat_auth`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.6.dist-info/LICENSE` & `yaxil-0.9.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.6.dist-info/RECORD` & `yaxil-0.9.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 yaxil/__init__.py,sha256=ORVt8FrzAKC-vkG6-Nmne_ydZUgjnojDPgoAN3iXHsE,46800
-yaxil/__version__.py,sha256=0zVgEkhBwHX85OKt-YQ8cVmtB--owN0Iedwbh9iBVTc,232
+yaxil/__version__.py,sha256=nqteRgdfAtEhbOw1wgndcoOW4Xe06Jf3zSIH-I3ZhtM,232
 yaxil/assessments/__init__.py,sha256=TpcTgZ9L8FnHvBOwkeK07BDBnoqqHLV1hVaVG9-yXg8,84
-yaxil/assessments/neuroinfo/__init__.py,sha256=HLA6BTTUeUWDau6k-_yJnM1rDlXHOyTI5cEbACpsGK8,22420
+yaxil/assessments/neuroinfo/__init__.py,sha256=OSbI5e2mwXtnp4bHvZvktaRrUziQDhTcz4mYPmYpM1M,25532
 yaxil/assessments/neuroinfo/legacy/__init__.py,sha256=k7kzdPUCcFDE7CWYzLQj6KkgokcZPiAwa0Pp62-V2fY,7117
 yaxil/assessments/neuroinfo/session/__init__.py,sha256=W3COlgCEoyO0hth3idT1JP7IRhaFmT0CC7lNxVG0uRs,699
 yaxil/bids/__init__.py,sha256=I4VUikLW9gLwfPmEpw4SXJDSa_riBX7IOPryykxOFF8,16280
 yaxil/commons/__init__.py,sha256=lCdwSNdIavfJi5Wux0mZ5Ay_HgKU-FnG-X6vZclDq24,2805
 yaxil/dicom/__init__.py,sha256=hsrcXBZDMBJDrDtaGuVG-T8Btb-EDBSAf5PJbs-qht0,1656
 yaxil/exceptions/__init__.py,sha256=1xNTBxyCkWGevMNBe1kbESSMD5gH06bOG_3XUMYcUHQ,625
 yaxil/functools/__init__.py,sha256=P5yiAU1yotWAFPTi0_rs9SpKTxj1EH9NeBjVMHG3lGs,783
 yaxil/session/__init__.py,sha256=Tr9ALXprn6Xnx6smZHJgOcSBESMkgjB3dSnW_RnrZh8,1477
-yaxil-0.9.6.data/scripts/ArcGet.py,sha256=eNhHHTVeBgkkaZVu1fdLgiJv0ZHSGqNQU9aTRU-hIrU,9426
-yaxil-0.9.6.data/scripts/xnat_auth,sha256=wQ1aNeFxLjtarDu7LqdG-zEepMUShVjw0av_sT8uv3w,4114
-yaxil-0.9.6.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
-yaxil-0.9.6.dist-info/METADATA,sha256=1DlqDDSElq5h6oqB0WEwS3stiW9Kx8MPuKFq5kLRCJs,387
-yaxil-0.9.6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-yaxil-0.9.6.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
-yaxil-0.9.6.dist-info/RECORD,,
+yaxil-0.9.7.data/scripts/ArcGet.py,sha256=eNhHHTVeBgkkaZVu1fdLgiJv0ZHSGqNQU9aTRU-hIrU,9426
+yaxil-0.9.7.data/scripts/xnat_auth,sha256=wQ1aNeFxLjtarDu7LqdG-zEepMUShVjw0av_sT8uv3w,4114
+yaxil-0.9.7.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
+yaxil-0.9.7.dist-info/METADATA,sha256=EHxEWyz8L3RGmGGwc-9SSPuO_FVMFwPDA-USqZjObfM,387
+yaxil-0.9.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+yaxil-0.9.7.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
+yaxil-0.9.7.dist-info/RECORD,,
```

