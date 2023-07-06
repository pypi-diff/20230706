# Comparing `tmp/infotools-0.9.1.tar.gz` & `tmp/infotools-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infotools-0.9.1.tar", last modified: Tue Feb 28 22:38:47 2023, max compression
+gzip compressed data, was "infotools-0.9.2.tar", last modified: Thu Jul  6 02:50:58 2023, max compression
```

## Comparing `infotools-0.9.1.tar` & `infotools-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)        0 2023-02-28 22:38:47.673510 infotools-0.9.1/
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     1068 2021-04-01 22:25:21.000000 infotools-0.9.1/LICENSE
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)      430 2023-02-28 22:38:47.673671 infotools-0.9.1/PKG-INFO
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     2037 2021-04-01 22:25:21.000000 infotools-0.9.1/README.md
-drwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)        0 2023-02-28 22:38:47.666242 infotools-0.9.1/infotools/
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)       90 2022-02-01 04:04:24.000000 infotools-0.9.1/infotools/__init__.py
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)      887 2021-07-10 15:15:19.000000 infotools-0.9.1/infotools/datatools.py
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     4525 2023-02-28 22:26:37.000000 infotools-0.9.1/infotools/filetools.py
-drwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)        0 2023-02-28 22:38:47.670416 infotools-0.9.1/infotools/numbertools/
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)      120 2021-07-10 15:15:19.000000 infotools-0.9.1/infotools/numbertools/__init__.py
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     2834 2021-07-10 15:15:19.000000 infotools-0.9.1/infotools/numbertools/_numbertools.py
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     4517 2021-06-01 04:16:55.000000 infotools-0.9.1/infotools/numbertools/_scale.py
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     1399 2022-10-04 16:36:17.000000 infotools-0.9.1/infotools/plottools.py
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     2365 2022-05-05 19:35:44.000000 infotools-0.9.1/infotools/tabletools.py
-drwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)        0 2023-02-28 22:38:47.672984 infotools-0.9.1/infotools/timetools/
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)       92 2021-04-01 22:25:25.000000 infotools-0.9.1/infotools/timetools/__init__.py
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     9521 2022-08-22 19:34:03.000000 infotools-0.9.1/infotools/timetools/_duration.py
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     4454 2021-07-10 15:15:19.000000 infotools-0.9.1/infotools/timetools/_timer.py
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)     7649 2023-02-28 22:13:57.000000 infotools-0.9.1/infotools/timetools/_timestamp.py
-drwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)        0 2023-02-28 22:38:47.668566 infotools-0.9.1/infotools.egg-info/
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)      430 2023-02-28 22:38:47.000000 infotools-0.9.1/infotools.egg-info/PKG-INFO
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)      548 2023-02-28 22:38:47.000000 infotools-0.9.1/infotools.egg-info/SOURCES.txt
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)        1 2023-02-28 22:38:47.000000 infotools-0.9.1/infotools.egg-info/dependency_links.txt
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)       46 2023-02-28 22:38:47.000000 infotools-0.9.1/infotools.egg-info/requires.txt
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)       10 2023-02-28 22:38:47.000000 infotools-0.9.1/infotools.egg-info/top_level.txt
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)      132 2023-02-28 22:38:47.674104 infotools-0.9.1/setup.cfg
--rwxrwxrwx   0 proginoskes  (1000) proginoskes  (1000)      819 2023-02-28 22:16:07.000000 infotools-0.9.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 02:50:58.401127 infotools-0.9.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2023-03-20 21:01:30.000000 infotools-0.9.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      402 2023-07-06 02:50:58.401215 infotools-0.9.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2037 2023-03-20 21:01:30.000000 infotools-0.9.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 02:50:58.396700 infotools-0.9.2/infotools/
+-rwxrwxrwx   0 root         (0) root         (0)       90 2023-03-20 21:01:30.000000 infotools-0.9.2/infotools/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      887 2023-03-20 21:01:30.000000 infotools-0.9.2/infotools/datatools.py
+-rwxrwxrwx   0 root         (0) root         (0)     5489 2023-04-27 16:45:31.000000 infotools-0.9.2/infotools/filetools.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 02:50:58.399116 infotools-0.9.2/infotools/numbertools/
+-rwxrwxrwx   0 root         (0) root         (0)      120 2023-03-20 21:01:30.000000 infotools-0.9.2/infotools/numbertools/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5332 2023-07-05 18:57:57.000000 infotools-0.9.2/infotools/numbertools/_numbertools.py
+-rwxrwxrwx   0 root         (0) root         (0)     4517 2023-03-20 21:01:30.000000 infotools-0.9.2/infotools/numbertools/_scale.py
+-rwxrwxrwx   0 root         (0) root         (0)     2094 2023-04-17 17:07:31.000000 infotools-0.9.2/infotools/plottools.py
+-rwxrwxrwx   0 root         (0) root         (0)     2366 2023-07-06 01:55:28.000000 infotools-0.9.2/infotools/tabletools.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 02:50:58.400756 infotools-0.9.2/infotools/timetools/
+-rwxrwxrwx   0 root         (0) root         (0)       92 2023-03-20 21:01:30.000000 infotools-0.9.2/infotools/timetools/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9521 2023-03-20 21:01:30.000000 infotools-0.9.2/infotools/timetools/_duration.py
+-rwxrwxrwx   0 root         (0) root         (0)     4454 2023-03-20 21:01:30.000000 infotools-0.9.2/infotools/timetools/_timer.py
+-rwxrwxrwx   0 root         (0) root         (0)     7578 2023-04-01 18:30:36.000000 infotools-0.9.2/infotools/timetools/_timestamp.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 02:50:58.398131 infotools-0.9.2/infotools.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      402 2023-07-06 02:50:58.000000 infotools-0.9.2/infotools.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      548 2023-07-06 02:50:58.000000 infotools-0.9.2/infotools.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-06 02:50:58.000000 infotools-0.9.2/infotools.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       46 2023-07-06 02:50:58.000000 infotools-0.9.2/infotools.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2023-07-06 02:50:58.000000 infotools-0.9.2/infotools.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      132 2023-07-06 02:50:58.401594 infotools-0.9.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      819 2023-07-06 02:41:45.000000 infotools-0.9.2/setup.py
```

### Comparing `infotools-0.9.1/LICENSE` & `infotools-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `infotools-0.9.1/README.md` & `infotools-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `infotools-0.9.1/infotools/datatools.py` & `infotools-0.9.2/infotools/datatools.py`

 * *Files identical despite different names*

### Comparing `infotools-0.9.1/infotools/filetools.py` & `infotools-0.9.2/infotools/filetools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import hashlib
 import mimetypes
 import os
 from pathlib import Path
