# Comparing `tmp/tja2fumen-0.3.0.tar.gz` & `tmp/tja2fumen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.3.0.tar", last modified: Wed Jul  5 20:10:18 2023, max compression
+gzip compressed data, was "tja2fumen-0.4.0.tar", last modified: Thu Jul  6 03:55:54 2023, max compression
```

## Comparing `tja2fumen-0.3.0.tar` & `tja2fumen-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.502142 tja2fumen-0.3.0/
--rw-rw-rw-   0        0        0     1083 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4388 2023-07-05 20:10:18.502142 tja2fumen-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2669 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/README.md
--rw-rw-rw-   0        0        0      897 2023-07-05 20:10:07.000000 tja2fumen-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 20:10:18.502142 tja2fumen-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.470891 tja2fumen-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.486514 tja2fumen-0.3.0/src/tja2fumen/
--rw-rw-rw-   0        0        0     1825 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     3856 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    15536 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    19843 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.502142 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/
--rw-rw-rw-   0        0        0    23889 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
--rw-rw-rw-   0        0        0    23889 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
--rw-rw-rw-   0        0        0    23890 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
--rw-rw-rw-   0        0        0    23886 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
--rw-rw-rw-   0        0        0    23884 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
--rw-rw-rw-   0        0        0    23884 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
--rw-rw-rw-   0        0        0    23883 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
--rw-rw-rw-   0        0        0    23889 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
--rw-rw-rw-   0        0        0    23889 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
--rw-rw-rw-   0        0        0    23887 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
--rw-rw-rw-   0        0        0    23886 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
--rw-rw-rw-   0        0        0    23880 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
--rw-rw-rw-   0        0        0    23872 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
--rw-rw-rw-   0        0        0    23869 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
--rw-rw-rw-   0        0        0     3308 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     2905 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.486514 tja2fumen-0.3.0/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     4388 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.344051 tja2fumen-0.4.0/
+-rw-rw-rw-   0        0        0     1083 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4388 2023-07-06 03:55:54.344051 tja2fumen-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/README.md
+-rw-rw-rw-   0        0        0      897 2023-07-06 03:55:38.000000 tja2fumen-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:55:54.344051 tja2fumen-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.312815 tja2fumen-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.328426 tja2fumen-0.4.0/src/tja2fumen/
+-rw-rw-rw-   0        0        0     1825 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     3856 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    15705 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0    19907 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.344051 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/
+-rw-rw-rw-   0        0        0    23889 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
+-rw-rw-rw-   0        0        0    23890 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
+-rw-rw-rw-   0        0        0    23883 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
+-rw-rw-rw-   0        0        0    23887 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
+-rw-rw-rw-   0        0        0    23880 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
+-rw-rw-rw-   0        0        0    23872 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
+-rw-rw-rw-   0        0        0    23869 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
+-rw-rw-rw-   0        0        0     3308 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/utils.py
+-rw-rw-rw-   0        0        0     2905 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.328426 tja2fumen-0.4.0/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0     4388 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.3.0/LICENSE.txt` & `tja2fumen-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/PKG-INFO` & `tja2fumen-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.3.0/README.md` & `tja2fumen-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/pyproject.toml` & `tja2fumen-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.3.0"
+version = "0.4.0"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
```

### Comparing `tja2fumen-0.3.0/src/tja2fumen/__init__.py` & `tja2fumen-0.4.0/src/tja2fumen/__init__.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/constants.py` & `tja2fumen-0.4.0/src/tja2fumen/constants.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/converters.py` & `tja2fumen-0.4.0/src/tja2fumen/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,22 +50,24 @@
         currentGogo = False
         currentBarline = True
         currentDividend = 4
         currentDivisor = 4
         for measure in branch:
             # Split measure into submeasure
             measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo, 'barline': currentBarline,
-                           'subdivisions': len(measure['data']), 'pos_start': 0, 'pos_end': 0,
+                           'subdivisions': len(measure['data']), 'pos_start': 0, 'pos_end': 0, 'delay': 0,
                            'branchStart': None, 'time_sig': [currentDividend, currentDivisor], 'data': []}
             for data in measure['combined']:
                 # Handle note data
                 if data['type'] == 'note':
                     measure_cur['data'].append(data)
 
                 # Handle commands that can only be placed between measures (i.e. no mid-measure variations)
+                elif data['type'] == 'delay':
+                    measure_cur['delay'] = data['value'] * 1000  # ms -> s
                 elif data['type'] == 'branchStart':
                     measure_cur['branchStart'] = data['value']
                 elif data['type'] == 'barline':
                     currentBarline = bool(int(data['value']))
                     measure_cur['barline'] = currentBarline
                 elif data['type'] == 'measure':
                     matchMeasure = re.match(r"(\d+)/(\d+)", data['value'])