-from typing import Tuple, Union
-import datetime
+from typing import Tuple, Union, Set
+import string
 import re
+
 mimetypes.add_type('audio/aac', '.aac')
 
 from loguru import logger
 
 Pathlike = Union[str, Path]
-def get_type_name(t)->str:
+
+
+def get_type_name(t) -> str:
 	pattern = "[\w]+[.][\w]+"
 	match = re.search(pattern, str(t))
 	if match:
 		match = match.group(0)
 	return match
 
+
 def get_mimetype(filename: Pathlike) -> Tuple[str, str]:
 	""" Wrapper to get the mimetype of a given file. Returns `None` if the mimetype cannot be determined.
 		Returns
 		-------
 		mimetype, filetype
 			Ex. ('text', 'plain'), ('video', 'mp4')
 
@@ -102,17 +106,39 @@
 		while True:
 			buf = f.read(blocksize)
 			if not buf: break
 			m.update(buf)
 	return m.hexdigest()
 
 
-def sanitize_path(path: Path) -> Path:
-	""" Removes illegal characters from a path. """
-	pass
+def get_allowed_characters() -> Set[str]:
+	allowed_characters = set(string.ascii_letters + string.digits)
+	allowed_characters = allowed_characters | {'.', ',', '&', '(', ')', '+', '-', '[', ']', '_'}
+	to_keep = {'Ñ', 'Ö', 'ß', 'á', 'ã', 'ä', 'ç', 'è', 'é', 'ê', 'ñ', 'ó', 'ö', 'ü', 'ę', 'Μ', 'Φ', 'К', 'М', 'Т', 'а', 'в', 'е', 'и', 'к', 'н', 'р',
+		'т', 'у', 'х', 'я', '/', ' '}
+	allowed_characters = allowed_characters | to_keep
+
+	return allowed_characters
+
+
+def sanitize_text(text: str, replacement: str = "") -> str:
+	allowed_characteres = get_allowed_characters()
+	characters = set(text)
+	characters_to_remove = characters - allowed_characteres
+	characters_to_replace = {' -': "", '/': "-", '&amp': "&"}
+	for char in characters_to_remove:
+		text = text.replace(char, replacement)
+
+	for character_to_replace, replacement in characters_to_replace.items():
+		text = text.replace(character_to_replace, replacement)
+
+	# Remove all extra whitespace
+	# pattern = "[\s]+"
+	# text = re.sub(pattern, " ", text)
+	return text
 
 
 def to_json(obj, filename: Path = None) -> str:
 	""" Tries to convert datatypes to json-usable versions. Ex numpy.ndarray -> list(). """
 	import json
 	import numpy
 	import datetime
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `infotools-0.9.1/infotools/numbertools/_scale.py` & `infotools-0.9.2/infotools/numbertools/_scale.py`

 * *Files identical despite different names*

### Comparing `infotools-0.9.1/infotools/plottools.py` & `infotools-0.9.2/infotools/plottools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,44 @@
 from typing import *
 
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 from infotools import numbertools
 import random
 
-def add_legend(ax: plt.Axes, colormap: Dict[str, str]) -> plt.Axes:
+class Palette:
+	def __init__(self, colormap: str = "Blues", step:int = 10):
+		self.breakpoints = [i * step for i in range(10)]
+		self.colors = seaborn.color_palette(colormap, len(self.breakpoints) + 1)
+
+		self.colormap_bins = {cutoff: color for cutoff, color in zip(self.breakpoints, self.colors)}
+
+	def get_color(self, value: float) -> str:
+		for cutoff, color in self.colormap_bins.items():
+			if value <= cutoff:
+				break
+		else:
+			color = '#FF0000'
+		return color
+
+	def add_legend(self, ax: plt.Axes, colormap: Dict[str, str] = None, **kwargs) -> plt.Axes:
+		if colormap is None:
+			colormap = self.colormap_bins
+		ax = add_legend(ax, colormap,**kwargs)
+		return ax
+
+
+
+def add_legend(ax: plt.Axes, colormap: Dict[str, str], **kwargs) -> plt.Axes:
 	patches = list()
 	for label, color in sorted(colormap.items(), key = lambda s: (len(s[0].split('|')), s[0])):
 		patch = mpatches.Patch(color = color, label = label)
 		patches.append(patch)
 
-	ax.legend(handles = patches)
+	ax.legend(handles = patches, **kwargs)
 	return ax
 
 
 def get_random_color(lower: int = 50, upper: int = 250) -> str:
 	red = random.randint(lower, upper)
 	green = random.randint(lower, upper)
 	blue = random.randint(lower, upper)
```

### Comparing `infotools-0.9.1/infotools/tabletools.py` & `infotools-0.9.2/infotools/tabletools.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,20 +42,21 @@
 	filename: str, pathlib.Path
 		The output file.
 
 	Returns
 	-------
 	Path: The output filename
 	"""
-	writer = pandas.ExcelWriter(str(filename))
+	#writer = pandas.ExcelWriter(str(filename))
 	# python 3.5 or 3.6 made all dicts ordered by default, so the sheets will be ordered in the same order they were defined in `tables`
-	for sheet_label, df in tables.items():
-		if df is None: continue
-		df.to_excel(writer, sheet_label, index = include_index)
-	writer.save()  # otherwise color_table_cells will not be able to load the file
+	with pandas.ExcelWriter(str(filename)) as writer:
+		for sheet_label, table in tables.items():
+			if table is None:
+				continue
+			table.to_excel(writer, sheet_name = sheet_label, index = include_index)
 
 	# Need to use the xlsx library to change some features of the spreadsheet.
 
 	return filename
 
 def to_csv(table:pandas.DataFrame, filename:Path, precision:int = 2):
 	"""
```

### Comparing `infotools-0.9.1/infotools/timetools/_duration.py` & `infotools-0.9.2/infotools/timetools/_duration.py`

 * *Files identical despite different names*

### Comparing `infotools-0.9.1/infotools/timetools/_timer.py` & `infotools-0.9.2/infotools/timetools/_timer.py`

 * *Files identical despite different names*

### Comparing `infotools-0.9.1/infotools/timetools/_timestamp.py` & `infotools-0.9.2/infotools/timetools/_timestamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,20 +200,18 @@
 			}
 			return cls.from_dict(**data)
 
 	@classmethod
 	def from_string(cls, value: str) -> 'Timestamp':
 
 		try:
-			logger.debug(f"parsing...")
 			obj = pendulum.parse(value)
 
 		except ValueError:
 			try:
-				logger.debug(f"From American Date")
 				obj = cls.from_american_date(value)
 			except ValueError:
 				obj = cls.from_verbal_date(value)
 
 		return cls.from_object(obj)
 
 	@classmethod
```

### Comparing `infotools-0.9.1/infotools.egg-info/SOURCES.txt` & `infotools-0.9.2/infotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infotools-0.9.1/setup.py` & `infotools-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 if infotools.DEBUG:
 	message = f"The module is still in debug mode!"
 	raise ValueError(message)
 """
 setup(
 	name = 'infotools',
-	version = '0.9.1',
+	version = '0.9.2',
 	packages = ['infotools', 'infotools.timetools', 'infotools.numbertools'],
 	url = 'https://github.com/Kokitis/infotools',
 	license = 'MIT',
 	author = 'proginoskes',
 	author_email = 'chrisdeitrick1@gmail.com',
 	description = 'A collection of tools to make common tasks simpler.',
 	classifiers = [
```