@@ -91,16 +93,16 @@
                     if data['pos'] == 0:
                         measure_cur[data['type']] = new_val
                     # - Case 2: Command occurs mid-measure, so start a new sub-measure
                     else:
                         measure_cur['pos_end'] = data['pos']
                         branchesCorrected[branchName].append(measure_cur)
                         measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo,
-                                       'barline': currentBarline,
-                                       'subdivisions': len(measure['data']), 'pos_start': data['pos'], 'pos_end': 0,
+                                       'barline': currentBarline, 'subdivisions': len(measure['data']),
+                                       'pos_start': data['pos'], 'pos_end': 0, 'delay': 0,
                                        'branchStart': None, 'time_sig': [currentDividend, currentDivisor], 'data': []}
 
                 else:
                     print(f"Unexpected event type: {data['type']}")
 
             measure_cur['pos_end'] = len(measure['data'])
             branchesCorrected[branchName].append(measure_cur)
@@ -170,15 +172,15 @@
             else:
                 # Compute the 1st measure's offset by subtracting the 2nd measure's duration from the tjaOffset
                 if idx_m == 1:
                     tjaOffset = float(tja['metadata']['offset']) * 1000 * -1
                     tjaConverted['measures'][idx_m-1]['fumenOffset'] = tjaOffset - measureDurationPrev
                 # Use the previous measure's offset plus the previous duration to compute the current measure's offset
                 measureOffsetPrev = tjaConverted['measures'][idx_m-1]['fumenOffset']
-                measureFumen['fumenOffset'] = measureOffsetPrev + measureDurationPrev
+                measureFumen['fumenOffset'] = measureOffsetPrev + measureDurationPrev + measureTJA['delay']
             measureDurationPrev = measureDuration
 
             # Best guess at what 'barline' status means for each measure:
             # - 'True' means the measure lands on a barline (i.e. most measures), and thus barline should be shown
             # - 'False' means that the measure doesn't land on a barline, and thus barline should be hidden.
             #   For example:
             #     1. Measures where #BARLINEOFF has been set
```

### Comparing `tja2fumen-0.3.0/src/tja2fumen/parsers.py` & `tja2fumen-0.4.0/src/tja2fumen/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,29 +124,31 @@
                 idx_m += 1
             # Otherwise, keep adding notes to the current measure ('idx_m')
             else:
                 for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
                     branches[branch][idx_m]['data'] += notes
 
         # 2. Parse measure commands that produce an "event"
-        elif line['name'] in ['GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF',
+        elif line['name'] in ['GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF', 'DELAY',
                               'SCROLL', 'BPMCHANGE', 'MEASURE', 'BRANCHSTART']:
             # Get position of the event
             for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
                 pos = len(branches[branch][idx_m]['data'])
 
             # Parse event type
             if line['name'] == 'GOGOSTART':
                 currentEvent = {"name": 'gogo', "position": pos, "value": '1'}
             elif line['name'] == 'GOGOEND':
                 currentEvent = {"name": 'gogo', "position": pos, "value": '0'}
             elif line['name'] == 'BARLINEON':
                 currentEvent = {"name": 'barline', "position": pos, "value": '1'}
             elif line['name'] == 'BARLINEOFF':
                 currentEvent = {"name": 'barline', "position": pos, "value": '0'}
+            elif line['name'] == 'DELAY':
+                currentEvent = {"name": 'delay', "position": pos, "value": float(line['value'])}
             elif line['name'] == 'SCROLL':
                 currentEvent = {"name": 'scroll', "position": pos, "value": float(line['value'])}
             elif line['name'] == 'BPMCHANGE':
                 currentEvent = {"name": 'bpm', "position": pos, "value": float(line['value'])}
             elif line['name'] == 'MEASURE':
                 currentEvent = {"name": 'measure', "position": pos, "value": line['value']}
             elif line["name"] == 'BRANCHSTART':
@@ -191,16 +193,14 @@
                 pass
             elif line['name'] == 'NEXTSONG':
                 pass
 
             # Not implemented commands
             elif line['name'] == 'SECTION':
                 pass  # This seems to be inconsequential, but I'm not 100% sure. Need to test more branching fumens.
-            elif line['name'] == 'DELAY':
-                raise NotImplementedError
             else:
                 raise NotImplementedError
 
     # Delete the last measure in the branch if no notes or events were added to it (due to preallocating empty measures)
     for branch in branches.values():
         if not branch[-1]['data'] and not branch[-1]['events']:
             del branch[-1]
```

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv` & `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/utils.py` & `tja2fumen-0.4.0/src/tja2fumen/utils.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen/writers.py` & `tja2fumen-0.4.0/src/tja2fumen/writers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.3.0/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.4.0/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.3.0/src/tja2fumen.egg-info/SOURCES.txt` & `tja2fumen-0.4.0/src/tja2fumen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

