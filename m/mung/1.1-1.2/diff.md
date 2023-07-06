# Comparing `tmp/mung-1.1.tar.gz` & `tmp/mung-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mung-1.1.tar", last modified: Mon Aug 12 15:11:10 2019, max compression
+gzip compressed data, was "mung-1.2.tar", last modified: Thu Jul  6 17:37:32 2023, max compression
```

## Comparing `mung-1.1.tar` & `mung-1.2.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxrwx   0        0        0        0 2019-08-12 15:11:10.000000 mung-1.1/
--rw-rw-rw-   0        0        0     3020 2019-08-12 15:11:10.000000 mung-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1588 2019-08-12 08:21:43.000000 mung-1.1/README.md
-drwxrwxrwx   0        0        0        0 2019-08-12 15:11:10.000000 mung-1.1/mung/
--rw-rw-rw-   0        0        0       21 2019-08-12 15:09:19.000000 mung-1.1/mung/__init__.py
--rw-rw-rw-   0        0        0     6504 2019-08-12 08:21:43.000000 mung-1.1/mung/constants.py
--rw-rw-rw-   0        0        0     7308 2019-08-08 15:24:11.000000 mung-1.1/mung/dataset.py
--rw-rw-rw-   0        0        0    33554 2019-08-08 15:24:11.000000 mung-1.1/mung/grammar.py
--rw-rw-rw-   0        0        0    41578 2019-08-08 15:24:11.000000 mung-1.1/mung/graph.py
--rw-rw-rw-   0        0        0    18629 2019-08-12 08:21:43.000000 mung-1.1/mung/io.py
--rw-rw-rw-   0        0        0    11216 2019-08-12 08:21:43.000000 mung-1.1/mung/mungmatcher.py
--rw-rw-rw-   0        0        0    54024 2019-08-12 15:09:19.000000 mung-1.1/mung/node.py
--rw-rw-rw-   0        0        0     4512 2019-08-08 15:24:11.000000 mung-1.1/mung/node_class.py
--rw-rw-rw-   0        0        0    37780 2019-08-08 15:24:11.000000 mung-1.1/mung/stafflines.py
--rw-rw-rw-   0        0        0     1774 2019-08-08 15:24:11.000000 mung-1.1/mung/utils.py
-drwxrwxrwx   0        0        0        0 2019-08-12 15:11:10.000000 mung-1.1/mung.egg-info/
--rw-rw-rw-   0        0        0     3020 2019-08-12 15:11:10.000000 mung-1.1/mung.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2019-08-12 15:11:10.000000 mung-1.1/mung.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-08-12 15:11:10.000000 mung-1.1/mung.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2019-08-12 15:11:10.000000 mung-1.1/mung.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2019-08-12 15:11:10.000000 mung-1.1/mung.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2019-08-12 15:11:10.000000 mung-1.1/mung2midi/
--rw-rw-rw-   0        0        0        0 2019-08-08 15:24:11.000000 mung-1.1/mung2midi/__init__.py
--rw-rw-rw-   0        0        0   109677 2019-08-12 08:21:43.000000 mung-1.1/mung2midi/inference.py
-drwxrwxrwx   0        0        0        0 2019-08-12 15:11:10.000000 mung-1.1/scripts/
--rw-rw-rw-   0        0        0    15639 2019-08-12 08:21:43.000000 mung-1.1/scripts/add_staff_relationships.py
--rw-rw-rw-   0        0        0    19464 2019-08-12 08:21:43.000000 mung-1.1/scripts/add_staffline_symbols.py
--rw-rw-rw-   0        0        0    18859 2019-08-12 08:21:43.000000 mung-1.1/scripts/analyze_agreement.py
--rw-rw-rw-   0        0        0     6404 2019-08-12 08:21:43.000000 mung-1.1/scripts/analyze_annotations.py
--rw-rw-rw-   0        0        0    16654 2019-08-12 08:21:43.000000 mung-1.1/scripts/analyze_tracking_log.py
--rw-rw-rw-   0        0        0    32669 2019-08-12 08:21:43.000000 mung-1.1/scripts/baseline_process_symbols.py
--rw-rw-rw-   0        0        0     4401 2019-08-08 15:24:11.000000 mung-1.1/scripts/get_images_from_muscima.py
--rw-rw-rw-   0        0        0     4800 2019-08-12 08:21:43.000000 mung-1.1/scripts/infer_pitches.py
--rw-rw-rw-   0        0        0     3149 2019-08-12 08:21:43.000000 mung-1.1/scripts/strip_staffline_symbols.py
--rw-rw-rw-   0        0        0       86 2019-08-12 15:11:10.000000 mung-1.1/setup.cfg
--rw-rw-rw-   0        0        0     2840 2019-08-12 08:21:43.000000 mung-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2019-08-12 15:11:10.000000 mung-1.1/test/
--rw-rw-rw-   0        0        0      816 2019-08-08 15:24:11.000000 mung-1.1/test/test_grammar.py
--rw-rw-rw-   0        0        0     2593 2019-08-08 15:24:11.000000 mung-1.1/test/test_node.py
--rw-rw-rw-   0        0        0      982 2019-08-08 15:24:11.000000 mung-1.1/test/test_node_class.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-06 17:37:32.539737 mung-1.2/
+-rw-r--r--   0 alex       (501) staff       (20)     1140 2023-07-04 20:47:07.000000 mung-1.2/LICENSE.txt
+-rw-r--r--   0 alex       (501) staff       (20)     3776 2023-07-06 17:37:32.539936 mung-1.2/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2563 2023-07-04 20:53:17.000000 mung-1.2/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-06 17:37:32.522493 mung-1.2/mung/
+-rw-r--r--   0 alex       (501) staff       (20)       20 2023-07-04 20:48:40.000000 mung-1.2/mung/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     6910 2020-05-29 09:41:08.000000 mung-1.2/mung/constants.py
+-rw-r--r--   0 alex       (501) staff       (20)     7127 2020-04-27 08:27:06.000000 mung-1.2/mung/dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)    32825 2020-05-29 10:18:18.000000 mung-1.2/mung/grammar.py
+-rw-r--r--   0 alex       (501) staff       (20)    40487 2020-05-29 09:20:16.000000 mung-1.2/mung/graph.py
+-rw-r--r--   0 alex       (501) staff       (20)    18737 2020-06-29 12:20:06.000000 mung-1.2/mung/io.py
+-rw-r--r--   0 alex       (501) staff       (20)    10975 2020-05-14 14:59:04.000000 mung-1.2/mung/mungmatcher.py
+-rw-r--r--   0 alex       (501) staff       (20)    52815 2021-04-28 09:12:01.000000 mung-1.2/mung/node.py
+-rw-r--r--   0 alex       (501) staff       (20)     4380 2020-04-27 08:27:06.000000 mung-1.2/mung/node_class.py
+-rw-r--r--   0 alex       (501) staff       (20)    36731 2020-05-29 09:20:16.000000 mung-1.2/mung/stafflines.py
+-rw-r--r--   0 alex       (501) staff       (20)     1654 2020-05-14 14:59:04.000000 mung-1.2/mung/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-06 17:37:32.525403 mung-1.2/mung.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     3776 2023-07-06 17:37:32.000000 mung-1.2/mung.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      782 2023-07-06 17:37:32.000000 mung-1.2/mung.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-06 17:37:32.000000 mung-1.2/mung.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       24 2023-07-06 17:37:32.000000 mung-1.2/mung.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       15 2023-07-06 17:37:32.000000 mung-1.2/mung.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-06 17:37:32.528275 mung-1.2/mung2midi/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2020-04-27 08:27:06.000000 mung-1.2/mung2midi/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)   101911 2020-05-29 10:18:18.000000 mung-1.2/mung2midi/inference.py
+-rw-r--r--   0 alex       (501) staff       (20)    10310 2020-06-29 12:20:06.000000 mung-1.2/mung2midi/run_inference.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-06 17:37:32.536542 mung-1.2/scripts/
+-rwxr-xr-x   0 alex       (501) staff       (20)    15240 2020-05-29 10:18:01.000000 mung-1.2/scripts/add_staff_relationships.py
+-rwxr-xr-x   0 alex       (501) staff       (20)    18952 2020-05-29 09:20:16.000000 mung-1.2/scripts/add_staffline_symbols.py
+-rwxr-xr-x   0 alex       (501) staff       (20)    18419 2020-04-27 08:27:06.000000 mung-1.2/scripts/analyze_agreement.py
+-rwxr-xr-x   0 alex       (501) staff       (20)     6235 2020-04-27 08:27:06.000000 mung-1.2/scripts/analyze_annotations.py
+-rwxr-xr-x   0 alex       (501) staff       (20)    16212 2020-04-27 08:27:06.000000 mung-1.2/scripts/analyze_tracking_log.py
+-rw-r--r--   0 alex       (501) staff       (20)    31762 2020-06-03 09:45:15.000000 mung-1.2/scripts/baseline_process_symbols.py
+-rwxr-xr-x   0 alex       (501) staff       (20)     4286 2020-04-27 08:27:06.000000 mung-1.2/scripts/get_images_from_muscima.py
+-rwxr-xr-x   0 alex       (501) staff       (20)     4655 2020-05-15 09:30:01.000000 mung-1.2/scripts/infer_pitches.py
+-rwxr-xr-x   0 alex       (501) staff       (20)     3064 2020-05-29 09:20:16.000000 mung-1.2/scripts/strip_staffline_symbols.py
+-rw-r--r--   0 alex       (501) staff       (20)       79 2023-07-06 17:37:32.540656 mung-1.2/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     2765 2023-07-04 20:54:14.000000 mung-1.2/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-06 17:37:32.539135 mung-1.2/test/
+-rw-r--r--   0 alex       (501) staff       (20)      795 2020-04-27 08:27:06.000000 mung-1.2/test/test_grammar.py
+-rw-r--r--   0 alex       (501) staff       (20)     2537 2020-06-03 09:15:23.000000 mung-1.2/test/test_node.py
+-rw-r--r--   0 alex       (501) staff       (20)     1108 2020-06-03 09:17:06.000000 mung-1.2/test/test_node_class.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mung-1.1/PKG-INFO` & `mung-1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,47 @@
-Metadata-Version: 2.1
-Name: mung
-Version: 1.1
-Summary: Tools for the Music Notation Graph representation of music notation, used primarily for optical music recognition.
-Home-page: https://mung.readthedocs.io
-Author: Jan Hajič jr. and Alexander Pacha
-Author-email: alexander.pacha@tuwien.ac.at
-License: MIT Software License
-Description: # MuNG
-        
-        The ``mung`` (**Mu**sic **N**otation **G**raph) package implements a graph representation
-         of music notation that is especially amenable to Optical Music Recognition (OMR).
-        It was used for instance in the [MUSCIMA++](https://ufal.mff.cuni.cz/muscima) dataset of music notation.
-        
-        [![Build Status](https://travis-ci.org/OMR-Research/mung.svg?branch=master)](https://travis-ci.org/OMR-Research/mung)
-        [![PyPI version](https://badge.fury.io/py/mung.svg)](https://badge.fury.io/py/mung)
-        [![Documentation Status](https://readthedocs.org/projects/mung/badge/?version=latest)](https://mung.readthedocs.io/en/latest/?badge=latest)
-        [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE.txt)
-        [![codecov](https://codecov.io/gh/OMR-Research/mung/branch/master/graph/badge.svg)](https://codecov.io/gh/OMR-Research/mung)
-        
-        Requires Python >= 3.6.
-        
-        
-        ## Getting started
-        
-        1. Install this package: ``pip install mung``
-        2. Download the [MUSCIMA++ dataset](https://github.com/OMR-Research/muscima-pp).
-        3. Run through the [tutorial](https://muscima.readthedocs.io/en/latest/Tutorial.html#tutorial).
-        
-        
-        
-        ## Dataset
-        The dataset itself is available for download
-        [here](https://github.com/OMR-Research/muscima-pp) and due to its derived nature, licensed differently:
-        
-        [![abc](https://img.shields.io/badge/Dataset_Version-2.0-brightgreen.svg)](https://github.com/OMR-Research/muscima-pp)
-        [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
-        
-        
-        
-        Changelog
-        =========
-        
-        This changelog does not refer to the older `muscima` package.
-        
-        
-        1.0
-        ---
-        
-        First public release of `mung` package, which is equivalent to the muscima-package, but updated 
-        to comply with the version 2.0 of the MUSCIMA++ dataset.
-        
-        
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 4 - Beta
-Classifier: Natural Language :: English
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
-Description-Content-Type: text/markdown
+# MuNG
+
+The ``mung`` (**Mu**sic **N**otation **G**raph) package implements a graph representation
+ of music notation that is especially amenable to Optical Music Recognition (OMR).
+It was used for instance in the [MUSCIMA++](https://ufal.mff.cuni.cz/muscima) dataset of music notation.
+
+[![Build Status](https://travis-ci.org/OMR-Research/mung.svg?branch=master)](https://travis-ci.org/OMR-Research/mung)
+[![PyPI version](https://badge.fury.io/py/mung.svg)](https://badge.fury.io/py/mung)
+[![Documentation Status](https://readthedocs.org/projects/mung/badge/?version=latest)](https://mung.readthedocs.io/en/latest/?badge=latest)
+[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE.txt)
+[![codecov](https://codecov.io/gh/OMR-Research/mung/branch/master/graph/badge.svg)](https://codecov.io/gh/OMR-Research/mung)
+
+Requires Python >= 3.6 and was tested with Python 3.11.
+
+
+## Getting started
+
+1. Install this package: ``pip install mung``
+2. Download the [MUSCIMA++ dataset](https://github.com/OMR-Research/muscima-pp).
+3. Run through the [tutorial](https://muscima.readthedocs.io/en/latest/Tutorial.html#tutorial).
+
+Fundamentally, the Music Notatation Graph is a very simple construct:
+
+![](doc/MuNG%20Class%20Diagram.png)
+
+It stores the primitives that can be detected by a [Music Object Detector](https://github.com/apacha/MusicObjectDetector-TF)
+as nodes and then store the relations between those nodes. But the devil is
+in the details. To better understand what kind of [relations are useful](https://archives.ismir.net/ismir2019/paper/000006.pdf) 
+and which kind of relations are stored for common western music notation, check out the
+[annotator instruction from MUSCIMarker](https://muscimarker.readthedocs.io/en/latest/instructions.html).
+
+
+
+## Dataset
+The dataset itself is available for download
+[here](https://github.com/OMR-Research/muscima-pp) and due to its derived nature, licensed differently:
+
+[![abc](https://img.shields.io/badge/Dataset_Version-2.0-brightgreen.svg)](https://github.com/OMR-Research/muscima-pp)
+[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
+
+
+### Introduction to MUSCIMA++ Video
+
+Watch Jan give a 30 minute introduction into this dataset on YouTube, which explains many design decisions and thoughts that directly affected the creation of the MuNG format:
+
+[![Introduction to MUSCIMA++](https://img.youtube.com/vi/SvBvcxdGoE8/0.jpg)](https://www.youtube.com/watch?v=SvBvcxdGoE8)
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mung-1.1/mung/constants.py` & `mung-1.2/mung/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,243 +1,278 @@
-"""This module implements constants that are used inside the pitch,
-duration and onset inference algorithm."""
-import operator
-
-
-class InferenceEngineConstants(object):
-    """This class stores the constants used for pitch inference."""
-
-    ON_STAFFLINE_RATIO_THRESHOLD = 0.2
-    '''Magic number for determining whether a notehead is *on* a leger
-    line, or *next* to a leger line: if the ratio between the smaller
-    and larger vertical difference of (top, bottom) vs. l.l. (top, bottom)
-    is smaller than this, it means the notehead is most probably *NOT*
-    on the l.l. and is next to it.'''
-
-    STAFFLINE_CLASS_NAME = 'staffLine'
-    STAFFSPACE_CLASS_NAME = 'staffSpace'
-    STAFF_CLASS_NAME = 'staff'
-    LEGER_LINE_CLASS_NAME = 'legerLine'
-
-    STAFF_CLASS_NAMES = [STAFFLINE_CLASS_NAME, STAFFSPACE_CLASS_NAME, STAFF_CLASS_NAME]
-    STAFFLINE_CLASS_NAMES = [STAFFLINE_CLASS_NAME, STAFFSPACE_CLASS_NAME]
-
-    STAFFLINE_LIKE_CLASS_NAMES = [STAFFLINE_CLASS_NAME, LEGER_LINE_CLASS_NAME]
-    TIE_CLASS_NAME = 'tie'
-
-    G_CLEF = 'gClef'
-    C_CLEF = 'cClef'
-    F_CLEF = 'fClef'
-
-    STAFF_RELATED_CLASS_NAMES = {
-        'staffGrouping',
-        'measureSeparator',
-        'keySignature',
-        'timeSignature',
-        G_CLEF,
-        C_CLEF,
-        F_CLEF
-    }
-
-    SYSTEM_LEVEL_CLASS_NAMES = {
-        'staff_grouping',
-        'measure_separator',
-    }
-
-    NOTEHEAD_CLASS_NAMES = {
-        'noteheadFull',
-        'noteheadHalf',
-        'noteheadWhole',
-        'noteheadFullSmall',
-        'noteheadHalfSmall',
-    }
-
-    NONGRACE_NOTEHEAD_CLASS_NAMES = {
-        'noteheadFull',
-        'noteheadHalf',
-        'noteheadWhole',
-    }
-
-    CLEF_CLASS_NAMES = {
-        G_CLEF,
-        C_CLEF,
-        F_CLEF
-    }
-
-    KEY_SIGNATURE_CLASS_NAMES = {
-        'keySignature',
-    }
-
-    MEASURE_SEPARATOR_CLASS_NAMES = {
-        'measureSeparator',
-    }
-
-    FLAGS_CLASS_NAMES = {
-        'flag8thUp',
-        'flag8thDown',
-        'flag16thUp',
-        'flag16thDown',
-        'flag32ndUp',
-        'flag32ndDown',
-        'flag64thUp',
-        'flag64thDown',
-    }
-
-    BEAM_CLASS_NAMES = {
-        'beam',
-    }
-
-    FLAGS_AND_BEAMS = set(list(FLAGS_CLASS_NAMES) + list(BEAM_CLASS_NAMES))
-
-    ACCIDENTAL_CLASS_NAMES = {
-        'accidentalSharp': 1,
-        'accidentalFlat': -1,
-        'accidentalNatural': 0,
-        'accidentalDoubleSharp': 2,
-        'accidentalDoubleFlat': -2,
-    }
-
-    MIDI_CODE_RESIDUES_FOR_PITCH_STEPS = {
-        0: 'C',
-        1: 'C#',
-        2: 'D',
-        3: 'Eb',
-        4: 'E',
-        5: 'F',
-        6: 'F#',
-        7: 'G',
-        8: 'Ab',
-        9: 'A',
-        10: 'Bb',
-        11: 'B',
-    }
-    '''Simplified pitch naming.'''
-
-    # The individual MIDI codes for for the unmodified steps.
-    _fs = list(range(5, 114, 12))
-    _cs = list(range(0, 121, 12))
-    _gs = list(range(7, 116, 12))
-    _ds = list(range(2, 110, 12))
-    _as = list(range(9, 118, 12))
-    _es = list(range(4, 112, 12))
-    _bs = list(range(11, 120, 12))
-
-    KEY_TABLE_SHARPS = {
-        0: {},
-        1: {i: 1 for i in _fs},
-        2: {i: 1 for i in _fs + _cs},
-        3: {i: 1 for i in _fs + _cs + _gs},
-        4: {i: 1 for i in _fs + _cs + _gs + _ds},
-        5: {i: 1 for i in _fs + _cs + _gs + _ds + _as},
-        6: {i: 1 for i in _fs + _cs + _gs + _ds + _as + _es},
-        7: {i: 1 for i in _fs + _cs + _gs + _ds + _as + _es + _bs},
-    }
-
-    KEY_TABLE_FLATS = {
-        0: {},
-        1: {i: -1 for i in _bs},
-        2: {i: -1 for i in _bs + _es},
-        3: {i: -1 for i in _bs + _es + _as},
-        4: {i: -1 for i in _bs + _es + _as + _ds},
-        5: {i: -1 for i in _bs + _es + _as + _ds + _gs},
-        6: {i: -1 for i in _bs + _es + _as + _ds + _gs + _cs},
-        7: {i: -1 for i in _bs + _es + _as + _ds + _gs + _cs + _fs},
-    }
-
-    # FROM clef --> TO clef. Imagine this on inline accidental delta
-    CLEF_CHANGE_DELTA = {
-        G_CLEF: {
-            G_CLEF: 0,
-            C_CLEF: 6,
-            F_CLEF: 12,
-        },
-        C_CLEF: {
-            G_CLEF: -6,
-            C_CLEF: 0,
-            F_CLEF: 6,
-        },
-        F_CLEF: {
-            G_CLEF: -12,
-            C_CLEF: -6,
-            F_CLEF: 0,
-        }
-    }
-
-    PITCH_STEPS = ['C', 'D', 'E', 'F', 'G', 'A', 'B',
-                   'C', 'D', 'E', 'F', 'G', 'A', 'B']
-    # Wrap around twice for easier indexing.
-
-    ACCIDENTAL_CODES = {'accidentalSharp': '#', 'accidentalFlat': 'b',
-                        'accidentalDoubleSharp': 'x', 'accidentalDoubleFlat': 'bb'}
-
-    REST_CLASS_NAMES = {
-        'restWhole',
-        'restHalf',
-        'restQuarter',
-        'rest8th',
-        'rest16th',
-        'rest32nd',
-        'rest64th',
-        'multiMeasureRest',
-    }
-
-    MEAUSURE_LASTING_CLASS_NAMES = {
-        'restWhole',
-        'multiMeasureRest',
-        'repeat1Bar',
-    }
-
-    TIME_SIGNATURES = {
-        'timeSignature',
-    }
-
-    TIME_SIGNATURE_MEMBERS = {
-        'timeSigCommon',
-        'timeSigCutCommon',
-        'numeral0',
-        'numeral1',
-        'numeral2',
-        'numeral3',
-        'numeral4',
-        'numeral5',
-        'numeral6',
-        'numeral7',
-        'numeral8',
-        'numeral9',
-    }
-
-    NUMERALS = {
-        'numeral0',
-        'numeral1',
-        'numeral2',
-        'numeral3',
-        'numeral4',
-        'numeral5',
-        'numeral6',
-        'numeral7',
-        'numeral8',
-        'numeral9',
-    }
-
-    @property
-    def classes_affecting_onsets(self):
-        """Returns a list of Node class names for objects
-        that affect onsets. Assumes notehead and rest durations
-        have already been given."""
-        output = set()
-        output.update(self.NONGRACE_NOTEHEAD_CLASS_NAMES)
-        output.update(self.REST_CLASS_NAMES)
-        output.update(self.MEASURE_SEPARATOR_CLASS_NAMES)
-        output.update(self.TIME_SIGNATURES)
-        output.add('repeat1Bar')
-        return output
-
-    @property
-    def classes_bearing_duration(self):
-        """Returns the list of classes that actually bear duration,
-        i.e. contribute to onsets of their descendants in the precedence
-        graph."""
-        output = set()
-        output.update(self.NONGRACE_NOTEHEAD_CLASS_NAMES)
-        output.update(self.REST_CLASS_NAMES)
-        return output
-
+"""This module implements constants that are used inside the pitch,
+duration and onset inference algorithm."""
+import operator
+
+
+class InferenceEngineConstants(object):
+    """This class stores the constants used for pitch inference."""
+
+    ON_STAFFLINE_RATIO_THRESHOLD = 0.2
+    '''Magic number for determining whether a notehead is *on* a leger
+    line, or *next* to a leger line: if the ratio between the smaller
+    and larger vertical difference of (top, bottom) vs. l.l. (top, bottom)
+    is smaller than this, it means the notehead is most probably *NOT*
+    on the l.l. and is next to it.'''
+
+    STAFFLINE = 'staffLine'
+    STAFFSPACE = 'staffSpace'
+    STAFF = 'staff'
+    LEGER_LINE = 'legerLine'
+    STEM = 'stem'
+
+    STAFF_CLASSES = [STAFFLINE, STAFFSPACE, STAFF]
+    STAFFLINE_CLASS_NAMES = [STAFFLINE, STAFFSPACE]
+
+    STAFFLINE_LIKE_CLASS_NAMES = [STAFFLINE, LEGER_LINE]
+    TIE_CLASS_NAME = 'tie'
+
+    G_CLEF = 'gClef'
+    C_CLEF = 'cClef'
+    F_CLEF = 'fClef'
+
+    STAFF_RELATED_CLASS_NAMES = {
+        'staffGrouping',
+        'measureSeparator',
+        'keySignature',
+        'timeSignature',
+        G_CLEF,
+        C_CLEF,
+        F_CLEF
+    }
+
+    SYSTEM_LEVEL_CLASS_NAMES = {
+        'staffGrouping',
+        'measureSeparator',
+    }
+
+    NOTEHEAD_CLASS_NAMES = {
+        'noteheadFull',
+        'noteheadHalf',
+        'noteheadWhole',
+        'noteheadFullSmall',
+        'noteheadHalfSmall',
+    }
+
+    NOTEHEAD_FULL = "noteheadFull"
+
+    NOTEHEAD_HALF = "noteheadHalf"
+
+    NOTEHEAD_WHOLE = "noteheadWhole"
+
+    NOTEHEADS_EMPTY = {
+        NOTEHEAD_HALF,
+        NOTEHEAD_WHOLE
+    }
+
+    GRACE_NOTEHEAD_CLASS_NAMES = {
+        'noteheadFullSmall',
+        'noteheadHalfSmall',
+    }
+
+    NONGRACE_NOTEHEAD_CLASS_NAMES = {
+        'noteheadFull',
+        'noteheadHalf',
+        'noteheadWhole',
+    }
+
+    REST_WHOLE = 'restWhole'
+    REST_HALF = 'restHalf'
+    REST_QUARTER = 'restQuarter'
+    REST_8TH = 'rest8th'
+    REST_16TH = 'rest16th'
+    REST_32ND = 'rest32nd'
+    REST_64TH = 'rest64th'
+    REPEAT_ONE_BAR = 'repeat1Bar'
+    MULTI_MEASURE_REST = 'multiMeasureRest'
+    AUGMENTATION_DOT = 'augmentationDot'
+
+    TUPLE = 'tuple'
+
+    CLEF_CLASS_NAMES = {
+        G_CLEF,
+        C_CLEF,
+        F_CLEF
+    }
+
+    KEY_SIGNATURE = 'keySignature'
+
+    MEASURE_SEPARATOR = 'measureSeparator'
+
+    MEASURE_SEPARATOR_CLASS_NAMES = {
+        MEASURE_SEPARATOR,
+    }
+
+    FLAGS_CLASS_NAMES = {
+        'flag8thUp',
+        'flag8thDown',
+        'flag16thUp',
+        'flag16thDown',
+        'flag32ndUp',
+        'flag32ndDown',
+        'flag64thUp',
+        'flag64thDown',
+    }
+
+    BEAM_CLASS_NAMES = {
+        'beam',
+    }
+
+    FLAGS_AND_BEAMS = set(list(FLAGS_CLASS_NAMES) + list(BEAM_CLASS_NAMES))
+
+    ACCIDENTAL_CLASS_NAMES = {
+        'accidentalSharp': 1,
+        'accidentalFlat': -1,
+        'accidentalNatural': 0,
+        'accidentalDoubleSharp': 2,
+        'accidentalDoubleFlat': -2,
+    }
+
+    MIDI_CODE_RESIDUES_FOR_PITCH_STEPS = {
+        0: 'C',
+        1: 'C#',
+        2: 'D',
+        3: 'Eb',
+        4: 'E',
+        5: 'F',
+        6: 'F#',
+        7: 'G',
+        8: 'Ab',
+        9: 'A',
+        10: 'Bb',
+        11: 'B',
+    }
+    '''Simplified pitch naming.'''
+
+    # The individual MIDI codes for for the unmodified steps.
+    _fs = list(range(5, 114, 12))
+    _cs = list(range(0, 121, 12))
+    _gs = list(range(7, 116, 12))
+    _ds = list(range(2, 110, 12))
+    _as = list(range(9, 118, 12))
+    _es = list(range(4, 112, 12))
+    _bs = list(range(11, 120, 12))
+
+    KEY_TABLE_SHARPS = {
+        0: {},
+        1: {i: 1 for i in _fs},
+        2: {i: 1 for i in _fs + _cs},
+        3: {i: 1 for i in _fs + _cs + _gs},
+        4: {i: 1 for i in _fs + _cs + _gs + _ds},
+        5: {i: 1 for i in _fs + _cs + _gs + _ds + _as},
+        6: {i: 1 for i in _fs + _cs + _gs + _ds + _as + _es},
+        7: {i: 1 for i in _fs + _cs + _gs + _ds + _as + _es + _bs},
+    }
+
+    KEY_TABLE_FLATS = {
+        0: {},
+        1: {i: -1 for i in _bs},
+        2: {i: -1 for i in _bs + _es},
+        3: {i: -1 for i in _bs + _es + _as},
+        4: {i: -1 for i in _bs + _es + _as + _ds},
+        5: {i: -1 for i in _bs + _es + _as + _ds + _gs},
+        6: {i: -1 for i in _bs + _es + _as + _ds + _gs + _cs},
+        7: {i: -1 for i in _bs + _es + _as + _ds + _gs + _cs + _fs},
+    }
+
+    # FROM clef --> TO clef. Imagine this on inline accidental delta
+    CLEF_CHANGE_DELTA = {
+        G_CLEF: {
+            G_CLEF: 0,
+            C_CLEF: 6,
+            F_CLEF: 12,
+        },
+        C_CLEF: {
+            G_CLEF: -6,
+            C_CLEF: 0,
+            F_CLEF: 6,
+        },
+        F_CLEF: {
+            G_CLEF: -12,
+            C_CLEF: -6,
+            F_CLEF: 0,
+        }
+    }
+
+    PITCH_STEPS = ['C', 'D', 'E', 'F', 'G', 'A', 'B',
+                   'C', 'D', 'E', 'F', 'G', 'A', 'B']
+    # Wrap around twice for easier indexing.
+
+    ACCIDENTAL_CODES = {'accidentalSharp': '#', 'accidentalFlat': 'b',
+                        'accidentalDoubleSharp': 'x', 'accidentalDoubleFlat': 'bb'}
+
+    REST_CLASS_NAMES = {
+        'restWhole',
+        'restHalf',
+        'restQuarter',
+        'rest8th',
+        'rest16th',
+        'rest32nd',
+        'rest64th',
+        'multiMeasureRest',
+    }
+
+    MEAUSURE_LASTING_CLASS_NAMES = {
+        'restWhole',
+        'multiMeasureRest',
+        'repeat1Bar',
+    }
+
+    TIME_SIGNATURES = {
+        'timeSignature',
+    }
+
+    TIME_SIG_COMMON = 'timeSigCommon'
+    TIME_SIG_CUT_COMMON = 'timeSigCutCommon'
+
+    TIME_SIGNATURE_MEMBERS = {
+        'timeSigCommon',
+        'timeSigCutCommon',
+        'numeral0',
+        'numeral1',
+        'numeral2',
+        'numeral3',
+        'numeral4',
+        'numeral5',
+        'numeral6',
+        'numeral7',
+        'numeral8',
+        'numeral9',
+    }
+
+    NUMERALS = {
+        'numeral0',
+        'numeral1',
+        'numeral2',
+        'numeral3',
+        'numeral4',
+        'numeral5',
+        'numeral6',
+        'numeral7',
+        'numeral8',
+        'numeral9',
+    }
+
+    LETTER_OTHER = 'characterOther'
+
+    @property
+    def classes_affecting_onsets(self):
+        """Returns a list of Node class names for objects
+        that affect onsets. Assumes notehead and rest durations
+        have already been given."""
+        output = set()
+        output.update(self.NONGRACE_NOTEHEAD_CLASS_NAMES)
+        output.update(self.REST_CLASS_NAMES)
+        output.update(self.MEASURE_SEPARATOR_CLASS_NAMES)
+        output.update(self.TIME_SIGNATURES)
+        output.add('repeat1Bar')
+        return output
+
+    @property
+    def classes_bearing_duration(self):
+        """Returns the list of classes that actually bear duration,
+        i.e. contribute to onsets of their descendants in the precedence
+        graph."""
+        output = set()
+        output.update(self.NONGRACE_NOTEHEAD_CLASS_NAMES)
+        output.update(self.REST_CLASS_NAMES)
+        return output
+
```

### Comparing `mung-1.1/mung/grammar.py` & `mung-1.2/mung/grammar.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,729 +1,729 @@
-"""This module implements a Grammar.
-
-A Grammar is a set of rules about how objects from a certain set
-of classes are allowed to form relationships. In a dependency grammar,
-the relationships are formed directly between the objects. (In
-constituency grammars, we'd have a "merge result" object instead.)
-
-In the ``mung`` package, you can use grammars to validate
-whether the relationships between the annotated objects conform
-to the specification.
-
-.. warning::
-
-    The grammar is not a formal specification. Music notation sometimes
-    breaks its own rules. More importantly, people who write music
-    notation by hand make mistakes. This means that not all annotation
-    files will pass grammar validation without errors, and that is fine.
-    If this bothers you, use the MUSCIMarker tool to visualize the errors.
-
-
-.. TODO::
-    create image:: ../doc/_static/grammar_explainer.png
-
-"""
-import codecs
-import logging
-import os
-import pprint
-
-import collections
-
-from typing import Tuple, List, Set, Dict
-
-
-class DependencyGrammarParseError(ValueError):
-    pass
-
-
-class DependencyGrammar(object):
-    """The DependencyGrammar class implements rules about valid graphs above
-    objects from a set of recognized classes.
-
-    The Grammar complements a Parser. It defines rules, and the Parser
-    implements algorithms to apply these rules to some input.
-
-    A grammar has an **Alphabet** and **Rules**. The alphabet is a list
-    of symbols that the grammar recognizes. Rules are constraints on
-    the structures that can be induced among these symbols.
-
-    There are two kinds of grammars according to what kinds of rules
-    they use: **dependency** rules, and **constituency** rules. We use
-    dependency grammars. Dependency grammar rules specify which symbols
-    are governing, and which symbols are governed::
-
-      noteheadFull | stem
-
-    There can be multiple left-hand side and right-hand side symbols,
-    as a shortcut for a list of rules::
-
-        noteheadFull | stem beam
-        noteheadFull noteheadHalf | legerLine durationDot tie notehead*Small
-
-    The asterisk works as a wildcard. Currently, only one wildcard per symbol
-    is allowed::
-
-      timeSignature | numeral*
-
-    Lines starting with a ``#`` are regarded as comments and ignored.
-    Empty lines are also ignored.
-
-    **Cardinality rules**
-
-    We can also specify in the grammar the minimum and/or maximum number
-    of relationships, both inlinks and outlinks, that an object can form
-    with other objects of given types. For example:
-
-    * One notehead may have up to two stems attached.
-    * We also allow for stemless full noteheads.
-    * One stem can be attached to multiple noteheads, but at least one.
-
-    This would be expressed as::
-
-      notehead*{,2} | stem{1,}
-
-    The relationship of noteheads to leger lines is generally ``m:n``::
-
-      noteheadFull | legerLine
-
-    A time signature may consist of multiple numerals, but only one
-    other symbol::
-
-      timeSignature{1,} | numeral*{1}
-      timeSignature{1} | timeSigCommon timeSigCutCommon
-
-    A key signature may have any number of sharps and flats.
-    A sharp or flat can only belong to one key signature. However,
-    not every sharp belongs to a key signature::
-
-      keySignature | accidentalSharp{,1} accidentalFlat{,1} accidentalNatural{,1} accidentalDoubleSharp{,1} accidentalDoubleFlat{,1}
-
-    For the left-hand side of the rule, the cardinality restrictions apply to
-    outlinks towards symbols of classes on the right-hand side of the rule.
-    For the right-hand side, the cardinality restrictions apply to inlinks
-    from symbols of left-hand side classes.
-
-    It is also possible to specify that regardless of where outlinks
-    lead, a symbol should always have at least some::
-
-      timeSignature{1,} |
-      repeat{2,} |
-
-    And analogously for inlinks::
-
-      | letter*{1,}
-      | numeral*{1,}
-      | legerLine{1,}
-      | noteheadFullSmall{1,}
-
-    **Interface**
-
-    The basic role of the dependency grammar is to provide the list of rules:
-
-    >>> from mung.io import parse_node_classes
-    >>> filepath = os.path.dirname(os.path.dirname(__file__)) + u'/test/test_data/mff-muscima-classes-annot.deprules'
-    >>> node_classes_path = os.path.dirname(os.path.dirname(__file__)) + u'/test/test_data/mff-muscima-classes-annot.xml'
-    >>> node_classes = parse_node_classes(node_classes_path)
-    >>> node_classes_dict = {node_class.name for node_class in node_classes}
-    >>> dependency_graph = DependencyGrammar(grammar_filename=filepath, alphabet=node_classes_dict)
-    >>> len(dependency_graph.rules)
-    646
-
-    The grammar can validate against these rules. The workhorse of this
-    functionality is the ``find_invalid_in_graph()`` method, which finds
-    objects that have inlinks/outlinks which do not comply with the grammar,
-    and the non-compliant inlinks/outlinks as well.
-
-    If we have the following notation objects ``0``, ``1``, ``2``, and ``3``,
-    with the following symbol classes:
-
-    >>> vertices = {0: 'noteheadFull', 1: 'stem', 2: 'flag8thUp', 3: 'noteheadHalf'}
-
-    And the following relationships were recorded:
-
-    >>> edges = [(0, 1), (0, 2), (0, 3)]
-
-    We can check for errors against our music notation symbols dependency
-    grammar:
-
-    >>> wrong_vertices, wrong_inlinks, wrong_outlinks, _, _, _ = \
-            dependency_graph.find_invalid_in_graph(vertices=vertices, edges=edges)
-
-    Because the edge ``(0, 3)`` connects a full notehead to an empty notehead,
-    the method should report the objects ``0`` and ``3`` as wrong, as well
-    as the corresponding inlink of ``3`` and outlink of ``0``:
-
-    >>> wrong_vertices
-    [0, 3]
-    >>> wrong_inlinks
-    [(0, 3)]
-    >>> wrong_outlinks
-    [(0, 3)]
-
-    (Note that both the inlinks and outlinks are recorded in a ``(from, to)``
-    format.)
-
-    .. caution::
-
-        Aside from checking against illegal relationships (such as we
-        saw in the example), errors can also come from too many or too
-        few inlinks/outlinks of a given type. However,
-        the validation currently implements checks only for aggregate
-        cardinalities, not for pair cardinalities (so, there can be
-        e.g. multiple sharps attached to a notehead, even though the cardinality
-        in the ``notehead | sharp`` rule is set to max. 1).
-
-    **Grammar file formats**
-
-    The alphabet is stored by means of a ``NodeClassList`` XML file with
-    :class:`NodeClass` elements, as described in the :mod:`mung.io` module.
-
-    The rules are stored in *rule files*, with the suffix ``.deprules``.
-
-    A rule file line can be empty, start with a ``#`` (comment), or contain
-    a rule symbol ``|``. Empty lines and comments are ignored during parsing.
-    Rules are split into left- and right-hand side tokens, according to
-    the position of the ``|`` symbol.
-
-    Parsing a token returns the token string (unexpanded wildcards), its
-    minimum and maximum cardinality in the rule (defaults are ``(0, 10000)``
-    if no cardinality is provided).
-
-    >>> dependency_graph.parse_token('notehead*')
-    ('notehead*', 0, 10000)
-    >>> dependency_graph.parse_token('notehead*{1,5}')
-    ('notehead*', 1, 5)
-    >>> dependency_graph.parse_token('notehead*{1,}')
-    ('notehead*', 1, 10000)
-    >>> dependency_graph.parse_token('notehead*{,5}')
-    ('notehead*', 0, 5)
-    >>> dependency_graph.parse_token('notehead*{1}')
-    ('notehead*', 1, 1)
-
-    The wildcards are expanded at the level of a line.
-
-    >>> l = 'notehead*{,2} | stem'
-    >>> rules, inlink_cards, outlink_cards, _, _ = dependency_graph.parse_dependency_grammar_line(l)
-    >>> rules
-    [('noteheadFull', 'stem'), ('noteheadFullSmall', 'stem'), ('noteheadHalf', 'stem'), ('noteheadHalfSmall', 'stem'), ('noteheadWhole', 'stem')]
-    >>> outlink_cards['noteheadHalf'] == {'stem': (0, 2)}
-    True
-    >>> inlink_cards['stem'] == {'noteheadHalf': (0, 10000), 'noteheadFull': (0, 10000),
-    ...    'noteheadWhole': (0, 10000), 'noteheadFullSmall': (0, 10000), 'noteheadHalfSmall': (0, 10000)}
-    True
-
-
-    A key signature can have any number of sharps, flats, or naturals,
-    but if a given symbol is part of a key signature, it can only be part of one.
-
-    >>> l = 'keySignature | accidentalSharp{1} accidentalFlat{1} accidentalNatural{1}'
-    >>> rules, inlink_cards, _, _, _ = dependency_graph.parse_dependency_grammar_line(l)
-    >>> rules
-    [('keySignature', 'accidentalFlat'), ('keySignature', 'accidentalNatural'), ('keySignature', 'accidentalSharp')]
-    >>> inlink_cards == {'accidentalNatural': {'keySignature': (1, 1)},
-    ...                  'accidentalSharp': {'keySignature': (1, 1)},
-    ...                  'accidentalFlat': {'keySignature': (1, 1)}}
-    True
-
-
-    You can also give *aggregate* cardinality rules, of the style "whatever rule
-    applies, there should be at least X/at most Y edges for this type of object".
-    (If no maximum is specified, the value of ``DependencyGrammar._MAX_CARD``
-    is used, which is by default 10000).
-
-    >>> l = 'keySignature{1,} |'
-    >>> _, _, _, _, out_aggregate_cards = dependency_graph.parse_dependency_grammar_line(l)
-    >>> out_aggregate_cards == {'keySignature': (1, 10000)}
-    True
-    >>> l = 'notehead*Small{1,} |'
-    >>> _, _, _, _, out_aggregate_cards = dependency_graph.parse_dependency_grammar_line(l)
-    >>> out_aggregate_cards == {'noteheadFullSmall': (1, 10000), 'noteheadHalfSmall': (1, 10000)}
-    True
-    >>> l = '| beam{1,} stem{1,} accidentalFlat{1,}'
-    >>> _, _, _, in_aggregate_cards, _ = dependency_graph.parse_dependency_grammar_line(l)
-    >>> in_aggregate_cards == {'stem': (1, 10000), 'beam': (1, 10000), 'accidentalFlat': (1, 10000)}
-    True
-
-    """
-
-    WILDCARD = '*'
-
-    _MAX_CARDINALITY = 10000
-
-    def __init__(self, grammar_filename: str, alphabet: Set[str]):
-        """Initialize the Grammar: fill in alphabet and parse rules.
-
-        :param grammar_filename: Path to a file that contains deprules
-            (see class documentation for ``*.deprules`` file format).
-
-        :param alphabet: A set or list of symbol class names, which
-            are used in the *.deprules file.
-        """
-        self.alphabet = set(alphabet)
-        # logging.info('DependencyGrammar: got alphabet:\n{0}'
-        #              ''.format(pprint.pformat(self.alphabet)))
-        self.rules = []  # type: List[Tuple[str, str]]
-        self.inlink_cardinalities = {}  # type: Dict[str, Dict[str, Tuple[int, int]]]
-        self.outlink_cardinalities = {}  # type: Dict[str, Dict[str, Tuple[int, int]]]
-        self.inlink_aggregated_cardinalities = {}  # type: Dict[str, Tuple[int, int]]
-        self.outlink_aggregated_cardinalities = {}  # type: Dict[str, Tuple[int, int]]
-
-        rules, inlink_cardinalities, outlink_cardinalities, inlink_aggregated_cardinalitites, \
-        outlink_aggregated_cardinalitites = self.parse_dependency_grammar_rules(grammar_filename)
-
-        if self.__validate_rules(rules):
-            self.rules = rules
-            logging.info('DependencyGrammar: Imported {0} rules'
-                         ''.format(len(self.rules)))
-            self.inlink_cardinalities = inlink_cardinalities
-            self.outlink_cardinalities = outlink_cardinalities
-            self.inlink_aggregated_cardinalities = inlink_aggregated_cardinalitites
-            self.outlink_aggregated_cardinalities = outlink_aggregated_cardinalitites
-            logging.debug('DependencyGrammar: Inlink aggregated cardinalities: {0}'
-                          ''.format(pprint.pformat(inlink_aggregated_cardinalitites)))
-            logging.debug('DependencyGrammar: Outlink aggregated cardinalities: {0}'
-                          ''.format(pprint.pformat(outlink_aggregated_cardinalitites)))
-        else:
-            raise DependencyGrammarParseError(
-                'Not able to parse dependency grammar file {0}.'
-                ''.format(grammar_filename))
-
-    def validate_edge(self, head_name: str, child_name: str) -> bool:
-        """Check whether a given ``head --> child`` edge conforms
-        with this grammar."""
-        return (head_name, child_name) in self.rules
-
-    def validate_graph(self, vertices: Dict[int, str], edges: List[Tuple[int, int]]):
-        """Checks whether the given graph complies with the grammar.
-
-        :param vertices: A dict with any keys and values corresponding
-            to the alphabet of the grammar.
-
-        :param edges: A list of ``(from, to)`` pairs, where both
-            ``from`` and ``to`` are valid keys into the ``vertices`` dict.
-
-        :returns: ``True`` if the graph is valid, ``False`` otherwise.
-        """
-        v, i, o, _, _, _ = self.find_invalid_in_graph(vertices=vertices, edges=edges)
-        return len(v) == 0
-
-    def find_invalid_in_graph(self, vertices: Dict[int, str], edges: List[Tuple[int, int]]) \
-            -> Tuple[List[int], List[Tuple[int, int]], List[Tuple[int, int]], Dict[int, str], Dict[
-                Tuple[int, int], str], Dict[Tuple[int, int], str]]:
-        """Finds vertices and edges where the given object graph does
-        not comply with the grammar.
-
-        Wrong vertices are any that:
-
-        * are not in the alphabet;
-        * have a wrong inlink or outlink;
-        * have missing outlinks or inlinks.
-
-        Discovering missing edges is difficult, because the grammar
-        defines cardinalities on a per-rule basis and there is currently
-        no way to make a rule compulsory, or to require at least one rule
-        from a group to apply. It is currently not implemented.
-
-        Wrong outlinks are such that:
-
-        * connect symbol pairs that should not be connected based on their
-          classes;
-        * connect so that they exceed the allowed number of outlinks to
-          the given symbol type
-
-        Wrong inlinks are such that:
-
-        * connect symbol pairs that should not be connected based on their
-          classes;
-        * connect so that they exceed the allowed number of inlinks
-          to the given symbol based on the originating symbols' classes.
-
-        :param vertices: A dict with any keys, and values corresponding
-            to the alphabet of the grammar.
-
-        :param edges: A list of ``(from, to)`` pairs, where both
-            ``from`` and ``to`` are valid keys into the ``vertices`` dict.
-
-        :param provide_reasons: If set, will generate string descriptions
-            of each error and return them.
-
-        :returns: A list of vertices, a list of inlinks and a list of outlinks
-            that do not comply with the grammar as well as three dictionaries with reasons
-            for each list respectively.
-        """
-        logging.info('DependencyGrammar: looking for errors.')
-
-        wrong_vertices = []  # type: List[int]
-        wrong_inlinks = []  # type: List[Tuple[int,int]]
-        wrong_outlinks = []  # type: List[Tuple[int,int]]
-
-        reasons_incorrect_vertices = {}  # type: Dict[int, str]
-        reasons_incorrect_inlinks = {}  # type: Dict[Tuple[int,int], str]
-        reasons_incorrect_outlinks = {}  # type: Dict[Tuple[int,int], str]
-
-        # Check that vertices have labels that are in the alphabet
-        for v, class_name in list(vertices.items()):
-            if class_name not in self.alphabet:
-                wrong_vertices.append(v)
-                reasons_incorrect_vertices[v] = 'Symbol {0} not in alphabet: class {1}.' \
-                                                ''.format(v, class_name)
-
-        # Check that all edges are allowed
-        for from_id, to_id in edges:
-            from_class_name, to_class_name = str(vertices[from_id]), str(vertices[to_id])
-            if (from_class_name, to_class_name) not in self.rules:
-                logging.debug('Wrong edge: {0} --> {1}, rules:\n{2}'
-                              ''.format(from_class_name, to_class_name, pprint.pformat(self.rules)))
-
-                wrong_inlinks.append((from_id, to_id))
-                reasons_incorrect_inlinks[(from_id, to_id)] = 'Outlink {0} ({1}) -> {2} ({3}) not in alphabet.'.format(
-                    from_class_name, from_id, to_class_name, to_id)
-
-                wrong_outlinks.append((from_id, to_id))
-                reasons_incorrect_outlinks[(from_id, to_id)] = 'Outlink {0} ({1}) -> {2} ({3}) not in alphabet.'.format(
-                    from_class_name, from_id, to_class_name, to_id)
-                if from_id not in wrong_vertices:
-                    wrong_vertices.append(from_id)
-                    reasons_incorrect_vertices[from_id] = 'Symbol {0} (class: {1}) participates ' \
-                                                          'in wrong outlink: {2} ({3}) --> {4} ({5})' \
-                                                          ''.format(from_id, vertices[from_id],
-                                                                    from_class_name, from_id,
-                                                                    to_class_name, to_id)
-                if to_id not in wrong_vertices:
-                    wrong_vertices.append(to_id)
-                    reasons_incorrect_vertices[to_id] = 'Symbol {0} (class: {1}) participates ' \
-                                                        'in wrong inlink: {2} ({3}) --> {4} ({5})' \
-                                                        ''.format(to_id, vertices[to_id],
-                                                                  from_class_name, from_id,
-                                                                  to_class_name, to_id)
-
-        # Check aggregate cardinality rules
-        #  - build inlink and outlink dicts
-        inlinks = {}
-        outlinks = {}
-        for v in vertices:
-            outlinks[v] = set()
-            inlinks[v] = set()
-        for from_id, to_id in edges:
-            outlinks[from_id].add(to_id)
-            inlinks[to_id].add(from_id)
-
-        # If there are not enough edges, the vertex itself is wrong
-        # (and none of the existing edges are wrong).
-        # Currently, if there are too many edges, the vertex itself
-        # is wrong and none of the existing edges are marked.
-        #
-        # Future:
-        # If there are too many edges, the vertex itself and *all*
-        # the edges are marked as wrong (because any of them is the extra
-        # edge, and it's easiest to just delete them and start parsing
-        # again).
-        logging.info('DependencyGrammar: checking outlink aggregate cardinalities'
-                     '\n{0}'.format(pprint.pformat(outlinks)))
-        for from_id in outlinks:
-            from_class_name = vertices[from_id]
-            if from_class_name not in self.outlink_aggregated_cardinalities:
-                # Given vertex has no aggregate cardinality restrictions
-                continue
-            cmin, cmax = self.outlink_aggregated_cardinalities[from_class_name]
-            logging.info('DependencyGrammar: checking outlink cardinality'
-                         ' rule fulfilled for vertex {0} ({1}): should be'
-                         ' within {2} -- {3}'.format(from_id, vertices[from_id], cmin, cmax))
-            if not (cmin <= len(outlinks[from_id]) <= cmax):
-                wrong_vertices.append(from_id)
-                reasons_incorrect_vertices[from_id] = 'Symbol {0} (class: {1}) has {2} outlinks,' \
-                                                      ' but grammar specifies {3} -- {4}.' \
-                                                      ''.format(from_id, vertices[from_id],
-                                                                len(outlinks[from_id]),
-                                                                cmin, cmax)
-
-        for to_id in inlinks:
-            to_class_name = vertices[to_id]
-            if to_class_name not in self.inlink_aggregated_cardinalities:
-                continue
-            cmin, cmax = self.inlink_aggregated_cardinalities[to_class_name]
-            if not (cmin <= len(inlinks[to_id]) <= cmax):
-                wrong_vertices.append(to_id)
-                reasons_incorrect_vertices[to_id] = 'Symbol {0} (class: {1}) has {2} inlinks,' \
-                                                    ' but grammar specifies {3} -- {4}.' \
-                                                    ''.format(to_id, vertices[to_id],
-                                                              len(inlinks[to_id]),
-                                                              cmin, cmax)
-
-        return wrong_vertices, wrong_inlinks, wrong_outlinks, reasons_incorrect_vertices, reasons_incorrect_inlinks, reasons_incorrect_outlinks
-
-    def parse_dependency_grammar_rules(self, filename: str) -> \
-            Tuple[List[Tuple[str, str]], Dict[str, Dict[str, Tuple[int, int]]], Dict[str, Dict[str, Tuple[int, int]]],
-                  Dict[str, Tuple[int, int]], Dict[str, Tuple[int, int]]]:
-        """Returns the rules stored in the given rule file.
-
-        A dependency grammar rule file contains grammar lines,
-        comment lines, and other lines. A grammar line is any line that
-        contains the ``|`` symbol and does *not* have a ``#`` as the first
-        non-whitespace symbol.
-
-        Comment lines are those that have ``#`` as the first non-whitespace
-        symbol. They are ignored, even if they contain ``|``. All other lines
-        that do contain ``|`` are considered to be grammar lines.
-
-        All lines that do not contain ``|`` are considered non-grammar lines
-        and are ignored.
-
-        :param filename: The path to the rule file.
-
-        :returns: A quintuplet of the grammar rules.
-
-            * ``rules``: a list of ``(from_class, to_class)`` tuples. Each rule tuple
-              encodes that relationships leading from symbols of type ``from_class``
-              to symbols of type ``to_class`` may exist.
-            * ``inlink_cards``: a dictionary that encodes the range of permitted cardinalities
-              for each RHS symbol of *inlinks* from the LHS symbols.
-            * ``outlink_cards``: a dictionary that encodes the range of permitted cardinalities
-              for each LHS of *outlinks* to the RHS symbols.
-            * ``inlink_aggregate_cards``: A dict that holds for each RHS the range of
-              permitted total inlink counts. E.g., a stem must always have at least one inlink.
-            * ``outlink_aggregate_cards``: A dict that holds for each LHS the range
-              of permitted total outlink counts. E.g., a full notehead must always have
-              at least one outlink.
-
-        """
-        rules = []
-        inlink_cardinalities = collections.OrderedDict()
-        outlink_cardinalities = collections.OrderedDict()
-
-        inlink_aggregated_cardinalities = collections.OrderedDict()
-        outlink_aggregated_cardinalities = collections.OrderedDict()
-
-        _invalid_lines = []
-        with codecs.open(filename, 'r', 'utf-8') as hdl:
-            for line_no, line in enumerate(hdl):
-                l_rules, in_card, out_card, in_agg_card, out_agg_card = self.parse_dependency_grammar_line(
-                    line)
-
-                if not self.__validate_rules(l_rules):
-                    _invalid_lines.append((line_no, line))
-
-                rules.extend(l_rules)
-
-                # Update cardinalities
-                for lhs in out_card:
-                    if lhs not in outlink_cardinalities:
-                        outlink_cardinalities[lhs] = collections.OrderedDict()
-                    outlink_cardinalities[lhs].update(out_card[lhs])
-
-                for rhs in in_card:
-                    if rhs not in inlink_cardinalities:
-                        inlink_cardinalities[rhs] = collections.OrderedDict()
-                    inlink_cardinalities[rhs].update(in_card[rhs])
-
-                inlink_aggregated_cardinalities.update(in_agg_card)
-                outlink_aggregated_cardinalities.update(out_agg_card)
-
-        if len(_invalid_lines) > 0:
-            logging.warning('DependencyGrammar.parse_rules(): Invalid lines'
-                            ' {0}'.format(pprint.pformat(_invalid_lines)))
-
-        return rules, inlink_cardinalities, outlink_cardinalities, inlink_aggregated_cardinalities, outlink_aggregated_cardinalities
-
-    def parse_dependency_grammar_line(self, line: str) -> \
-            Tuple[List[Tuple[str, str]], Dict[str, Dict[str, Tuple[int, int]]], Dict[
-                str, Dict[str, Tuple[int, int]]], Dict[str, Tuple[int, int]], Dict[str, Tuple[int, int]]]:
-        """Parse one dependency grammar line. See DependencyGrammar
-        I/O documentation for the full format description of valid
-        grammar lines.
-
-        The grammar line specifies two kinds of information: which symbol
-        classes may form relationships, and what the valid cardinalities
-        for these relationships are. For instance, while ``time_signature``
-        symbols have outlinks to ``numeral_X`` symbols, one numeral cannot
-        be part of more than one time signature.
-
-        A grammar line has a left-hand side (lhs) and a right-hand side (rhs),
-        separated by the ``|`` symbol.
-
-        (See :class:`DependencyGramamr` documentation for examples.)
-
-        :param line: One line of a dependency grammar rule file.
-
-        :returns: A quintuplet of:
-
-            * ``rules``: a list of ``(from_class, to_class)`` tuples. Each rule tuple
-              encodes that relationships leading from symbols of type ``from_class``
-              to symbols of type ``to_class`` may exist.
-            * ``inlink_cards``: a dictionary that encodes the range of permitted cardinalities
-              for each RHS symbol of *inlinks* from the LHS symbols.
-            * ``outlink_cards``: a dictionary that encodes the range of permitted cardinalities
-              for each LHS of *outlinks* to the RHS symbols.
-            * ``inlink_aggregate_cards``: A dict that holds for each RHS the range of
-              permitted total inlink counts. E.g., a stem must always have at least one inlink.
-            * ``outlink_aggregate_cards``: A dict that holds for each LHS the range
-              of permitted total outlink counts. E.g., a full notehead must always have
-              at least one outlink.
-
-            For non-grammar lines (see :meth:`parse_dependency_grammar_rules`),
-            this method returns empty data structures.
-
-        """
-        rules = []
-        out_cards = collections.OrderedDict()
-        in_cards = collections.OrderedDict()
-        out_agg_cards = collections.OrderedDict()
-        in_agg_cards = collections.OrderedDict()
-
-        _no_rule_line_output = [], collections.OrderedDict(), collections.OrderedDict(), \
-                               collections.OrderedDict(), collections.OrderedDict()
-        if line.strip().startswith('#'):
-            return _no_rule_line_output
-        if len(line.strip()) == 0:
-            return _no_rule_line_output
-        if '|' not in line:
-            return _no_rule_line_output
-
-        # logging.info('DependencyGrammar: parsing rule line:\n\t\t{0}'
-        #              ''.format(line.rstrip('\n')))
-        lhs, rhs = line.strip().split('|', 1)
-        lhs_tokens = lhs.strip().split()
-        rhs_tokens = rhs.strip().split()
-
-        # logging.info('DependencyGrammar: tokens lhs={0}, rhs={1}'
-        #             ''.format(lhs_tokens, rhs_tokens))
-
-        # Normal rule line? Aggregate cardinality line?
-        _line_type = 'normal'
-        if len(lhs) == 0:
-            _line_type = 'aggregate_inlinks'
-        if len(rhs) == 0:
-            _line_type = 'aggregate_outlinks'
-
-        logging.debug('Line {0}: type {1}, lhs={2}, rhs={3}'.format(line, _line_type, lhs, rhs))
-
-        if _line_type == 'aggregate_inlinks':
-            rhs_tokens = rhs.strip().split()
-            for rt in rhs_tokens:
-                token, rhs_cmin, rhs_cmax = self.parse_token(rt)
-                for t in self.__matching_names(token):
-                    in_agg_cards[t] = (rhs_cmin, rhs_cmax)
-            logging.debug('DependencyGrammar: found inlinks: {0}'
-                          ''.format(pprint.pformat(in_agg_cards)))
-            return rules, out_cards, in_cards, in_agg_cards, out_agg_cards
-
-        if _line_type == 'aggregate_outlinks':
-            lhs_tokens = lhs.strip().split()
-            for lt in lhs_tokens:
-                token, lhs_cmin, lhs_cmax = self.parse_token(lt.strip())
-                for t in self.__matching_names(token):
-                    out_agg_cards[t] = (lhs_cmin, lhs_cmax)
-            logging.debug('DependencyGrammar: found outlinks: {0}'
-                          ''.format(pprint.pformat(out_agg_cards)))
-            return rules, out_cards, in_cards, in_agg_cards, out_agg_cards
-
-        # Normal line that defines a left-hand side and a right-hand side
-
-        lhs_symbols = []
-        # These cardinalities apply to all left-hand side tokens,
-        # for edges leading to any of the right-hand side tokens.
-        lhs_cards = collections.OrderedDict()
-        for l in lhs_tokens:
-            token, lhs_cmin, lhs_cmax = self.parse_token(l)
-            all_tokens = self.__matching_names(token)
-            lhs_symbols.extend(all_tokens)
-            for t in all_tokens:
-                lhs_cards[t] = (lhs_cmin, lhs_cmax)
-
-        rhs_symbols = []
-        rhs_cards = collections.OrderedDict()
-        for r in rhs_tokens:
-            token, rhs_cmin, rhs_cmax = self.parse_token(r)
-            all_tokens = self.__matching_names(token)
-            rhs_symbols.extend(all_tokens)
-            for t in all_tokens:
-                rhs_cards[t] = (rhs_cmin, rhs_cmax)
-
-        # Build the outputs from the cartesian product
-        # of left-hand and right-hand tokens.
-        for l in lhs_symbols:
-            if l not in out_cards:
-                out_cards[l] = collections.OrderedDict()
-            for r in rhs_symbols:
-                if r not in in_cards:
-                    in_cards[r] = collections.OrderedDict()
-
-                rules.append((l, r))
-                out_cards[l][r] = lhs_cards[l]
-                in_cards[r][l] = rhs_cards[r]
-
-        # Fixed rule ordering
-        rules = sorted(rules)
-
-        return rules, in_cards, out_cards, in_agg_cards, out_agg_cards
-
-    def parse_token(self, token: str) -> Tuple[str, int, int]:
-        """Parse one ``*.deprules`` file token. See class documentation for
-        examples.
-
-        :param token: One token of a ``*.deprules`` file.
-
-        :return: token, cmin, cmax
-        """
-        token = str(token)
-        cmin, cmax = 0, self._MAX_CARDINALITY
-        if '{' not in token:
-            token = token
-        else:
-            token, cardinality = token[:-1].split('{')
-            if ',' not in cardinality:
-                cmin, cmax = int(cardinality), int(cardinality)
-            else:
-                cmin_string, cmax_string = cardinality.split(',')
-                if len(cmin_string) > 0:
-                    cmin = int(cmin_string)
-                if len(cmax_string) > 0:
-                    cmax = int(cmax_string)
-        return token, cmin, cmax
-
-    def __matching_names(self, token: str) -> List[str]:
-        """Returns the list of alphabet symbols that match the given
-        name (regex, currently can process one '*' wildcard).
-
-        :param token: The symbol name (pattern) to expand.
-
-        :returns: A list of matching names. Empty list if no name matches.
-        """
-        if not self.__has_wildcard(token):
-            return [token]
-
-        wildcard_idx = token.index(self.WILDCARD)
-        prefix = token[:wildcard_idx]
-        if wildcard_idx < len(token) - 1:
-            suffix = token[wildcard_idx + 1:]
-        else:
-            suffix = ''
-
-        matching_names = list(self.alphabet)
-        if len(prefix) > 0:
-            matching_names = [n for n in matching_names if n.startswith(prefix)]
-        if len(suffix) > 0:
-            matching_names = [n for n in matching_names if n.endswith(suffix)]
-
-        return matching_names
-
-    def __validate_rules(self, rules: List[Tuple[str, str]]) -> bool:
-        """Check that all the rules are valid under the current alphabet."""
-        missing_heads = set()
-        missing_children = set()
-        for h, ch in rules:
-            if h not in self.alphabet:
-                missing_heads.add(h)
-            if ch not in self.alphabet:
-                missing_children.add(ch)
-
-        if (len(missing_heads) + len(missing_children)) > 0:
-            logging.warning('DependencyGrammar.validate_rules: missing heads '
-                            '{0}, children {1}'
-                            ''.format(missing_heads, missing_children))
-            return False
-        else:
-            return True
-
-    def __has_wildcard(self, name: str) -> bool:
-        return self.WILDCARD in name
+"""This module implements a Grammar.
+
+A Grammar is a set of rules about how objects from a certain set
+of classes are allowed to form relationships. In a dependency grammar,
+the relationships are formed directly between the objects. (In
+constituency grammars, we'd have a "merge result" object instead.)
+
+In the ``mung`` package, you can use grammars to validate
+whether the relationships between the annotated objects conform
+to the specification.
+
+.. warning::
+
+    The grammar is not a formal specification. Music notation sometimes
+    breaks its own rules. More importantly, people who write music
+    notation by hand make mistakes. This means that not all annotation
+    files will pass grammar validation without errors, and that is fine.
+    If this bothers you, use the MUSCIMarker tool to visualize the errors.
+
+
+.. TODO::
+    create image:: ../doc/_static/grammar_explainer.png
+
+"""
+import codecs
+import logging
+import os
+import pprint
+
+import collections
+
+from typing import Tuple, List, Set, Dict
+
+
+class DependencyGrammarParseError(ValueError):
+    pass
+
+
+class DependencyGrammar(object):
+    """The DependencyGrammar class implements rules about valid graphs above
+    objects from a set of recognized classes.
+
+    The Grammar complements a Parser. It defines rules, and the Parser
+    implements algorithms to apply these rules to some input.
+
+    A grammar has an **Alphabet** and **Rules**. The alphabet is a list
+    of symbols that the grammar recognizes. Rules are constraints on
+    the structures that can be induced among these symbols.
+
+    There are two kinds of grammars according to what kinds of rules
+    they use: **dependency** rules, and **constituency** rules. We use
+    dependency grammars. Dependency grammar rules specify which symbols
+    are governing, and which symbols are governed::
+
+      noteheadFull | stem
+
+    There can be multiple left-hand side and right-hand side symbols,
+    as a shortcut for a list of rules::
+
+        noteheadFull | stem beam
+        noteheadFull noteheadHalf | legerLine durationDot tie notehead*Small
+
+    The asterisk works as a wildcard. Currently, only one wildcard per symbol
+    is allowed::
+
+      timeSignature | numeral*
+
+    Lines starting with a ``#`` are regarded as comments and ignored.
+    Empty lines are also ignored.
+
+    **Cardinality rules**
+
+    We can also specify in the grammar the minimum and/or maximum number
+    of relationships, both inlinks and outlinks, that an object can form
+    with other objects of given types. For example:
+
+    * One notehead may have up to two stems attached.
+    * We also allow for stemless full noteheads.
+    * One stem can be attached to multiple noteheads, but at least one.
+
+    This would be expressed as::
+
+      notehead*{,2} | stem{1,}
+
+    The relationship of noteheads to leger lines is generally ``m:n``::
+
+      noteheadFull | legerLine
+
+    A time signature may consist of multiple numerals, but only one
+    other symbol::
+
+      timeSignature{1,} | numeral*{1}
+      timeSignature{1} | timeSigCommon timeSigCutCommon
+
+    A key signature may have any number of sharps and flats.
+    A sharp or flat can only belong to one key signature. However,
+    not every sharp belongs to a key signature::
+
+      keySignature | accidentalSharp{,1} accidentalFlat{,1} accidentalNatural{,1} accidentalDoubleSharp{,1} accidentalDoubleFlat{,1}
+
+    For the left-hand side of the rule, the cardinality restrictions apply to
+    outlinks towards symbols of classes on the right-hand side of the rule.
+    For the right-hand side, the cardinality restrictions apply to inlinks
+    from symbols of left-hand side classes.
+
+    It is also possible to specify that regardless of where outlinks
+    lead, a symbol should always have at least some::
+
+      timeSignature{1,} |
+      repeat{2,} |
+
+    And analogously for inlinks::
+
+      | letter*{1,}
+      | numeral*{1,}
+      | legerLine{1,}
+      | noteheadFullSmall{1,}
+
+    **Interface**
+
+    The basic role of the dependency grammar is to provide the list of rules:
+
+    >>> from mung.io import parse_node_classes
+    >>> filepath = os.path.dirname(os.path.dirname(__file__)) + u'/test/test_data/mff-muscima-classes-annot.deprules'
+    >>> node_classes_path = os.path.dirname(os.path.dirname(__file__)) + u'/test/test_data/mff-muscima-classes-annot.xml'
+    >>> node_classes = parse_node_classes(node_classes_path)
+    >>> node_classes_dict = {node_class.name for node_class in node_classes}
+    >>> dependency_graph = DependencyGrammar(grammar_filename=filepath, alphabet=node_classes_dict)
+    >>> len(dependency_graph.rules)
+    646
+
+    The grammar can validate against these rules. The workhorse of this
+    functionality is the ``find_invalid_in_graph()`` method, which finds
+    objects that have inlinks/outlinks which do not comply with the grammar,
+    and the non-compliant inlinks/outlinks as well.
+
+    If we have the following notation objects ``0``, ``1``, ``2``, and ``3``,
+    with the following symbol classes:
+
+    >>> vertices = {0: 'noteheadFull', 1: 'stem', 2: 'flag8thUp', 3: 'noteheadHalf'}
+
+    And the following relationships were recorded:
+
+    >>> edges = [(0, 1), (0, 2), (0, 3)]
+
+    We can check for errors against our music notation symbols dependency
+    grammar:
+
+    >>> wrong_vertices, wrong_inlinks, wrong_outlinks, _, _, _ = \
+            dependency_graph.find_invalid_in_graph(vertices=vertices, edges=edges)
+
+    Because the edge ``(0, 3)`` connects a full notehead to an empty notehead,
+    the method should report the objects ``0`` and ``3`` as wrong, as well
+    as the corresponding inlink of ``3`` and outlink of ``0``:
+
+    >>> wrong_vertices
+    [0, 3]
+    >>> wrong_inlinks
+    [(0, 3)]
+    >>> wrong_outlinks
+    [(0, 3)]
+
+    (Note that both the inlinks and outlinks are recorded in a ``(from, to)``
+    format.)
+
+    .. caution::
+
+        Aside from checking against illegal relationships (such as we
+        saw in the example), errors can also come from too many or too
+        few inlinks/outlinks of a given type. However,
+        the validation currently implements checks only for aggregate
+        cardinalities, not for pair cardinalities (so, there can be
+        e.g. multiple sharps attached to a notehead, even though the cardinality
+        in the ``notehead | sharp`` rule is set to max. 1).
+
+    **Grammar file formats**
+
+    The alphabet is stored by means of a ``NodeClassList`` XML file with
+    :class:`NodeClass` elements, as described in the :mod:`mung.io` module.
+
+    The rules are stored in *rule files*, with the suffix ``.deprules``.
+
+    A rule file line can be empty, start with a ``#`` (comment), or contain
+    a rule symbol ``|``. Empty lines and comments are ignored during parsing.
+    Rules are split into left- and right-hand side tokens, according to
+    the position of the ``|`` symbol.
+
+    Parsing a token returns the token string (unexpanded wildcards), its
+    minimum and maximum cardinality in the rule (defaults are ``(0, 10000)``
+    if no cardinality is provided).
+
+    >>> dependency_graph.parse_token('notehead*')
+    ('notehead*', 0, 10000)
+    >>> dependency_graph.parse_token('notehead*{1,5}')
+    ('notehead*', 1, 5)
+    >>> dependency_graph.parse_token('notehead*{1,}')
+    ('notehead*', 1, 10000)
+    >>> dependency_graph.parse_token('notehead*{,5}')
+    ('notehead*', 0, 5)
+    >>> dependency_graph.parse_token('notehead*{1}')
+    ('notehead*', 1, 1)
+
+    The wildcards are expanded at the level of a line.
+
+    >>> l = 'notehead*{,2} | stem'
+    >>> rules, inlink_cards, outlink_cards, _, _ = dependency_graph.parse_dependency_grammar_line(l)
+    >>> rules
+    [('noteheadFull', 'stem'), ('noteheadFullSmall', 'stem'), ('noteheadHalf', 'stem'), ('noteheadHalfSmall', 'stem'), ('noteheadWhole', 'stem')]
+    >>> outlink_cards['noteheadHalf'] == {'stem': (0, 2)}
+    True
+    >>> inlink_cards['stem'] == {'noteheadHalf': (0, 10000), 'noteheadFull': (0, 10000),
+    ...    'noteheadWhole': (0, 10000), 'noteheadFullSmall': (0, 10000), 'noteheadHalfSmall': (0, 10000)}
+    True
+
+
+    A key signature can have any number of sharps, flats, or naturals,
+    but if a given symbol is part of a key signature, it can only be part of one.
+
+    >>> l = 'keySignature | accidentalSharp{1} accidentalFlat{1} accidentalNatural{1}'
+    >>> rules, inlink_cards, _, _, _ = dependency_graph.parse_dependency_grammar_line(l)
+    >>> rules
+    [('keySignature', 'accidentalFlat'), ('keySignature', 'accidentalNatural'), ('keySignature', 'accidentalSharp')]
+    >>> inlink_cards == {'accidentalNatural': {'keySignature': (1, 1)},
+    ...                  'accidentalSharp': {'keySignature': (1, 1)},
+    ...                  'accidentalFlat': {'keySignature': (1, 1)}}
+    True
+
+
+    You can also give *aggregate* cardinality rules, of the style "whatever rule
+    applies, there should be at least X/at most Y edges for this type of object".
+    (If no maximum is specified, the value of ``DependencyGrammar._MAX_CARD``
+    is used, which is by default 10000).
+
+    >>> l = 'keySignature{1,} |'
+    >>> _, _, _, _, out_aggregate_cards = dependency_graph.parse_dependency_grammar_line(l)
+    >>> out_aggregate_cards == {'keySignature': (1, 10000)}
+    True
+    >>> l = 'notehead*Small{1,} |'
+    >>> _, _, _, _, out_aggregate_cards = dependency_graph.parse_dependency_grammar_line(l)
+    >>> out_aggregate_cards == {'noteheadFullSmall': (1, 10000), 'noteheadHalfSmall': (1, 10000)}
+    True
+    >>> l = '| beam{1,} stem{1,} accidentalFlat{1,}'
+    >>> _, _, _, in_aggregate_cards, _ = dependency_graph.parse_dependency_grammar_line(l)
+    >>> in_aggregate_cards == {'stem': (1, 10000), 'beam': (1, 10000), 'accidentalFlat': (1, 10000)}
+    True
+
+    """
+
+    WILDCARD = '*'
+
+    _MAX_CARDINALITY = 10000
+
+    def __init__(self, grammar_filename: str, alphabet: Set[str]):
+        """Initialize the Grammar: fill in alphabet and parse rules.
+
+        :param grammar_filename: Path to a file that contains deprules
+            (see class documentation for ``*.deprules`` file format).
+
+        :param alphabet: A set or list of symbol class names, which
+            are used in the *.deprules file.
+        """
+        self.alphabet = set(alphabet)
+        # logging.info('DependencyGrammar: got alphabet:\n{0}'
+        #              ''.format(pprint.pformat(self.alphabet)))
+        self.rules = []  # type: List[Tuple[str, str]]
+        self.inlink_cardinalities = {}  # type: Dict[str, Dict[str, Tuple[int, int]]]
+        self.outlink_cardinalities = {}  # type: Dict[str, Dict[str, Tuple[int, int]]]
+        self.inlink_aggregated_cardinalities = {}  # type: Dict[str, Tuple[int, int]]
+        self.outlink_aggregated_cardinalities = {}  # type: Dict[str, Tuple[int, int]]
+
+        rules, inlink_cardinalities, outlink_cardinalities, inlink_aggregated_cardinalitites, \
+        outlink_aggregated_cardinalitites = self.parse_dependency_grammar_rules(grammar_filename)
+
+        if self.__validate_rules(rules):
+            self.rules = rules
+            logging.info('DependencyGrammar: Imported {0} rules'
+                         ''.format(len(self.rules)))
+            self.inlink_cardinalities = inlink_cardinalities
+            self.outlink_cardinalities = outlink_cardinalities
+            self.inlink_aggregated_cardinalities = inlink_aggregated_cardinalitites
+            self.outlink_aggregated_cardinalities = outlink_aggregated_cardinalitites
+            logging.debug('DependencyGrammar: Inlink aggregated cardinalities: {0}'
+                          ''.format(pprint.pformat(inlink_aggregated_cardinalitites)))
+            logging.debug('DependencyGrammar: Outlink aggregated cardinalities: {0}'
+                          ''.format(pprint.pformat(outlink_aggregated_cardinalitites)))
+        else:
+            raise DependencyGrammarParseError(
+                'Not able to parse dependency grammar file {0}.'
+                ''.format(grammar_filename))
+
+    def validate_edge(self, head_name: str, child_name: str) -> bool:
+        """Check whether a given ``head --> child`` edge conforms
+        with this grammar."""
+        return (head_name, child_name) in self.rules
+
+    def validate_graph(self, vertices: Dict[int, str], edges: List[Tuple[int, int]]):
+        """Checks whether the given graph complies with the grammar.
+
+        :param vertices: A dict with any keys and values corresponding
+            to the alphabet of the grammar.
+
+        :param edges: A list of ``(from, to)`` pairs, where both
+            ``from`` and ``to`` are valid keys into the ``vertices`` dict.
+
+        :returns: ``True`` if the graph is valid, ``False`` otherwise.
+        """
+        v, i, o, _, _, _ = self.find_invalid_in_graph(vertices=vertices, edges=edges)
+        return len(v) == 0
+
+    def find_invalid_in_graph(self, vertices: Dict[int, str], edges: List[Tuple[int, int]]) \
+            -> Tuple[List[int], List[Tuple[int, int]], List[Tuple[int, int]], Dict[int, str], Dict[
+                Tuple[int, int], str], Dict[Tuple[int, int], str]]:
+        """Finds vertices and edges where the given object graph does
+        not comply with the grammar.
+
+        Wrong vertices are any that:
+
+        * are not in the alphabet;
+        * have a wrong inlink or outlink;
+        * have missing outlinks or inlinks.
+
+        Discovering missing edges is difficult, because the grammar
+        defines cardinalities on a per-rule basis and there is currently
+        no way to make a rule compulsory, or to require at least one rule
+        from a group to apply. It is currently not implemented.
+
+        Wrong outlinks are such that:
+
+        * connect symbol pairs that should not be connected based on their
+          classes;
+        * connect so that they exceed the allowed number of outlinks to
+          the given symbol type
+
+        Wrong inlinks are such that:
+
+        * connect symbol pairs that should not be connected based on their
+          classes;
+        * connect so that they exceed the allowed number of inlinks
+          to the given symbol based on the originating symbols' classes.
+
+        :param vertices: A dict with any keys, and values corresponding
+            to the alphabet of the grammar.
+
+        :param edges: A list of ``(from, to)`` pairs, where both
+            ``from`` and ``to`` are valid keys into the ``vertices`` dict.
+
+        :param provide_reasons: If set, will generate string descriptions
+            of each error and return them.
+
+        :returns: A list of vertices, a list of inlinks and a list of outlinks
+            that do not comply with the grammar as well as three dictionaries with reasons
+            for each list respectively.
+        """
+        logging.info('DependencyGrammar: looking for errors.')
+
+        wrong_vertices = []  # type: List[int]
+        wrong_inlinks = []  # type: List[Tuple[int,int]]
+        wrong_outlinks = []  # type: List[Tuple[int,int]]
+
+        reasons_incorrect_vertices = {}  # type: Dict[int, str]
+        reasons_incorrect_inlinks = {}  # type: Dict[Tuple[int,int], str]
+        reasons_incorrect_outlinks = {}  # type: Dict[Tuple[int,int], str]
+
+        # Check that vertices have labels that are in the alphabet
+        for v, class_name in list(vertices.items()):
+            if class_name not in self.alphabet:
+                wrong_vertices.append(v)
+                reasons_incorrect_vertices[v] = 'Symbol {0} not in alphabet: class {1}.' \
+                                                ''.format(v, class_name)
+
+        # Check that all edges are allowed
+        for from_id, to_id in edges:
+            from_class_name, to_class_name = str(vertices[from_id]), str(vertices[to_id])
+            if (from_class_name, to_class_name) not in self.rules:
+                logging.debug('Wrong edge: {0} --> {1}, rules:\n{2}'
+                              ''.format(from_class_name, to_class_name, pprint.pformat(self.rules)))
+
+                wrong_inlinks.append((from_id, to_id))
+                reasons_incorrect_inlinks[(from_id, to_id)] = 'Outlink {0} ({1}) -> {2} ({3}) not in alphabet.'.format(
+                    from_class_name, from_id, to_class_name, to_id)
+
+                wrong_outlinks.append((from_id, to_id))
+                reasons_incorrect_outlinks[(from_id, to_id)] = 'Outlink {0} ({1}) -> {2} ({3}) not in alphabet.'.format(
+                    from_class_name, from_id, to_class_name, to_id)
+                if from_id not in wrong_vertices:
+                    wrong_vertices.append(from_id)
+                    reasons_incorrect_vertices[from_id] = 'Symbol {0} (class: {1}) participates ' \
+                                                          'in wrong outlink: {2} ({3}) --> {4} ({5})' \
+                                                          ''.format(from_id, vertices[from_id],
+                                                                    from_class_name, from_id,
+                                                                    to_class_name, to_id)
+                if to_id not in wrong_vertices:
+                    wrong_vertices.append(to_id)
+                    reasons_incorrect_vertices[to_id] = 'Symbol {0} (class: {1}) participates ' \
+                                                        'in wrong inlink: {2} ({3}) --> {4} ({5})' \
+                                                        ''.format(to_id, vertices[to_id],
+                                                                  from_class_name, from_id,
+                                                                  to_class_name, to_id)
+
+        # Check aggregate cardinality rules
+        #  - build inlink and outlink dicts
+        inlinks = {}
+        outlinks = {}
+        for v in vertices:
+            outlinks[v] = set()
+            inlinks[v] = set()
+        for from_id, to_id in edges:
+            outlinks[from_id].add(to_id)
+            inlinks[to_id].add(from_id)
+
+        # If there are not enough edges, the vertex itself is wrong
+        # (and none of the existing edges are wrong).
+        # Currently, if there are too many edges, the vertex itself
+        # is wrong and none of the existing edges are marked.
+        #
+        # Future:
+        # If there are too many edges, the vertex itself and *all*
+        # the edges are marked as wrong (because any of them is the extra
+        # edge, and it's easiest to just delete them and start parsing
+        # again).
+        logging.info('DependencyGrammar: checking outlink aggregate cardinalities'
+                     '\n{0}'.format(pprint.pformat(outlinks)))
+        for from_id in outlinks:
+            from_class_name = vertices[from_id]
+            if from_class_name not in self.outlink_aggregated_cardinalities:
+                # Given vertex has no aggregate cardinality restrictions
+                continue
+            cmin, cmax = self.outlink_aggregated_cardinalities[from_class_name]
+            logging.info('DependencyGrammar: checking outlink cardinality'
+                         ' rule fulfilled for vertex {0} ({1}): should be'
+                         ' within {2} -- {3}'.format(from_id, vertices[from_id], cmin, cmax))
+            if not (cmin <= len(outlinks[from_id]) <= cmax):
+                wrong_vertices.append(from_id)
+                reasons_incorrect_vertices[from_id] = 'Symbol {0} (class: {1}) has {2} outlinks,' \
+                                                      ' but grammar specifies {3} -- {4}.' \
+                                                      ''.format(from_id, vertices[from_id],
+                                                                len(outlinks[from_id]),
+                                                                cmin, cmax)
+
+        for to_id in inlinks:
+            to_class_name = vertices[to_id]
+            if to_class_name not in self.inlink_aggregated_cardinalities:
+                continue
+            cmin, cmax = self.inlink_aggregated_cardinalities[to_class_name]
+            if not (cmin <= len(inlinks[to_id]) <= cmax):
+                wrong_vertices.append(to_id)
+                reasons_incorrect_vertices[to_id] = 'Symbol {0} (class: {1}) has {2} inlinks,' \
+                                                    ' but grammar specifies {3} -- {4}.' \
+                                                    ''.format(to_id, vertices[to_id],
+                                                              len(inlinks[to_id]),
+                                                              cmin, cmax)
+
+        return wrong_vertices, wrong_inlinks, wrong_outlinks, reasons_incorrect_vertices, reasons_incorrect_inlinks, reasons_incorrect_outlinks
+
+    def parse_dependency_grammar_rules(self, filename: str) -> \
+            Tuple[List[Tuple[str, str]], Dict[str, Dict[str, Tuple[int, int]]], Dict[str, Dict[str, Tuple[int, int]]],
+                  Dict[str, Tuple[int, int]], Dict[str, Tuple[int, int]]]:
+        """Returns the rules stored in the given rule file.
+
+        A dependency grammar rule file contains grammar lines,
+        comment lines, and other lines. A grammar line is any line that
+        contains the ``|`` symbol and does *not* have a ``#`` as the first
+        non-whitespace symbol.
+
+        Comment lines are those that have ``#`` as the first non-whitespace
+        symbol. They are ignored, even if they contain ``|``. All other lines
+        that do contain ``|`` are considered to be grammar lines.
+
+        All lines that do not contain ``|`` are considered non-grammar lines
+        and are ignored.
+
+        :param filename: The path to the rule file.
+
+        :returns: A quintuplet of the grammar rules.
+
+            * ``rules``: a list of ``(from_class, to_class)`` tuples. Each rule tuple
+              encodes that relationships leading from symbols of type ``from_class``
+              to symbols of type ``to_class`` may exist.
+            * ``inlink_cards``: a dictionary that encodes the range of permitted cardinalities
+              for each RHS symbol of *inlinks* from the LHS symbols.
+            * ``outlink_cards``: a dictionary that encodes the range of permitted cardinalities
+              for each LHS of *outlinks* to the RHS symbols.
+            * ``inlink_aggregate_cards``: A dict that holds for each RHS the range of
+              permitted total inlink counts. E.g., a stem must always have at least one inlink.
+            * ``outlink_aggregate_cards``: A dict that holds for each LHS the range
+              of permitted total outlink counts. E.g., a full notehead must always have
+              at least one outlink.
+
+        """
+        rules = []
+        inlink_cardinalities = collections.OrderedDict()
+        outlink_cardinalities = collections.OrderedDict()
+
+        inlink_aggregated_cardinalities = collections.OrderedDict()
+        outlink_aggregated_cardinalities = collections.OrderedDict()
+
+        _invalid_lines = []
+        with codecs.open(filename, 'r', 'utf-8') as hdl:
+            for line_no, line in enumerate(hdl):
+                l_rules, in_card, out_card, in_agg_card, out_agg_card = self.parse_dependency_grammar_line(
+                    line)
+
+                if not self.__validate_rules(l_rules):
+                    _invalid_lines.append((line_no, line))
+
+                rules.extend(l_rules)
+
+                # Update cardinalities
+                for lhs in out_card:
+                    if lhs not in outlink_cardinalities:
+                        outlink_cardinalities[lhs] = collections.OrderedDict()
+                    outlink_cardinalities[lhs].update(out_card[lhs])
+
+                for rhs in in_card:
+                    if rhs not in inlink_cardinalities:
+                        inlink_cardinalities[rhs] = collections.OrderedDict()
+                    inlink_cardinalities[rhs].update(in_card[rhs])
+
+                inlink_aggregated_cardinalities.update(in_agg_card)
+                outlink_aggregated_cardinalities.update(out_agg_card)
+
+        if len(_invalid_lines) > 0:
+            logging.warning('DependencyGrammar.parse_rules(): Invalid lines'
+                            ' {0}'.format(pprint.pformat(_invalid_lines)))
+
+        return rules, inlink_cardinalities, outlink_cardinalities, inlink_aggregated_cardinalities, outlink_aggregated_cardinalities
+
+    def parse_dependency_grammar_line(self, line: str) -> \
+            Tuple[List[Tuple[str, str]], Dict[str, Dict[str, Tuple[int, int]]], Dict[
+                str, Dict[str, Tuple[int, int]]], Dict[str, Tuple[int, int]], Dict[str, Tuple[int, int]]]:
+        """Parse one dependency grammar line. See DependencyGrammar
+        I/O documentation for the full format description of valid
+        grammar lines.
+
+        The grammar line specifies two kinds of information: which symbol
+        classes may form relationships, and what the valid cardinalities
+        for these relationships are. For instance, while ``time_signature``
+        symbols have outlinks to ``numeral_X`` symbols, one numeral cannot
+        be part of more than one time signature.
+
+        A grammar line has a left-hand side (lhs) and a right-hand side (rhs),
+        separated by the ``|`` symbol.
+
+        (See :class:`DependencyGramamr` documentation for examples.)
+
+        :param line: One line of a dependency grammar rule file.
+
+        :returns: A quintuplet of:
+
+            * ``rules``: a list of ``(from_class, to_class)`` tuples. Each rule tuple
+              encodes that relationships leading from symbols of type ``from_class``
+              to symbols of type ``to_class`` may exist.
+            * ``inlink_cards``: a dictionary that encodes the range of permitted cardinalities
+              for each RHS symbol of *inlinks* from the LHS symbols.
+            * ``outlink_cards``: a dictionary that encodes the range of permitted cardinalities
+              for each LHS of *outlinks* to the RHS symbols.
+            * ``inlink_aggregate_cards``: A dict that holds for each RHS the range of
+              permitted total inlink counts. E.g., a stem must always have at least one inlink.
+            * ``outlink_aggregate_cards``: A dict that holds for each LHS the range
+              of permitted total outlink counts. E.g., a full notehead must always have
+              at least one outlink.
+
+            For non-grammar lines (see :meth:`parse_dependency_grammar_rules`),
+            this method returns empty data structures.
+
+        """
+        rules = []
+        out_cards = collections.OrderedDict()
+        in_cards = collections.OrderedDict()
+        out_agg_cards = collections.OrderedDict()
+        in_agg_cards = collections.OrderedDict()
+
+        _no_rule_line_output = [], collections.OrderedDict(), collections.OrderedDict(), \
+                               collections.OrderedDict(), collections.OrderedDict()
+        if line.strip().startswith('#'):
+            return _no_rule_line_output
+        if len(line.strip()) == 0:
+            return _no_rule_line_output
+        if '|' not in line:
+            return _no_rule_line_output
+
+        # logging.info('DependencyGrammar: parsing rule line:\n\t\t{0}'
+        #              ''.format(line.rstrip('\n')))
+        lhs, rhs = line.strip().split('|', 1)
+        lhs_tokens = lhs.strip().split()
+        rhs_tokens = rhs.strip().split()
+
+        # logging.info('DependencyGrammar: tokens lhs={0}, rhs={1}'
+        #             ''.format(lhs_tokens, rhs_tokens))
+
+        # Normal rule line? Aggregate cardinality line?
+        _line_type = 'normal'
+        if len(lhs) == 0:
+            _line_type = 'aggregate_inlinks'
+        if len(rhs) == 0:
+            _line_type = 'aggregate_outlinks'
+
+        logging.debug('Line {0}: type {1}, lhs={2}, rhs={3}'.format(line, _line_type, lhs, rhs))
+
+        if _line_type == 'aggregate_inlinks':
+            rhs_tokens = rhs.strip().split()
+            for rt in rhs_tokens:
+                token, rhs_cmin, rhs_cmax = self.parse_token(rt)
+                for t in self.__matching_names(token):
+                    in_agg_cards[t] = (rhs_cmin, rhs_cmax)
+            logging.debug('DependencyGrammar: found inlinks: {0}'
+                          ''.format(pprint.pformat(in_agg_cards)))
+            return rules, out_cards, in_cards, in_agg_cards, out_agg_cards
+
+        if _line_type == 'aggregate_outlinks':
+            lhs_tokens = lhs.strip().split()
+            for lt in lhs_tokens:
+                token, lhs_cmin, lhs_cmax = self.parse_token(lt.strip())
+                for t in self.__matching_names(token):
+                    out_agg_cards[t] = (lhs_cmin, lhs_cmax)
+            logging.debug('DependencyGrammar: found outlinks: {0}'
+                          ''.format(pprint.pformat(out_agg_cards)))
+            return rules, out_cards, in_cards, in_agg_cards, out_agg_cards
+
+        # Normal line that defines a left-hand side and a right-hand side
+
+        lhs_symbols = []
+        # These cardinalities apply to all left-hand side tokens,
+        # for edges leading to any of the right-hand side tokens.
+        lhs_cards = collections.OrderedDict()
+        for l in lhs_tokens:
+            token, lhs_cmin, lhs_cmax = self.parse_token(l)
+            all_tokens = self.__matching_names(token)
+            lhs_symbols.extend(all_tokens)
+            for t in all_tokens:
+                lhs_cards[t] = (lhs_cmin, lhs_cmax)
+
+        rhs_symbols = []
+        rhs_cards = collections.OrderedDict()
+        for r in rhs_tokens:
+            token, rhs_cmin, rhs_cmax = self.parse_token(r)
+            all_tokens = self.__matching_names(token)
+            rhs_symbols.extend(all_tokens)
+            for t in all_tokens:
+                rhs_cards[t] = (rhs_cmin, rhs_cmax)
+
+        # Build the outputs from the cartesian product
+        # of left-hand and right-hand tokens.
+        for l in lhs_symbols:
+            if l not in out_cards:
+                out_cards[l] = collections.OrderedDict()
+            for r in rhs_symbols:
+                if r not in in_cards:
+                    in_cards[r] = collections.OrderedDict()
+
+                rules.append((l, r))
+                out_cards[l][r] = lhs_cards[l]
+                in_cards[r][l] = rhs_cards[r]
+
+        # Fixed rule ordering
+        rules = sorted(rules)
+
+        return rules, in_cards, out_cards, in_agg_cards, out_agg_cards
+
+    def parse_token(self, token: str) -> Tuple[str, int, int]:
+        """Parse one ``*.deprules`` file token. See class documentation for
+        examples.
+
+        :param token: One token of a ``*.deprules`` file.
+
+        :return: token, cmin, cmax
+        """
+        token = str(token)
+        cmin, cmax = 0, self._MAX_CARDINALITY
+        if '{' not in token:
+            token = token
+        else:
+            token, cardinality = token[:-1].split('{')
+            if ',' not in cardinality:
+                cmin, cmax = int(cardinality), int(cardinality)
+            else:
+                cmin_string, cmax_string = cardinality.split(',')
+                if len(cmin_string) > 0:
+                    cmin = int(cmin_string)
+                if len(cmax_string) > 0:
+                    cmax = int(cmax_string)
+        return token, cmin, cmax
+
+    def __matching_names(self, token: str) -> List[str]:
+        """Returns the list of alphabet symbols that match the given
+        name (regex, currently can process one '*' wildcard).
+
+        :param token: The symbol name (pattern) to expand.
+
+        :returns: A list of matching names. Empty list if no name matches.
+        """
+        if not self.__has_wildcard(token):
+            return [token]
+
+        wildcard_idx = token.index(self.WILDCARD)
+        prefix = token[:wildcard_idx]
+        if wildcard_idx < len(token) - 1:
+            suffix = token[wildcard_idx + 1:]
+        else:
+            suffix = ''
+
+        matching_names = list(self.alphabet)
+        if len(prefix) > 0:
+            matching_names = [n for n in matching_names if n.startswith(prefix)]
+        if len(suffix) > 0:
+            matching_names = [n for n in matching_names if n.endswith(suffix)]
+
+        return matching_names
+
+    def __validate_rules(self, rules: List[Tuple[str, str]]) -> bool:
+        """Check that all the rules are valid under the current alphabet."""
+        missing_heads = set()
+        missing_children = set()
+        for h, ch in rules:
+            if h not in self.alphabet:
+                missing_heads.add(h)
+            if ch not in self.alphabet:
+                missing_children.add(ch)
+
+        if (len(missing_heads) + len(missing_children)) > 0:
+            logging.warning('DependencyGrammar.validate_rules: missing heads '
+                            '{0}, children {1}'
+                            ''.format(missing_heads, missing_children))
+            return False
+        else:
+            return True
+
+    def __has_wildcard(self, name: str) -> bool:
+        return self.WILDCARD in name
```

### Comparing `mung-1.1/mung/graph.py` & `mung-1.2/mung/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,953 +1,953 @@
-"""This module implements an abstraction over a notation graph, and
-functions for manipulating notation graphs."""
-import copy
-import logging
-import operator
-from queue import Queue
-
-from typing import List, Union, Dict, Set, Tuple, Iterable, Optional
-
-from mung.node import Node
-from mung.constants import InferenceEngineConstants as _CONST
-
-
-class NotationGraphError(ValueError):
-    pass
-
-
-class NotationGraphUnsupportedError(NotImplementedError):
-    pass
-
-
-class NotationGraph(object):
-    """The NotationGraph class is the abstraction for a notation graph."""
-
-    def __init__(self, nodes: List[Node]):
-        """Initialize the notation graph with a list of Nodes."""
-        self.__nodes = nodes
-        self.__id_to_node_mapping = {node.id: node for node in self.__nodes}  # type: Dict[int, Node]
-
-    def __len__(self):
-        return len(self.__nodes)
-
-    def __to_id(self, node_or_id: Union[Node, int]) -> int:
-        if isinstance(node_or_id, Node):
-            return node_or_id.id
-        else:
-            return node_or_id
-
-    @property
-    def edges(self) -> Set[Tuple[int, int]]:
-        edges = set()
-        for node in self.__nodes:
-            for t in node.outlinks:
-                if (node.id, t) not in edges:
-                    edges.add((node.id, t))
-        return edges
-
-    @property
-    def vertices(self) -> List[Node]:
-        return self.__nodes
-
-    def __getitem__(self, node_id: int) -> Node:
-        """Returns a Node based on its id."""
-        return self.__id_to_node_mapping[node_id]
-
-    def children(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> List[Node]:
-        """Find all children of the given node. class_filter can be used to only get children of a particular class. """
-        node_id = self.__to_id(node_or_id)
-        if node_id not in self.__id_to_node_mapping:
-            raise ValueError('Node {0} not in graph!'.format(self.__id_to_node_mapping[node_id].id))
-
-        parent = self.__id_to_node_mapping[node_id]
-        children = []
-        for child_id in parent.outlinks:
-            if child_id in self.__id_to_node_mapping:
-                child = self.__id_to_node_mapping[child_id]
-                if class_filter is None:
-                    children.append(child)
-                elif child.class_name in class_filter:
-                    children.append(child)
-        return children
-
-    def parents(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> List[Node]:
-        """Find all parents of the given node.  class_filter can be used to only get parents of a particular class. """
-        node_id = self.__to_id(node_or_id)
-        if node_id not in self.__id_to_node_mapping:
-            raise ValueError('Node {0} not in graph!'.format(self.__id_to_node_mapping[node_id].id))
-
-        child = self.__id_to_node_mapping[node_id]
-        parents = []
-        for parent_ids in child.inlinks:
-            if parent_ids in self.__id_to_node_mapping:
-                parent = self.__id_to_node_mapping[parent_ids]
-                if class_filter is None:
-                    parents.append(parent)
-                elif parent.class_name in class_filter:
-                    parents.append(parent)
-        return parents
-
-    def descendants(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> List[Node]:
-        """Find all descendants of the given node."""
-        node_id = self.__to_id(node_or_id)
-
-        descendant_ids = []
-        queue = Queue()
-        queue.put(node_id)
-        while not queue.empty():
-            current_node_id = queue.get()
-            if current_node_id != node_id:
-                descendant_ids.append(current_node_id)
-            children = self.children(current_node_id, class_filter=class_filter)
-            children_node_ids = [child.id for child in children]
-            for child_id in children_node_ids:
-                if child_id not in queue:
-                    queue.put(child_id)
-        return [self.__id_to_node_mapping[o] for o in descendant_ids]
-
-    def ancestors(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> List[Node]:
-        """Find all ancestors of the given node."""
-        node_id = self.__to_id(node_or_id)
-
-        ancestor_node_ids = []
-        queue = Queue()
-        queue.put(node_id)
-        while not queue.empty():
-            current_node_id = queue.get()
-            if current_node_id != node_id:
-                ancestor_node_ids.append(current_node_id)
-            parents = self.parents(current_node_id, class_filter=class_filter)
-            parent_node_ids = [parent.id for parent in parents]
-            for parent_id in parent_node_ids:
-                if parent_id not in queue:
-                    queue.put(parent_id)
-
-        return [self.__id_to_node_mapping[objid] for objid in ancestor_node_ids]
-
-    def has_children(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> bool:
-        children = self.children(node_or_id, class_filter=class_filter)
-        return len(children) > 0
-
-    def has_parents(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> bool:
-        parents = self.parents(node_or_id, class_filter=class_filter)
-        return len(parents) > 0
-
-    def is_child_of(self, child_node_or_id: Union[Node, int],
-                    parent_node_or_id: Union[Node, int]) -> bool:
-        """Check whether the first symbol is a child of the second symbol."""
-        child_id = self.__to_id(child_node_or_id)
-        parent_id = self.__to_id(parent_node_or_id)
-
-        parent = self.__id_to_node_mapping[parent_id]
-        if child_id in parent.outlinks:
-            return True
-        else:
-            return False
-
-    def is_parent_of(self, parent_node_or_id: Union[Node, int],
-                     child_node_or_id: Union[Node, int]) -> bool:
-        """Check whether the first symbol is a parent of the second symbol."""
-        return self.is_child_of(child_node_or_id, parent_node_or_id)
-
-    def is_stem_direction_above(self, notehead: Node, stem: Node) -> bool:
-        """Determines whether the given stem of the given notehead
-        is above it or below. This is not trivial due to chords.
-        """
-        if notehead.id not in self.__id_to_node_mapping:
-            raise NotationGraphError('Asking for notehead which is not in graph: {0}'.format(notehead.id))
-
-        # This works even if there is just one. There should always be one.
-        sibling_noteheads = self.parents(stem, class_filter=_CONST.NOTEHEAD_CLASS_NAMES)
-        if notehead not in sibling_noteheads:
-            raise ValueError('Asked for stem direction, but notehead {0} is'
-                             ' unrelated to given stem {1}!'
-                             ''.format(notehead.id, stem.id))
-
-        topmost_notehead = min(sibling_noteheads, key=lambda x: x.top)
-        bottom_notehead = max(sibling_noteheads, key=lambda x: x.bottom)
-
-        d_top = topmost_notehead.top - stem.top
-        d_bottom = stem.bottom - bottom_notehead.bottom
-
-        return d_top > d_bottom
-
-    def is_symbol_above_notehead(self, notehead: Node, other: Node,
-                                 compare_on_intersect: bool = False) -> bool:
-        """Determines whether the given other symbol is above
-        the given notehead.
-
-        This is non-trivial because the other may reach above *and* below
-        the given notehead, if it is long and slanted (beam, slur, ...).
-        A horizontally intersecting subset of the mask of the other symbol
-        is used to determine its vertical bounds relevant to the given object.
-        """
-        if notehead.right <= other.left:
-            # No horizontal overlap, notehead to the left
-            beam_submask = other.mask[:, :1]
-        elif notehead.left >= other.right:
-            # No horizontal overlap, notehead to the right
-            beam_submask = other.mask[:, -1:]
-        else:
-            h_bounds = (max(notehead.left, other.left),
-                        min(notehead.right, other.right))
-
-            beam_submask = other.mask[:, (h_bounds[0] - other.left):(h_bounds[1] - other.left)]
-
-        # Get vertical bounds of beam submask
-        other_submask_hsum = beam_submask.sum(axis=1)
-        other_submask_top = min([i for i in range(beam_submask.shape[0])
-                                 if other_submask_hsum[i] != 0]) + other.top
-        other_submask_bottom = max([i for i in range(beam_submask.shape[0])
-                                    if other_submask_hsum[i] != 0]) + other.top
-        if (notehead.top <= other_submask_top <= notehead.bottom) \
-                or (other_submask_bottom <= notehead.top <= other_submask_bottom):
-            if compare_on_intersect:
-                logging.warning('Notehead {0} intersecting other. Returning false.'.format(notehead.id))
-                return False
-
-        if notehead.bottom < other_submask_top:
-            return False
-
-        elif notehead.top > other_submask_bottom:
-            return True
-
-        else:
-            raise NotationGraphError('Weird relative position of notehead'
-                                     ' {0} and other {1}.'.format(notehead.id, other.id))
-
-    def remove_vertex(self, node_id: int):
-        self.remove_edges_for_vertex(node_id)
-        node = self.__id_to_node_mapping[node_id]
-        self.__nodes.remove(node)
-        del self.__id_to_node_mapping[node_id]
-
-    def remove_edge(self, from_id: int, to_id: int):
-        if from_id not in self.__id_to_node_mapping:
-            raise ValueError('Cannot remove edge from id {0}: not in graph!'
-                             ''.format(from_id))
-        if to_id not in self.__id_to_node_mapping:
-            raise ValueError('Cannot remove edge to id {0}: not in graph!'
-                             ''.format(to_id))
-
-        from_node = self.__id_to_node_mapping[from_id]
-        from_node.outlinks.remove(to_id)
-        to_node = self.__id_to_node_mapping[to_id]
-        to_node.inlinks.remove(from_id)
-
-    def remove_edges_for_vertex(self, node_id: int):
-        if node_id not in self.__id_to_node_mapping:
-            raise ValueError('Cannot remove node with id {0}: not in graph!'
-                             ''.format(node_id))
-        node = self.__id_to_node_mapping[node_id]
-
-        # Remove from inlinks and outlinks:
-        for inlink in copy.deepcopy(node.inlinks):
-            self.remove_edge(inlink, node_id)
-        for outlink in copy.deepcopy(node.outlinks):
-            self.remove_edge(node_id, outlink)
-
-    def remove_classes(self, class_names: Iterable[str]):
-        """Remove all vertices with these class names."""
-        to_remove = [node.id for node in self.__nodes if node.class_name in class_names]
-        for node_id in to_remove:
-            self.remove_vertex(node_id)
-
-    def remove_from_precedence(self, node_or_id: Union[Node, int]):
-        """Bridge the precedence edges of the given object: each of its
-        predecessors is linked to all of its descendants.
-        If there are no predecessors or no descendants, the precedence
-        edges are simply removed."""
-        node_id = self.__to_id(node_or_id)
-        node = self.__id_to_node_mapping[node_id]
-
-        predecessors, descendants = [], []
-
-        # Check if the node has at least some predecessors or descendants
-        _has_predecessors = False
-        if 'precedence_inlinks' in node.data:
-            _has_predecessors = (len(node.data['precedence_inlinks']) > 0)
-        if _has_predecessors:
-            predecessors = copy.deepcopy(
-                node.data['precedence_inlinks'])  # That damn iterator modification
-
-        _has_descendants = False
-        if 'precedence_outlinks' in node.data:
-            _has_descendants = (len(node.data['precedence_outlinks']) > 0)
-        if _has_descendants:
-            descendants = copy.deepcopy(node.data['precedence_outlinks'])
-
-        if (not _has_predecessors) and (not _has_descendants):
-            return
-
-        # Remove inlinks
-        for predecessor_id in predecessors:
-            predecessor = self.__id_to_node_mapping[predecessor_id]
-            if 'precedence_outlinks' not in predecessor.data:
-                raise ValueError(
-                    'Predecessor {} of Node {} does not have precedence outlinks!'
-                    ''.format(predecessor_id, node.id))
-            if node.id not in predecessor.data['precedence_outlinks']:
-                raise ValueError('Predecessor {} of Node {} does not have reciprocal outlink!'
-                                 ''.format(predecessor_id, node.id))
-            predecessor.data['precedence_outlinks'].remove(node.id)
-            node.data['precedence_inlinks'].remove(predecessor_id)
-
-        # Remove outlinks
-        for descentant_id in descendants:
-            descentant = self.__id_to_node_mapping[descentant_id]
-            if 'precedence_inlinks' not in descentant.data:
-                raise ValueError('Descendant {} of node {} does not have precedence inlinks!'
-                                 ''.format(descentant_id, node.id))
-            if node.id not in descentant.data['precedence_inlinks']:
-                raise ValueError('Descendant {} of node {} does not have reciprocal inlink!'
-                                 ''.format(descentant_id, node.id))
-            descentant.data['precedence_inlinks'].remove(node.id)
-            node.data['precedence_outlinks'].remove(descentant_id)
-
-        # Bridge removed element
-        for predecessor_id in predecessors:
-            predecessor = self.__id_to_node_mapping[predecessor_id]
-            for descentant_id in descendants:
-                descentant = self.__id_to_node_mapping[descentant_id]
-                if descentant_id not in predecessor.data['precedence_outlinks']:
-                    predecessor.data['precedence_outlinks'].append(descentant_id)
-                if predecessor_id not in descentant.data['precedence_inlinks']:
-                    descentant.data['precedence_inlinks'].append(predecessor_id)
-
-    def has_edge(self, from_id: int, to_id: int) -> bool:
-        if from_id not in self.__id_to_node_mapping:
-            logging.warning('Asking for object {}, which is not in graph.'.format(from_id))
-        if to_id not in self.__id_to_node_mapping:
-            logging.warning('Asking for object {}, which is not in graph.'.format(to_id))
-
-        if to_id in self.__id_to_node_mapping[from_id].outlinks:
-            if from_id in self.__id_to_node_mapping[to_id].inlinks:
-                return True
-            else:
-                raise NotationGraphError('has_edge({}, {}): found {} in outlinks'
-                                         ' of {}, but not {} in inlinks of {}!'
-                                         ''.format(from_id, to_id, to_id, from_id, from_id, to_id))
-        elif from_id in self.__id_to_node_mapping[to_id].inlinks:
-            raise NotationGraphError('has_edge({}, {}): found {} in inlinks'
-                                     ' of {}, but not {} in outlinks of {}!'
-                                     ''.format(from_id, to_id, from_id, to_id, to_id, from_id))
-        else:
-            return False
-
-    def add_edge(self, from_id: int, to_id: int):
-        """Add an edge between the MuNGOs with ids ``fr --> to``.
-        If the edge is already in the graph, warns and does nothing."""
-        if from_id not in self.__id_to_node_mapping:
-            raise NotationGraphError('Cannot remove edge from id {0}: not in graph!'.format(from_id))
-        if to_id not in self.__id_to_node_mapping:
-            raise NotationGraphError('Cannot remove edge to id {0}: not in graph!'.format(to_id))
-
-        if to_id in self.__id_to_node_mapping[from_id].outlinks:
-            if from_id in self.__id_to_node_mapping[to_id].inlinks:
-                logging.info('Adding edge that is alredy in the graph: {} --> {}'
-                             ' -- doing nothing'.format(from_id, to_id))
-                return
-            else:
-                raise NotationGraphError('add_edge({}, {}): found {} in outlinks'
-                                         ' of {}, but not {} in inlinks of {}!'
-                                         ''.format(from_id, to_id, to_id, from_id, from_id, to_id))
-        elif from_id in self.__id_to_node_mapping[to_id].inlinks:
-            raise NotationGraphError('add_edge({}, {}): found {} in inlinks'
-                                     ' of {}, but not {} in outlinks of {}!'
-                                     ''.format(from_id, to_id, from_id, to_id, to_id, from_id))
-
-        self.__id_to_node_mapping[from_id].outlinks.append(to_id)
-        self.__id_to_node_mapping[to_id].inlinks.append(from_id)
-
-
-##############################################################################
-
-
-def group_staffs_into_systems(nodes: List[Node],
-                              use_fallback_measure_separators: bool = True,
-                              leftmost_measure_separators_only: bool = False) -> List[List[Node]]:
-    """Returns a list of lists of ``staff`` Nodes
-    grouped into systems. Uses the outer ``staff_grouping``
-    symbols (or ``measure_separator``) symbols.
-
-    Currently cannot deal with a situation where a system consists of
-    interlocking staff groupings and measure separators, and cannot deal
-    with system separator markings.
-
-    :param nodes: The complete list of Nodes in the current
-        document.
-
-    :param use_fallback_measure_separators: If set and no staff groupings
-        are found, will use measure separators instead to group
-        staffs. The algorithm is to find the leftmost measure
-        separator for each staff and use this set instead of staff
-        groupings: measure separators also have outlinks to all
-        staffs that they are relevant for.
-
-    :param leftmost_measure_separators_only:
-
-    :returns: A list of systems, where each system is a list of ``staff`` Nodes.
-    """
-    graph = NotationGraph(nodes)
-    id_to_node_mapping = {c.id: c for c in nodes}
-    staff_groups = [c for c in nodes
-                    if c.class_name == 'staff_grouping']
-
-    # Do not consider staffs that have no notehead or rest children.
-    empty_staffs = [node for node in nodes if (node.class_name == 'staff') and
-                    (len([inlink for inlink in node.inlinks
-                          if ((id_to_node_mapping[inlink].class_name in _CONST.NOTEHEAD_CLASS_NAMES) or
-                              (id_to_node_mapping[inlink].class_name in _CONST.REST_CLASS_NAMES))]) == 0)]
-    print('Empty staffs: {0}'.format('\n'.join([str(node.id) for node in empty_staffs])))
-
-    # There might also be non-empty staffs that are nevertheless
-    # not covered by a staff grouping, only measure separators.
-
-    if use_fallback_measure_separators:
-        # Collect measure separators, sort them left to right
-        measure_separators = [c for c in nodes if c.class_name in _CONST.MEASURE_SEPARATOR_CLASS_NAMES]
-        measure_separators = sorted(measure_separators, key=operator.attrgetter('left'))
-        # Use only the leftmost measure separator for each staff.
-        staffs = [c for c in nodes if c.class_name in [_CONST.STAFF_CLASS_NAME]]
-
-        if leftmost_measure_separators_only:
-            leftmost_measure_separators = set()
-            for staff in staffs:
-                if staff in empty_staffs:
-                    continue
-                for m in measure_separators:
-                    if graph.is_child_of(staff, m):
-                        leftmost_measure_separators.add(m)
-                        break
-            staff_groups += leftmost_measure_separators
-        else:
-            staff_groups += measure_separators
-
-    if len(staff_groups) != 0:
-        staffs_per_group = {node.id: [id_to_node_mapping[i] for i in sorted(node.outlinks)
-                                      if id_to_node_mapping[i].class_name == 'staff'] for node in staff_groups}
-        # Build hierarchy of staff_grouping based on inclusion
-        # between grouped staff sets.
-        outer_staff_groups = []
-        for staff_group in sorted(staff_groups, key=lambda c: c.left):
-            sg_staffs = staffs_per_group[staff_group.id]
-            is_outer = True
-            for other_sg in staff_groups:
-                if staff_group.id == other_sg.id:
-                    continue
-                other_sg_staffs = staffs_per_group[other_sg.id]
-                if len([s for s in sg_staffs
-                        if s not in other_sg_staffs]) == 0:
-                    # If the staff groups are equal (can happen with
-                    # a mixture of measure-separators and staff-groupings),
-                    # only the leftmost should be an outer grouping.
-                    if set(sg_staffs) == set(other_sg_staffs):
-                        if other_sg in outer_staff_groups:
-                            is_outer = False
-                    else:
-                        is_outer = False
-            if is_outer:
-                outer_staff_groups.append(staff_group)
-
-        systems = [[c for c in nodes if (c.class_name == 'staff') and (c.id in staff_group.outlinks)] for staff_group in
-                   outer_staff_groups]
-    else:
-        # Here we use the empty staff fallback
-        systems = [[c] for c in nodes if (c.class_name == 'staff') and (c not in empty_staffs)]
-
-    return systems
-
-
-def group_by_staff(nodes: List[Node]) -> Dict[int, List[Node]]:
-    """Returns one NotationGraph instance for each staff and its associated
-    Nodes. "Associated" means:
-
-    * the object is a descendant of the staff,
-    * the object is an ancestor of the staff, or
-    * the object is a descendant of an ancestor of the staff, *except*
-      measure separators and staff groupings.
-    """
-    g = NotationGraph(nodes=nodes)
-
-    staffs = [c for c in nodes if c.class_name == _CONST.STAFF_CLASS_NAME]
-    objects_per_staff = dict()  # type: Dict[int, List[Node]]
-    for staff in staffs:
-        descendants = g.descendants(staff)
-        ancestors = g.ancestors(staff)
-        a_descendants = []
-        for ancestor in ancestors:
-            if ancestor.class_name in _CONST.SYSTEM_LEVEL_CLASS_NAMES:
-                continue
-            _ad = g.descendants(ancestor)
-            a_descendants.extend(_ad)
-        staff_related = set()
-        for c in descendants + ancestors + a_descendants:
-            staff_related.add(c)
-
-        objects_per_staff[staff.id] = list(staff_related)
-
-    return objects_per_staff
-
-
-##############################################################################
-# Graph search utilities
-
-def find_related_staffs(query_nodes: List[Node], all_nodes: Union[NotationGraph, List[Node]],
-                        with_stafflines: bool = True) -> List[Node]:
-    """Find all staffs that are related to any of the nodes
-    in question. Ignores whether these staffs are already within
-    the list of ``query_nodes`` passed to the function.
-
-    Finds all staffs that are ancestors or descendants of at least
-    one of the query Nodes, and if ``with_stafflines`` is requested,
-    all stafflines and staffspaces that are descendants of at least one
-    of the related staffs as well.
-
-    :param query_nodes: A list of Nodes for which we want
-        to find related staffs. Subset of ``all_nodes``.
-
-    :param all_nodes: A list of all the Nodes in the document
-        (or directly a NotationGraph object). Assumes that the query
-        Nodes are a subset of ``all_nodes``.
-
-    :param with_stafflines: If set, will also return all stafflines
-        and staffspaces related to the discovered staffs.
-
-    :returns: List of staff (and, if requested, staffline/staffspace)
-        Nodes that are relate to the query Nodes.
-    """
-    if not isinstance(all_nodes, NotationGraph):
-        graph = NotationGraph(all_nodes)
-    else:
-        graph = all_nodes
-
-    related_staffs = set()
-    for c in query_nodes:
-        desc_staffs = graph.descendants(c, class_filter=[_CONST.STAFF_CLASS_NAME])
-        anc_staffs = graph.ancestors(c, class_filter=[_CONST.STAFF_CLASS_NAME])
-        current_staffs = set(desc_staffs + anc_staffs)
-        related_staffs = related_staffs.union(current_staffs)
-
-    if with_stafflines:
-        related_stafflines = set()
-        for s in related_staffs:
-            staffline_objs = graph.descendants(s, _CONST.STAFFLINE_CLASS_NAMES)
-            related_stafflines = related_stafflines.union(set(staffline_objs))
-        related_staffs = related_staffs.union(related_stafflines)
-
-    return list(related_staffs)
-
-
-##############################################################################
-# Graph validation/fixing.
-# An invariant of these methods should be that they never remove a correct
-# edge. There is a known problem in this if a second stem is marked across
-# staves: the beam orientation misfires.
-
-
-def find_beams_incoherent_with_stems(nodes: List[Node]) -> List[List[Node]]:
-    """Searches the graph for edges where a notehead is connected to a stem
-    in one direction, but is connected to beams that are in the
-    other direction.
-
-    If a notehead has zero or more than one stem, it is ignored.
-
-    :returns: A list of (notehead, beam) pairs such that the beam
-        is not coherent with the stem direction for the notehead.
-    """
-    graph = NotationGraph(nodes)
-    noteheads = [c for c in nodes if c.class_name in _CONST.NOTEHEAD_CLASS_NAMES]
-
-    incoherent_pairs = []
-    for notehead in noteheads:
-        stems = graph.children(notehead, class_filter=['stem'])
-        if len(stems) != 1:
-            continue
-        stem = stems[0]
-
-        beams = graph.children(notehead, class_filter=['beam'])
-        if len(beams) == 0:
-            continue
-
-        # Is the stem above the notehead, or not?
-        # This is not trivial because of chords.
-        is_stem_above = graph.is_stem_direction_above(notehead, stem)
-        logging.info('IncoherentBeams: stem of {0} is above'.format(notehead.id))
-
-        for beam in beams:
-            try:
-                is_beam_above = graph.is_symbol_above_notehead(notehead, beam)
-            except NotationGraphError:
-                logging.warning('IncoherentBeams: something is wrong in beam-notehead pair'
-                                ' {0}, {1}'.format(beam.id, notehead.id))
-                continue
-
-            logging.info('IncoherentBeams: beam {0} of {1} is above'.format(beam.id, notehead.id))
-            if is_stem_above != is_beam_above:
-                incoherent_pairs.append([notehead, beam])
-
-    return incoherent_pairs
-
-
-# Leger lines often cause problems with autoparser.
-# They should be always linked from noteheads in a consistent
-# direction (from outside inwards to the staff).
-# Also, no notehead should be connected to both a staffline/staffspace
-# *AND* a leger line.
-
-def find_leger_lines_with_noteheads_from_both_directions(nodes: List[Node]) -> List[Node]:
-    """Looks for leger lines that have inlinks from noteheads
-    on both sides. Returns a list of leger line Nodes."""
-    graph = NotationGraph(nodes)
-
-    problem_leger_lines = []
-
-    for node in nodes:
-        if node.class_name != _CONST.LEGER_LINE_CLASS_NAME:
-            continue
-
-        noteheads = graph.parents(node, class_filter=_CONST.NOTEHEAD_CLASS_NAMES)
-
-        if len(noteheads) < 2:
-            continue
-
-        positions = [resolve_notehead_wrt_staffline(notehead, node) for notehead in noteheads]
-        positions_not_on_staffline = [p for p in positions if p != 0]
-        unique_positions = set(positions_not_on_staffline)
-        if len(unique_positions) > 1:
-            problem_leger_lines.append(node)
-
-    return problem_leger_lines
-
-
-def find_noteheads_with_leger_line_and_staff_conflict(nodes: List[Node]) -> List[Node]:
-    """Find all noteheads that have a relationship both to a staffline
-    or staffspace and to a leger line.
-
-    Assumes (obviously) that staffline relationships have already been
-    resolved. Useful in a workflow where autoparsing is applied *after*
-    staff inference.
-    """
-    graph = NotationGraph(nodes)
-
-    problem_noteheads = []
-
-    for node in nodes:
-        if node.class_name not in _CONST.NOTEHEAD_CLASS_NAMES:
-            continue
-
-        lls = graph.children(node, [_CONST.LEGER_LINE_CLASS_NAME])
-        staff_objs = graph.children(node, _CONST.STAFFLINE_CLASS_NAMES)
-        if lls and staff_objs:
-            problem_noteheads.append(node)
-
-    return problem_noteheads
-
-
-def find_noteheads_on_staff_linked_to_leger_line(nodes: List[Node]) -> List[Node]:
-    """Find all noteheads that are linked to a leger line,
-    but at the same time intersect a staffline or lie
-    entirely within a staffspace. These should be fixed
-    by linking them to the corresponding staffline/staffspace,
-    but the fixing operation should be in infer_staffline_relationships.
-
-    This is the opposite of what ``resolve_leger_line_or_staffline_object()`` is doing.
-    """
-    graph = NotationGraph(nodes)
-    problem_noteheads = []
-
-    stafflines = sorted([c for c in nodes if c.class_name == 'staff_line'],
-                        key=lambda x: x.top)
-    staffspaces = sorted([c for c in nodes if c.class_name == 'staff_space'],
-                         key=lambda x: x.top)
-
-    for node in nodes:
-        if node.class_name not in _CONST.NOTEHEAD_CLASS_NAMES:
-            continue
-
-        lls = graph.children(node, [_CONST.LEGER_LINE_CLASS_NAME])
-        if len(lls) == 0:
-            continue
-
-        # Intersecting stafflines
-        overlapped_stafflines = []
-        for sl in stafflines:
-            if node.overlaps(sl):
-                overlapped_stafflines.append(sl)
-
-        container_staffspaces = []
-        for ss in staffspaces:
-            if ss.contains(node):
-                container_staffspaces.append(ss)
-
-        if (len(overlapped_stafflines) + len(container_staffspaces)) > 0:
-            problem_noteheads.append(node)
-
-    return problem_noteheads
-
-
-def find_misdirected_leger_line_edges(nodes: List[Node], retain_ll_for_disconnected_noteheads: bool = True) -> \
-        List[List[Node]]:
-    """Finds all edges that connect to leger lines, but do not
-    lead in the direction of the staff.
-
-    Silently assumes that all noteheads are connected to the correct staff.
-
-    :param retain_ll_for_disconnected_noteheads:
-        If the notehead would be left disconnected from all stafflines
-        and staffspaces, retain its edges to its LLs -- it is better
-        to get imperfect inference rather than for the PLAY button to fail.
-    """
-    graph = NotationGraph(nodes)
-
-    misdirected_object_pairs = []
-
-    for node in nodes:
-        if node.class_name not in _CONST.NOTEHEAD_CLASS_NAMES:
-            continue
-
-        lls = graph.children(node, [_CONST.LEGER_LINE_CLASS_NAME])
-        if not lls:
-            continue
-
-        staffs = graph.children(node, [_CONST.STAFF_CLASS_NAME])
-        if not staffs:
-            logging.warning('Notehead {0} not connected to any staff!'.format(node.id))
-            continue
-        staff = staffs[0]
-
-        # Determine whether notehead is above or below staff.
-        # Because of mistakes in notehead-ll edges, can actually be
-        # *on* the staff. (If it is on a staffline, then the edge is
-        # definitely wrong.)
-        stafflines = sorted(graph.children(staff, [_CONST.STAFFLINE_CLASS_NAME]),
-                            key=lambda x: x.top)
-        p_top = resolve_notehead_wrt_staffline(node, stafflines[0])
-        p_bottom = resolve_notehead_wrt_staffline(node, stafflines[-1])
-        # Notehead actually located on the staff somewhere:
-        # all of the LL rels. are false.
-        if (p_top != p_bottom) or (p_top == 0) or (p_bottom == 0):
-            for ll in lls:
-                misdirected_object_pairs.append([node, ll])
-            continue
-
-        notehead_staff_direction = 1
-        if p_bottom == -1:
-            notehead_staff_direction = -1
-
-        _current_misdirected_object_pairs = []
-        for ll in lls:
-            ll_direction = resolve_notehead_wrt_staffline(node, ll)
-            if (ll_direction != 0) and (ll_direction != notehead_staff_direction):
-                misdirected_object_pairs.append([node, ll])
-                _current_misdirected_object_pairs.append([node, ll])
-
-        if retain_ll_for_disconnected_noteheads:
-            staffline_like_children = graph.children(node, class_filter=[_CONST.STAFFLINE_CLASS_NAME,
-                                                                         _CONST.STAFFSPACE_CLASS_NAME,
-                                                                         _CONST.LEGER_LINE_CLASS_NAME])
-            # If all the notehead's links to staffline-like objects are scheduled to be discarded:
-            if len(staffline_like_children) == len(_current_misdirected_object_pairs):
-                # Remove them from the schedule
-                misdirected_object_pairs = misdirected_object_pairs[:-len(_current_misdirected_object_pairs)]
-
-    return misdirected_object_pairs
-
-
-def resolve_leger_line_or_staffline_object(nodes: List[Node]):
-    """If staff relationships are created before notehead to leger line
-    relationships, then there will be noteheads on leger lines that
-    are nevertheless connected to staffspaces. This function should be
-    applied after both staffspace and leger line relationships have been
-    inferred, to guess whether the notehead's relationship to the staff
-    object should be discarded.
-
-    Has no dependence on misdirected edge detection (handles this as a part
-    of the conflict resolution).
-    """
-    graph = NotationGraph(nodes)
-
-    for node in nodes:
-        if node.class_name not in _CONST.NOTEHEAD_CLASS_NAMES:
-            continue
-
-        lls = graph.children(node, [_CONST.LEGER_LINE_CLASS_NAME])
-        stafflines = graph.children(node, _CONST.STAFFLINE_CLASS_NAMES)
-        staff = graph.children(node, _CONST.STAFF_CLASS_NAME)
-
-        if len(lls) == 0:
-            continue
-        if len(stafflines) == 0:
-            continue
-
-        if len(staff) == 0:
-            logging.warning('Notehead {0} not connected to any staff!'
-                            ' Unable to resolve ll/staffline.'.format(node.id))
-            continue
-
-        # Multiple LLs: must check direction
-        # Multiple stafflines: ???
-        if len(stafflines) > 1:
-            logging.warning('Notehead {0} is connected to multiple staffline'
-                            ' objects!'.format(node.id))
-
-
-##############################################################################
-
-def group_by_measure(nodes: List[Node]):
-    """Groups the objects into measures.
-    Assumes the measures are consistent across staffs: no polytempi.
-
-    If there are objects that span multiple measures, they are assigned
-    to all the measures they intersect.
-
-    If no measure separators are found, assumes everything belongs
-    to one measure.
-
-    :returns: A list of Node lists corresponding to measures. The list
-        is ordered left-to-right.
-    """
-    graph = NotationGraph(nodes)
-    logging.debug('Find measure separators.')
-
-    measure_separators = [node for node in nodes if node.class_name in _CONST.MEASURE_SEPARATOR_CLASS_NAMES]
-
-    if len(measure_separators) == 0:
-        return nodes
-
-    logging.debug('Order measure separators by precedence.')
-    # Systems
-    # measure seps. by system
-    measure_separators = sorted(measure_separators, key=lambda m: m.left)
-
-    logging.debug('Denote measure areas: bounding boxes and masks.')
-    logging.debug('Assign objects to measures, based on overlap.')
-
-    raise NotImplementedError()
-
-
-##############################################################################
-# Searching for MuNGOs that are contained within other MuNGOs
-# and removing them safely from the MuNG.
-
-def find_contained_nodes(nodes: List[Node], mask_threshold: float = 0.95):
-    """Find all nodes that are contained within other nodes
-    and not connected by an edge from container to contained.
-
-    Does *NOT* check for transitive edges!"""
-    graph = NotationGraph(nodes)
-
-    # We should have some smarter indexing structure here, but since
-    # we are just checking bounding boxes for candidates first,
-    # it does not matter too much.
-
-    nonstaff_nodes = [node for node in nodes if node.class_name not in _CONST.STAFF_CLASS_NAMES]
-
-    contained_nodes = []
-    for c1 in nonstaff_nodes:
-        for c2 in nonstaff_nodes:
-            if c1.id == c2.id:
-                continue
-            if c1.contains(c2):
-                # Check mask overlap
-                r, p, f = c1.compute_recall_precision_fscore_on_mask(c2)
-                if r < mask_threshold:
-                    continue
-                if c2.id in c1.outlinks:
-                    continue
-                contained_nodes.append(c2)
-
-    # Make unique
-    return [c for c in set(contained_nodes)]
-
-
-def remove_contained_nodes(nodes: List[Node], contained: List[Node]) -> List[Node]:
-    """Removes ``contained`` Nodes from ``nodes`` so that the
-    graph takes minimum damage.
-
-    * Attachment edges of contained objects are removed.
-    * For precedence edges, we link all precedence ancestors of a removed node
-      to all its descendants.
-    """
-    # Operating on a copy. Inefficient, but safe.
-    output_nodes = [copy.deepcopy(c) for c in nodes]
-
-    # The nodes are then edited in-place by manipulating
-    # the graph; hence we can then just return output_nodes.
-    graph = NotationGraph(output_nodes)
-    for c in contained:
-        graph.remove_from_precedence(c.id)
-    for c in contained:
-        graph.remove_vertex(c.id)
-
-    return graph.vertices
-
-
-def resolve_notehead_wrt_staffline(notehead, staffline_or_leger_line) -> int:
-    # type: (Node, Node) -> int
-    """Resolves the relative vertical position of the notehead with respect
-    to the given staff_line or legerLine object. Returns -1 if notehead
-    is *below* staffline, 0 if notehead is *on* staffline, and 1 if notehead
-    is *above* staffline."""
-    ll = staffline_or_leger_line
-
-    # Determining whether the notehead is on a leger
-    # line or in the adjacent temp staffspace.
-    # This uses a magic number, ON_STAFFLINE_RATIO_THRESHOLD.
-    output_position = 0
-
-    # Weird situation with notehead vertically *inside* bbox
-    # of leger line (could happen with slanted LLs and very small
-    # noteheads).
-    if ll.top <= notehead.top <= notehead.bottom <= ll.bottom:
-        output_position = 0
-
-    # No vertical overlap between LL and notehead
-    elif ll.top > notehead.bottom:
-        output_position = 1
-    elif notehead.top > ll.bottom:
-        output_position = -1
-
-    # Complicated situations: overlap
-    else:
-        # Notehead "around" leger line.
-        if notehead.top < ll.top <= ll.bottom < notehead.bottom:
-            dtop = ll.top - notehead.top
-            dbottom = notehead.bottom - ll.bottom
-
-            if min(dtop, dbottom) / max(dtop, dbottom) \
-                    < _CONST.ON_STAFFLINE_RATIO_THRESHOLD:
-                if dtop > dbottom:
-                    output_position = 1
-                else:
-                    output_position = -1
-
-        # Notehead interlaced with leger line, notehead on top
-        elif notehead.top < ll.top <= notehead.bottom <= ll.bottom:
-            output_position = 1
-
-        # Notehead interlaced with leger line, leger line on top
-        elif ll.top <= notehead.top <= ll.bottom < notehead.bottom:
-            output_position = -1
-
-        else:
-            logging.warning('Strange notehead {0} vs. leger line {1}'
-                            ' situation: bbox notehead {2}, LL {3}.'
-                            ' Note that the output position is unusable;'
-                            ' pleasre re-do this attachment manually.'
-                            ''.format(notehead.id, ll.id,
-                                      notehead.bounding_box,
-                                      ll.bounding_box))
-    return output_position
-
-
-def is_notehead_on_line(notehead, line) -> bool:
-    # type: (Node, Node) -> bool
-    """Check whether given notehead is positioned on the line object."""
-    if line.class_name not in _CONST.STAFFLINE_LIKE_CLASS_NAMES:
-        raise ValueError('Cannot resolve relative position of notehead'
-                         ' {0} to non-staffline-like object {1}'
-                         ''.format(notehead.id, line.id))
-
-    position = resolve_notehead_wrt_staffline(notehead, line)
-    return position == 0
+"""This module implements an abstraction over a notation graph, and
+functions for manipulating notation graphs."""
+import copy
+import logging
+import operator
+from queue import Queue
+
+from typing import List, Union, Dict, Set, Tuple, Iterable, Optional
+
+from mung.node import Node
+from mung.constants import InferenceEngineConstants
+_CONST = InferenceEngineConstants()
+
+class NotationGraphError(ValueError):
+    pass
+
+
+class NotationGraphUnsupportedError(NotImplementedError):
+    pass
+
+
+class NotationGraph(object):
+    """The NotationGraph class is the abstraction for a notation graph."""
+
+    def __init__(self, nodes: List[Node]):
+        """Initialize the notation graph with a list of Nodes."""
+        self.__nodes = nodes
+        self.__id_to_node_mapping = {node.id: node for node in self.__nodes}  # type: Dict[int, Node]
+
+    def __len__(self):
+        return len(self.__nodes)
+
+    def __to_id(self, node_or_id: Union[Node, int]) -> int:
+        if isinstance(node_or_id, Node):
+            return node_or_id.id
+        else:
+            return node_or_id
+
+    @property
+    def edges(self) -> Set[Tuple[int, int]]:
+        edges = set()
+        for node in self.__nodes:
+            for t in node.outlinks:
+                if (node.id, t) not in edges:
+                    edges.add((node.id, t))
+        return edges
+
+    @property
+    def vertices(self) -> List[Node]:
+        return self.__nodes
+
+    def __getitem__(self, node_id: int) -> Node:
+        """Returns a Node based on its id."""
+        return self.__id_to_node_mapping[node_id]
+
+    def children(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> List[Node]:
+        """Find all children of the given node. class_filter can be used to only get children of a particular class. """
+        node_id = self.__to_id(node_or_id)
+        if node_id not in self.__id_to_node_mapping:
+            raise ValueError('Node {0} not in graph!'.format(self.__id_to_node_mapping[node_id].id))
+
+        parent = self.__id_to_node_mapping[node_id]
+        children = []
+        for child_id in parent.outlinks:
+            if child_id in self.__id_to_node_mapping:
+                child = self.__id_to_node_mapping[child_id]
+                if class_filter is None:
+                    children.append(child)
+                elif child.class_name in class_filter:
+                    children.append(child)
+        return children
+
+    def parents(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> List[Node]:
+        """Find all parents of the given node.  class_filter can be used to only get parents of a particular class. """
+        node_id = self.__to_id(node_or_id)
+        if node_id not in self.__id_to_node_mapping:
+            raise ValueError('Node {0} not in graph!'.format(self.__id_to_node_mapping[node_id].id))
+
+        child = self.__id_to_node_mapping[node_id]
+        parents = []
+        for parent_ids in child.inlinks:
+            if parent_ids in self.__id_to_node_mapping:
+                parent = self.__id_to_node_mapping[parent_ids]
+                if class_filter is None:
+                    parents.append(parent)
+                elif parent.class_name in class_filter:
+                    parents.append(parent)
+        return parents
+
+    def descendants(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> List[Node]:
+        """Find all descendants of the given node."""
+        node_id = self.__to_id(node_or_id)
+
+        descendant_ids = []
+        queue = Queue()
+        queue.put(node_id)
+        while not queue.empty():
+            current_node_id = queue.get()
+            if current_node_id != node_id:
+                descendant_ids.append(current_node_id)
+            children = self.children(current_node_id, class_filter=class_filter)
+            children_node_ids = [child.id for child in children]
+            for child_id in children_node_ids:
+                if child_id not in queue:
+                    queue.put(child_id)
+        return [self.__id_to_node_mapping[o] for o in descendant_ids]
+
+    def ancestors(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> List[Node]:
+        """Find all ancestors of the given node."""
+        node_id = self.__to_id(node_or_id)
+
+        ancestor_node_ids = []
+        queue = Queue()
+        queue.put(node_id)
+        while not queue.empty():
+            current_node_id = queue.get()
+            if current_node_id != node_id:
+                ancestor_node_ids.append(current_node_id)
+            parents = self.parents(current_node_id, class_filter=class_filter)
+            parent_node_ids = [parent.id for parent in parents]
+            for parent_id in parent_node_ids:
+                if parent_id not in queue.queue:
+                    queue.put(parent_id)
+
+        return [self.__id_to_node_mapping[objid] for objid in ancestor_node_ids]
+
+    def has_children(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> bool:
+        children = self.children(node_or_id, class_filter=class_filter)
+        return len(children) > 0
+
+    def has_parents(self, node_or_id: Union[Node, int], class_filter: Optional[Iterable[str]] = None) -> bool:
+        parents = self.parents(node_or_id, class_filter=class_filter)
+        return len(parents) > 0
+
+    def is_child_of(self, child_node_or_id: Union[Node, int],
+                    parent_node_or_id: Union[Node, int]) -> bool:
+        """Check whether the first symbol is a child of the second symbol."""
+        child_id = self.__to_id(child_node_or_id)
+        parent_id = self.__to_id(parent_node_or_id)
+
+        parent = self.__id_to_node_mapping[parent_id]
+        if child_id in parent.outlinks:
+            return True
+        else:
+            return False
+
+    def is_parent_of(self, parent_node_or_id: Union[Node, int],
+                     child_node_or_id: Union[Node, int]) -> bool:
+        """Check whether the first symbol is a parent of the second symbol."""
+        return self.is_child_of(child_node_or_id, parent_node_or_id)
+
+    def is_stem_direction_above(self, notehead: Node, stem: Node) -> bool:
+        """Determines whether the given stem of the given notehead
+        is above it or below. This is not trivial due to chords.
+        """
+        if notehead.id not in self.__id_to_node_mapping:
+            raise NotationGraphError('Asking for notehead which is not in graph: {0}'.format(notehead.id))
+
+        # This works even if there is just one. There should always be one.
+        sibling_noteheads = self.parents(stem, class_filter=_CONST.NOTEHEAD_CLASS_NAMES)
+        if notehead not in sibling_noteheads:
+            raise ValueError('Asked for stem direction, but notehead {0} is'
+                             ' unrelated to given stem {1}!'
+                             ''.format(notehead.id, stem.id))
+
+        topmost_notehead = min(sibling_noteheads, key=lambda x: x.top)
+        bottom_notehead = max(sibling_noteheads, key=lambda x: x.bottom)
+
+        d_top = topmost_notehead.top - stem.top
+        d_bottom = stem.bottom - bottom_notehead.bottom
+
+        return d_top > d_bottom
+
+    def is_symbol_above_notehead(self, notehead: Node, other: Node,
+                                 compare_on_intersect: bool = False) -> bool:
+        """Determines whether the given other symbol is above
+        the given notehead.
+
+        This is non-trivial because the other may reach above *and* below
+        the given notehead, if it is long and slanted (beam, slur, ...).
+        A horizontally intersecting subset of the mask of the other symbol
+        is used to determine its vertical bounds relevant to the given object.
+        """
+        if notehead.right <= other.left:
+            # No horizontal overlap, notehead to the left
+            beam_submask = other.mask[:, :1]
+        elif notehead.left >= other.right:
+            # No horizontal overlap, notehead to the right
+            beam_submask = other.mask[:, -1:]
+        else:
+            h_bounds = (max(notehead.left, other.left),
+                        min(notehead.right, other.right))
+
+            beam_submask = other.mask[:, (h_bounds[0] - other.left):(h_bounds[1] - other.left)]
+
+        # Get vertical bounds of beam submask
+        other_submask_hsum = beam_submask.sum(axis=1)
+        other_submask_top = min([i for i in range(beam_submask.shape[0])
+                                 if other_submask_hsum[i] != 0]) + other.top
+        other_submask_bottom = max([i for i in range(beam_submask.shape[0])
+                                    if other_submask_hsum[i] != 0]) + other.top
+        if (notehead.top <= other_submask_top <= notehead.bottom) \
+                or (other_submask_bottom <= notehead.top <= other_submask_bottom):
+            if compare_on_intersect:
+                logging.warning('Notehead {0} intersecting other. Returning false.'.format(notehead.id))
+                return False
+
+        if notehead.bottom < other_submask_top:
+            return False
+
+        elif notehead.top > other_submask_bottom:
+            return True
+
+        else:
+            raise NotationGraphError('Weird relative position of notehead'
+                                     ' {0} and other {1}.'.format(notehead.id, other.id))
+
+    def remove_vertex(self, node_id: int):
+        self.remove_edges_for_vertex(node_id)
+        node = self.__id_to_node_mapping[node_id]
+        self.__nodes.remove(node)
+        del self.__id_to_node_mapping[node_id]
+
+    def remove_edge(self, from_id: int, to_id: int):
+        if from_id not in self.__id_to_node_mapping:
+            raise ValueError('Cannot remove edge from id {0}: not in graph!'
+                             ''.format(from_id))
+        if to_id not in self.__id_to_node_mapping:
+            raise ValueError('Cannot remove edge to id {0}: not in graph!'
+                             ''.format(to_id))
+
+        from_node = self.__id_to_node_mapping[from_id]
+        from_node.outlinks.remove(to_id)
+        to_node = self.__id_to_node_mapping[to_id]
+        to_node.inlinks.remove(from_id)
+
+    def remove_edges_for_vertex(self, node_id: int):
+        if node_id not in self.__id_to_node_mapping:
+            raise ValueError('Cannot remove node with id {0}: not in graph!'
+                             ''.format(node_id))
+        node = self.__id_to_node_mapping[node_id]
+
+        # Remove from inlinks and outlinks:
+        for inlink in copy.deepcopy(node.inlinks):
+            self.remove_edge(inlink, node_id)
+        for outlink in copy.deepcopy(node.outlinks):
+            self.remove_edge(node_id, outlink)
+
+    def remove_classes(self, class_names: Iterable[str]):
+        """Remove all vertices with these class names."""
+        to_remove = [node.id for node in self.__nodes if node.class_name in class_names]
+        for node_id in to_remove:
+            self.remove_vertex(node_id)
+
+    def remove_from_precedence(self, node_or_id: Union[Node, int]):
+        """Bridge the precedence edges of the given object: each of its
+        predecessors is linked to all of its descendants.
+        If there are no predecessors or no descendants, the precedence
+        edges are simply removed."""
+        node_id = self.__to_id(node_or_id)
+        node = self.__id_to_node_mapping[node_id]
+
+        predecessors, descendants = [], []
+
+        # Check if the node has at least some predecessors or descendants
+        _has_predecessors = False
+        if 'precedence_inlinks' in node.data:
+            _has_predecessors = (len(node.data['precedence_inlinks']) > 0)
+        if _has_predecessors:
+            predecessors = copy.deepcopy(
+                node.data['precedence_inlinks'])  # That damn iterator modification
+
+        _has_descendants = False
+        if 'precedence_outlinks' in node.data:
+            _has_descendants = (len(node.data['precedence_outlinks']) > 0)
+        if _has_descendants:
+            descendants = copy.deepcopy(node.data['precedence_outlinks'])
+
+        if (not _has_predecessors) and (not _has_descendants):
+            return
+
+        # Remove inlinks
+        for predecessor_id in predecessors:
+            predecessor = self.__id_to_node_mapping[predecessor_id]
+            if 'precedence_outlinks' not in predecessor.data:
+                raise ValueError(
+                    'Predecessor {} of Node {} does not have precedence outlinks!'
+                    ''.format(predecessor_id, node.id))
+            if node.id not in predecessor.data['precedence_outlinks']:
+                raise ValueError('Predecessor {} of Node {} does not have reciprocal outlink!'
+                                 ''.format(predecessor_id, node.id))
+            predecessor.data['precedence_outlinks'].remove(node.id)
+            node.data['precedence_inlinks'].remove(predecessor_id)
+
+        # Remove outlinks
+        for descentant_id in descendants:
+            descentant = self.__id_to_node_mapping[descentant_id]
+            if 'precedence_inlinks' not in descentant.data:
+                raise ValueError('Descendant {} of node {} does not have precedence inlinks!'
+                                 ''.format(descentant_id, node.id))
+            if node.id not in descentant.data['precedence_inlinks']:
+                raise ValueError('Descendant {} of node {} does not have reciprocal inlink!'
+                                 ''.format(descentant_id, node.id))
+            descentant.data['precedence_inlinks'].remove(node.id)
+            node.data['precedence_outlinks'].remove(descentant_id)
+
+        # Bridge removed element
+        for predecessor_id in predecessors:
+            predecessor = self.__id_to_node_mapping[predecessor_id]
+            for descentant_id in descendants:
+                descentant = self.__id_to_node_mapping[descentant_id]
+                if descentant_id not in predecessor.data['precedence_outlinks']:
+                    predecessor.data['precedence_outlinks'].append(descentant_id)
+                if predecessor_id not in descentant.data['precedence_inlinks']:
+                    descentant.data['precedence_inlinks'].append(predecessor_id)
+
+    def has_edge(self, from_id: int, to_id: int) -> bool:
+        if from_id not in self.__id_to_node_mapping:
+            logging.warning('Asking for object {}, which is not in graph.'.format(from_id))
+        if to_id not in self.__id_to_node_mapping:
+            logging.warning('Asking for object {}, which is not in graph.'.format(to_id))
+
+        if to_id in self.__id_to_node_mapping[from_id].outlinks:
+            if from_id in self.__id_to_node_mapping[to_id].inlinks:
+                return True
+            else:
+                raise NotationGraphError('has_edge({}, {}): found {} in outlinks'
+                                         ' of {}, but not {} in inlinks of {}!'
+                                         ''.format(from_id, to_id, to_id, from_id, from_id, to_id))
+        elif from_id in self.__id_to_node_mapping[to_id].inlinks:
+            raise NotationGraphError('has_edge({}, {}): found {} in inlinks'
+                                     ' of {}, but not {} in outlinks of {}!'
+                                     ''.format(from_id, to_id, from_id, to_id, to_id, from_id))
+        else:
+            return False
+
+    def add_edge(self, from_id: int, to_id: int):
+        """Add an edge between the MuNGOs with ids ``fr --> to``.
+        If the edge is already in the graph, warns and does nothing."""
+        if from_id not in self.__id_to_node_mapping:
+            raise NotationGraphError('Cannot remove edge from id {0}: not in graph!'.format(from_id))
+        if to_id not in self.__id_to_node_mapping:
+            raise NotationGraphError('Cannot remove edge to id {0}: not in graph!'.format(to_id))
+
+        if to_id in self.__id_to_node_mapping[from_id].outlinks:
+            if from_id in self.__id_to_node_mapping[to_id].inlinks:
+                logging.info('Adding edge that is alredy in the graph: {} --> {}'
+                             ' -- doing nothing'.format(from_id, to_id))
+                return
+            else:
+                raise NotationGraphError('add_edge({}, {}): found {} in outlinks'
+                                         ' of {}, but not {} in inlinks of {}!'
+                                         ''.format(from_id, to_id, to_id, from_id, from_id, to_id))
+        elif from_id in self.__id_to_node_mapping[to_id].inlinks:
+            raise NotationGraphError('add_edge({}, {}): found {} in inlinks'
+                                     ' of {}, but not {} in outlinks of {}!'
+                                     ''.format(from_id, to_id, from_id, to_id, to_id, from_id))
+
+        self.__id_to_node_mapping[from_id].outlinks.append(to_id)
+        self.__id_to_node_mapping[to_id].inlinks.append(from_id)
+
+
+##############################################################################
+
+
+def group_staffs_into_systems(nodes: List[Node],
+                              use_fallback_measure_separators: bool = True,
+                              leftmost_measure_separators_only: bool = False) -> List[List[Node]]:
+    """Returns a list of lists of ``staff`` Nodes
+    grouped into systems. Uses the outer ``staff_grouping``
+    symbols (or ``measure_separator``) symbols.
+
+    Currently cannot deal with a situation where a system consists of
+    interlocking staff groupings and measure separators, and cannot deal
+    with system separator markings.
+
+    :param nodes: The complete list of Nodes in the current
+        document.
+
+    :param use_fallback_measure_separators: If set and no staff groupings
+        are found, will use measure separators instead to group
+        staffs. The algorithm is to find the leftmost measure
+        separator for each staff and use this set instead of staff
+        groupings: measure separators also have outlinks to all
+        staffs that they are relevant for.
+
+    :param leftmost_measure_separators_only:
+
+    :returns: A list of systems, where each system is a list of ``staff`` Nodes.
+    """
+    graph = NotationGraph(nodes)
+    id_to_node_mapping = {c.id: c for c in nodes}
+    staff_groups = [c for c in nodes
+                    if c.class_name == 'staff_grouping']
+
+    # Do not consider staffs that have no notehead or rest children.
+    empty_staffs = [node for node in nodes if (node.class_name == 'staff') and
+                    (len([inlink for inlink in node.inlinks
+                          if ((id_to_node_mapping[inlink].class_name in _CONST.NOTEHEAD_CLASS_NAMES) or
+                              (id_to_node_mapping[inlink].class_name in _CONST.REST_CLASS_NAMES))]) == 0)]
+    print('Empty staffs: {0}'.format('\n'.join([str(node.id) for node in empty_staffs])))
+
+    # There might also be non-empty staffs that are nevertheless
+    # not covered by a staff grouping, only measure separators.
+
+    if use_fallback_measure_separators:
+        # Collect measure separators, sort them left to right
+        measure_separators = [c for c in nodes if c.class_name in _CONST.MEASURE_SEPARATOR_CLASS_NAMES]
+        measure_separators = sorted(measure_separators, key=operator.attrgetter('left'))
+        # Use only the leftmost measure separator for each staff.
+        staffs = [c for c in nodes if c.class_name in [_CONST.STAFF]]
+
+        if leftmost_measure_separators_only:
+            leftmost_measure_separators = set()
+            for staff in staffs:
+                if staff in empty_staffs:
+                    continue
+                for m in measure_separators:
+                    if graph.is_child_of(staff, m):
+                        leftmost_measure_separators.add(m)
+                        break
+            staff_groups += leftmost_measure_separators
+        else:
+            staff_groups += measure_separators
+
+    if len(staff_groups) != 0:
+        staffs_per_group = {node.id: [id_to_node_mapping[i] for i in sorted(node.outlinks)
+                                      if id_to_node_mapping[i].class_name == 'staff'] for node in staff_groups}
+        # Build hierarchy of staff_grouping based on inclusion
+        # between grouped staff sets.
+        outer_staff_groups = []
+        for staff_group in sorted(staff_groups, key=lambda c: c.left):
+            sg_staffs = staffs_per_group[staff_group.id]
+            is_outer = True
+            for other_sg in staff_groups:
+                if staff_group.id == other_sg.id:
+                    continue
+                other_sg_staffs = staffs_per_group[other_sg.id]
+                if len([s for s in sg_staffs
+                        if s not in other_sg_staffs]) == 0:
+                    # If the staff groups are equal (can happen with
+                    # a mixture of measure-separators and staff-groupings),
+                    # only the leftmost should be an outer grouping.
+                    if set(sg_staffs) == set(other_sg_staffs):
+                        if other_sg in outer_staff_groups:
+                            is_outer = False
+                    else:
+                        is_outer = False
+            if is_outer:
+                outer_staff_groups.append(staff_group)
+
+        systems = [[c for c in nodes if (c.class_name == 'staff') and (c.id in staff_group.outlinks)] for staff_group in
+                   outer_staff_groups]
+    else:
+        # Here we use the empty staff fallback
+        systems = [[c] for c in nodes if (c.class_name == 'staff') and (c not in empty_staffs)]
+
+    return systems
+
+
+def group_by_staff(nodes: List[Node]) -> Dict[int, List[Node]]:
+    """Returns one NotationGraph instance for each staff and its associated
+    Nodes. "Associated" means:
+
+    * the object is a descendant of the staff,
+    * the object is an ancestor of the staff, or
+    * the object is a descendant of an ancestor of the staff, *except*
+      measure separators and staff groupings.
+    """
+    g = NotationGraph(nodes=nodes)
+
+    staffs = [c for c in nodes if c.class_name == _CONST.STAFF]
+    objects_per_staff = dict()  # type: Dict[int, List[Node]]
+    for staff in staffs:
+        descendants = g.descendants(staff)
+        ancestors = g.ancestors(staff)
+        a_descendants = []
+        for ancestor in ancestors:
+            if ancestor.class_name in _CONST.SYSTEM_LEVEL_CLASS_NAMES:
+                continue
+            _ad = g.descendants(ancestor)
+            a_descendants.extend(_ad)
+        staff_related = set()
+        for c in descendants + ancestors + a_descendants:
+            staff_related.add(c)
+
+        objects_per_staff[staff.id] = list(staff_related)
+
+    return objects_per_staff
+
+
+##############################################################################
+# Graph search utilities
+
+def find_related_staffs(query_nodes: List[Node], all_nodes: Union[NotationGraph, List[Node]],
+                        with_stafflines: bool = True) -> List[Node]:
+    """Find all staffs that are related to any of the nodes
+    in question. Ignores whether these staffs are already within
+    the list of ``query_nodes`` passed to the function.
+
+    Finds all staffs that are ancestors or descendants of at least
+    one of the query Nodes, and if ``with_stafflines`` is requested,
+    all stafflines and staffspaces that are descendants of at least one
+    of the related staffs as well.
+
+    :param query_nodes: A list of Nodes for which we want
+        to find related staffs. Subset of ``all_nodes``.
+
+    :param all_nodes: A list of all the Nodes in the document
+        (or directly a NotationGraph object). Assumes that the query
+        Nodes are a subset of ``all_nodes``.
+
+    :param with_stafflines: If set, will also return all stafflines
+        and staffspaces related to the discovered staffs.
+
+    :returns: List of staff (and, if requested, staffline/staffspace)
+        Nodes that are relate to the query Nodes.
+    """
+    if not isinstance(all_nodes, NotationGraph):
+        graph = NotationGraph(all_nodes)
+    else:
+        graph = all_nodes
+
+    related_staffs = set()
+    for c in query_nodes:
+        desc_staffs = graph.descendants(c, class_filter=[_CONST.STAFF])
+        anc_staffs = graph.ancestors(c, class_filter=[_CONST.STAFF])
+        current_staffs = set(desc_staffs + anc_staffs)
+        related_staffs = related_staffs.union(current_staffs)
+
+    if with_stafflines:
+        related_stafflines = set()
+        for s in related_staffs:
+            staffline_objs = graph.descendants(s, _CONST.STAFFLINE_CLASS_NAMES)
+            related_stafflines = related_stafflines.union(set(staffline_objs))
+        related_staffs = related_staffs.union(related_stafflines)
+
+    return list(related_staffs)
+
+
+##############################################################################
+# Graph validation/fixing.
+# An invariant of these methods should be that they never remove a correct
+# edge. There is a known problem in this if a second stem is marked across
+# staves: the beam orientation misfires.
+
+
+def find_beams_incoherent_with_stems(nodes: List[Node]) -> List[List[Node]]:
+    """Searches the graph for edges where a notehead is connected to a stem
+    in one direction, but is connected to beams that are in the
+    other direction.
+
+    If a notehead has zero or more than one stem, it is ignored.
+
+    :returns: A list of (notehead, beam) pairs such that the beam
+        is not coherent with the stem direction for the notehead.
+    """
+    graph = NotationGraph(nodes)
+    noteheads = [c for c in nodes if c.class_name in _CONST.NOTEHEAD_CLASS_NAMES]
+
+    incoherent_pairs = []
+    for notehead in noteheads:
+        stems = graph.children(notehead, class_filter=['stem'])
+        if len(stems) != 1:
+            continue
+        stem = stems[0]
+
+        beams = graph.children(notehead, class_filter=['beam'])
+        if len(beams) == 0:
+            continue
+
+        # Is the stem above the notehead, or not?
+        # This is not trivial because of chords.
+        is_stem_above = graph.is_stem_direction_above(notehead, stem)
+        logging.info('IncoherentBeams: stem of {0} is above'.format(notehead.id))
+
+        for beam in beams:
+            try:
+                is_beam_above = graph.is_symbol_above_notehead(notehead, beam)
+            except NotationGraphError:
+                logging.warning('IncoherentBeams: something is wrong in beam-notehead pair'
+                                ' {0}, {1}'.format(beam.id, notehead.id))
+                continue
+
+            logging.info('IncoherentBeams: beam {0} of {1} is above'.format(beam.id, notehead.id))
+            if is_stem_above != is_beam_above:
+                incoherent_pairs.append([notehead, beam])
+
+    return incoherent_pairs
+
+
+# Leger lines often cause problems with autoparser.
+# They should be always linked from noteheads in a consistent
+# direction (from outside inwards to the staff).
+# Also, no notehead should be connected to both a staffline/staffspace
+# *AND* a leger line.
+
+def find_leger_lines_with_noteheads_from_both_directions(nodes: List[Node]) -> List[Node]:
+    """Looks for leger lines that have inlinks from noteheads
+    on both sides. Returns a list of leger line Nodes."""
+    graph = NotationGraph(nodes)
+
+    problem_leger_lines = []
+
+    for node in nodes:
+        if node.class_name != _CONST.LEGER_LINE:
+            continue
+
+        noteheads = graph.parents(node, class_filter=_CONST.NOTEHEAD_CLASS_NAMES)
+
+        if len(noteheads) < 2:
+            continue
+
+        positions = [resolve_notehead_wrt_staffline(notehead, node) for notehead in noteheads]
+        positions_not_on_staffline = [p for p in positions if p != 0]
+        unique_positions = set(positions_not_on_staffline)
+        if len(unique_positions) > 1:
+            problem_leger_lines.append(node)
+
+    return problem_leger_lines
+
+
+def find_noteheads_with_leger_line_and_staff_conflict(nodes: List[Node]) -> List[Node]:
+    """Find all noteheads that have a relationship both to a staffline
+    or staffspace and to a leger line.
+
+    Assumes (obviously) that staffline relationships have already been
+    resolved. Useful in a workflow where autoparsing is applied *after*
+    staff inference.
+    """
+    graph = NotationGraph(nodes)
+
+    problem_noteheads = []
+
+    for node in nodes:
+        if node.class_name not in _CONST.NOTEHEAD_CLASS_NAMES:
+            continue
+
+        lls = graph.children(node, [_CONST.LEGER_LINE])
+        staff_objs = graph.children(node, _CONST.STAFFLINE_CLASS_NAMES)
+        if lls and staff_objs:
+            problem_noteheads.append(node)
+
+    return problem_noteheads
+
+
+def find_noteheads_on_staff_linked_to_leger_line(nodes: List[Node]) -> List[Node]:
+    """Find all noteheads that are linked to a leger line,
+    but at the same time intersect a staffline or lie
+    entirely within a staffspace. These should be fixed
+    by linking them to the corresponding staffline/staffspace,
+    but the fixing operation should be in infer_staffline_relationships.
+
+    This is the opposite of what ``resolve_leger_line_or_staffline_object()`` is doing.
+    """
+    graph = NotationGraph(nodes)
+    problem_noteheads = []
+
+    stafflines = sorted([c for c in nodes if c.class_name == 'staff_line'],
+                        key=lambda x: x.top)
+    staffspaces = sorted([c for c in nodes if c.class_name == 'staff_space'],
+                         key=lambda x: x.top)
+
+    for node in nodes:
+        if node.class_name not in _CONST.NOTEHEAD_CLASS_NAMES:
+            continue
+
+        lls = graph.children(node, [_CONST.LEGER_LINE])
+        if len(lls) == 0:
+            continue
+
+        # Intersecting stafflines
+        overlapped_stafflines = []
+        for sl in stafflines:
+            if node.overlaps(sl):
+                overlapped_stafflines.append(sl)
+
+        container_staffspaces = []
+        for ss in staffspaces:
+            if ss.contains(node):
+                container_staffspaces.append(ss)
+
+        if (len(overlapped_stafflines) + len(container_staffspaces)) > 0:
+            problem_noteheads.append(node)
+
+    return problem_noteheads
+
+
+def find_misdirected_leger_line_edges(nodes: List[Node], retain_ll_for_disconnected_noteheads: bool = True) -> \
+        List[List[Node]]:
+    """Finds all edges that connect to leger lines, but do not
+    lead in the direction of the staff.
+
+    Silently assumes that all noteheads are connected to the correct staff.
+
+    :param retain_ll_for_disconnected_noteheads:
+        If the notehead would be left disconnected from all stafflines
+        and staffspaces, retain its edges to its LLs -- it is better
+        to get imperfect inference rather than for the PLAY button to fail.
+    """
+    graph = NotationGraph(nodes)
+
+    misdirected_object_pairs = []
+
+    for node in nodes:
+        if node.class_name not in _CONST.NOTEHEAD_CLASS_NAMES:
+            continue
+
+        lls = graph.children(node, [_CONST.LEGER_LINE])
+        if not lls:
+            continue
+
+        staffs = graph.children(node, [_CONST.STAFF])
+        if not staffs:
+            logging.warning('Notehead {0} not connected to any staff!'.format(node.id))
+            continue
+        staff = staffs[0]
+
+        # Determine whether notehead is above or below staff.
+        # Because of mistakes in notehead-ll edges, can actually be
+        # *on* the staff. (If it is on a staffline, then the edge is
+        # definitely wrong.)
+        stafflines = sorted(graph.children(staff, [_CONST.STAFFLINE]),
+                            key=lambda x: x.top)
+        p_top = resolve_notehead_wrt_staffline(node, stafflines[0])
+        p_bottom = resolve_notehead_wrt_staffline(node, stafflines[-1])
+        # Notehead actually located on the staff somewhere:
+        # all of the LL rels. are false.
+        if (p_top != p_bottom) or (p_top == 0) or (p_bottom == 0):
+            for ll in lls:
+                misdirected_object_pairs.append([node, ll])
+            continue
+
+        notehead_staff_direction = 1
+        if p_bottom == -1:
+            notehead_staff_direction = -1
+
+        _current_misdirected_object_pairs = []
+        for ll in lls:
+            ll_direction = resolve_notehead_wrt_staffline(node, ll)
+            if (ll_direction != 0) and (ll_direction != notehead_staff_direction):
+                misdirected_object_pairs.append([node, ll])
+                _current_misdirected_object_pairs.append([node, ll])
+
+        if retain_ll_for_disconnected_noteheads:
+            staffline_like_children = graph.children(node, class_filter=[_CONST.STAFFLINE,
+                                                                         _CONST.STAFFSPACE,
+                                                                         _CONST.LEGER_LINE])
+            # If all the notehead's links to staffline-like objects are scheduled to be discarded:
+            if len(staffline_like_children) == len(_current_misdirected_object_pairs):
+                # Remove them from the schedule
+                misdirected_object_pairs = misdirected_object_pairs[:-len(_current_misdirected_object_pairs)]
+
+    return misdirected_object_pairs
+
+
+def resolve_leger_line_or_staffline_object(nodes: List[Node]):
+    """If staff relationships are created before notehead to leger line
+    relationships, then there will be noteheads on leger lines that
+    are nevertheless connected to staffspaces. This function should be
+    applied after both staffspace and leger line relationships have been
+    inferred, to guess whether the notehead's relationship to the staff
+    object should be discarded.
+
+    Has no dependence on misdirected edge detection (handles this as a part
+    of the conflict resolution).
+    """
+    graph = NotationGraph(nodes)
+
+    for node in nodes:
+        if node.class_name not in _CONST.NOTEHEAD_CLASS_NAMES:
+            continue
+
+        lls = graph.children(node, [_CONST.LEGER_LINE])
+        stafflines = graph.children(node, _CONST.STAFFLINE_CLASS_NAMES)
+        staff = graph.children(node, _CONST.STAFF)
+
+        if len(lls) == 0:
+            continue
+        if len(stafflines) == 0:
+            continue
+
+        if len(staff) == 0:
+            logging.warning('Notehead {0} not connected to any staff!'
+                            ' Unable to resolve ll/staffline.'.format(node.id))
+            continue
+
+        # Multiple LLs: must check direction
+        # Multiple stafflines: ???
+        if len(stafflines) > 1:
+            logging.warning('Notehead {0} is connected to multiple staffline'
+                            ' objects!'.format(node.id))
+
+
+##############################################################################
+
+def group_by_measure(nodes: List[Node]):
+    """Groups the objects into measures.
+    Assumes the measures are consistent across staffs: no polytempi.
+
+    If there are objects that span multiple measures, they are assigned
+    to all the measures they intersect.
+
+    If no measure separators are found, assumes everything belongs
+    to one measure.
+
+    :returns: A list of Node lists corresponding to measures. The list
+        is ordered left-to-right.
+    """
+    graph = NotationGraph(nodes)
+    logging.debug('Find measure separators.')
+
+    measure_separators = [node for node in nodes if node.class_name in _CONST.MEASURE_SEPARATOR_CLASS_NAMES]
+
+    if len(measure_separators) == 0:
+        return nodes
+
+    logging.debug('Order measure separators by precedence.')
+    # Systems
+    # measure seps. by system
+    measure_separators = sorted(measure_separators, key=lambda m: m.left)
+
+    logging.debug('Denote measure areas: bounding boxes and masks.')
+    logging.debug('Assign objects to measures, based on overlap.')
+
+    raise NotImplementedError()
+
+
+##############################################################################
+# Searching for MuNGOs that are contained within other MuNGOs
+# and removing them safely from the MuNG.
+
+def find_contained_nodes(nodes: List[Node], mask_threshold: float = 0.95):
+    """Find all nodes that are contained within other nodes
+    and not connected by an edge from container to contained.
+
+    Does *NOT* check for transitive edges!"""
+    graph = NotationGraph(nodes)
+
+    # We should have some smarter indexing structure here, but since
+    # we are just checking bounding boxes for candidates first,
+    # it does not matter too much.
+
+    nonstaff_nodes = [node for node in nodes if node.class_name not in _CONST.STAFF_CLASSES]
+
+    contained_nodes = []
+    for c1 in nonstaff_nodes:
+        for c2 in nonstaff_nodes:
+            if c1.id == c2.id:
+                continue
+            if c1.contains(c2):
+                # Check mask overlap
+                r, p, f = c1.compute_recall_precision_fscore_on_mask(c2)
+                if r < mask_threshold:
+                    continue
+                if c2.id in c1.outlinks:
+                    continue
+                contained_nodes.append(c2)
+
+    # Make unique
+    return [c for c in set(contained_nodes)]
+
+
+def remove_contained_nodes(nodes: List[Node], contained: List[Node]) -> List[Node]:
+    """Removes ``contained`` Nodes from ``nodes`` so that the
+    graph takes minimum damage.
+
+    * Attachment edges of contained objects are removed.
+    * For precedence edges, we link all precedence ancestors of a removed node
+      to all its descendants.
+    """
+    # Operating on a copy. Inefficient, but safe.
+    output_nodes = [copy.deepcopy(c) for c in nodes]
+
+    # The nodes are then edited in-place by manipulating
+    # the graph; hence we can then just return output_nodes.
+    graph = NotationGraph(output_nodes)
+    for c in contained:
+        graph.remove_from_precedence(c.id)
+    for c in contained:
+        graph.remove_vertex(c.id)
+
+    return graph.vertices
+
+
+def resolve_notehead_wrt_staffline(notehead, staffline_or_leger_line) -> int:
+    # type: (Node, Node) -> int
+    """Resolves the relative vertical position of the notehead with respect
+    to the given staff_line or legerLine object. Returns -1 if notehead
+    is *below* staffline, 0 if notehead is *on* staffline, and 1 if notehead
+    is *above* staffline."""
+    ll = staffline_or_leger_line
+
+    # Determining whether the notehead is on a leger
+    # line or in the adjacent temp staffspace.
+    # This uses a magic number, ON_STAFFLINE_RATIO_THRESHOLD.
+    output_position = 0
+
+    # Weird situation with notehead vertically *inside* bbox
+    # of leger line (could happen with slanted LLs and very small
+    # noteheads).
+    if ll.top <= notehead.top <= notehead.bottom <= ll.bottom:
+        output_position = 0
+
+    # No vertical overlap between LL and notehead
+    elif ll.top > notehead.bottom:
+        output_position = 1
+    elif notehead.top > ll.bottom:
+        output_position = -1
+
+    # Complicated situations: overlap
+    else:
+        # Notehead "around" leger line.
+        if notehead.top < ll.top <= ll.bottom < notehead.bottom:
+            dtop = ll.top - notehead.top
+            dbottom = notehead.bottom - ll.bottom
+
+            if min(dtop, dbottom) / max(dtop, dbottom) \
+                    < _CONST.ON_STAFFLINE_RATIO_THRESHOLD:
+                if dtop > dbottom:
+                    output_position = 1
+                else:
+                    output_position = -1
+
+        # Notehead interlaced with leger line, notehead on top
+        elif notehead.top < ll.top <= notehead.bottom <= ll.bottom:
+            output_position = 1
+
+        # Notehead interlaced with leger line, leger line on top
+        elif ll.top <= notehead.top <= ll.bottom < notehead.bottom:
+            output_position = -1
+
+        else:
+            logging.warning('Strange notehead {0} vs. leger line {1}'
+                            ' situation: bbox notehead {2}, LL {3}.'
+                            ' Note that the output position is unusable;'
+                            ' pleasre re-do this attachment manually.'
+                            ''.format(notehead.id, ll.id,
+                                      notehead.bounding_box,
+                                      ll.bounding_box))
+    return output_position
+
+
+def is_notehead_on_line(notehead, line) -> bool:
+    # type: (Node, Node) -> bool
+    """Check whether given notehead is positioned on the line object."""
+    if line.class_name not in _CONST.STAFFLINE_LIKE_CLASS_NAMES:
+        raise ValueError('Cannot resolve relative position of notehead'
+                         ' {0} to non-staffline-like object {1}'
+                         ''.format(notehead.id, line.id))
+
+    position = resolve_notehead_wrt_staffline(notehead, line)
+    return position == 0
```

### Comparing `mung-1.1/mung/io.py` & `mung-1.2/mung/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,487 +1,499 @@
-"""This module implements functions for reading and writing the data formats used by MUSCIMA++.
-
-Data formats
-============
-
-All MUSCIMA++ data is stored as XML, in ``<Node>`` elements.
-These are grouped into ``<Nodes>`` elements, which are
-the top-level elements in the ``*.xml`` dataset files.
-
-The list of object classes used in the dataset is also stored as XML,
-in ``<NodeClass>`` elements (within a ``<NodeClasses>``
-element).
-
-Node
-----------
-
-To read a Node list file (in this case, a test data file):
-
-    >>> from mung.io import read_nodes_from_file
-    >>> import os
-    >>> file = os.path.join(os.path.dirname(__file__), '../test/test_data/01_basic.xml')
-    >>> nodes = read_nodes_from_file(file)
-
-The ``Node`` string representation is a XML object::
-
-    <Node xml:id="MUSCIMA-pp_1.0___CVC-MUSCIMA_W-01_N-10_D-ideal___25">
-      <Id>25</Id>
-      <ClassName>grace-notehead-full</ClassName>
-      <Top>119</Top>
-      <Left>413</Left>
-      <Width>16</Width>
-      <Height>6</Height>
-      <Mask>1:5 0:11 (...) 1:4 0:6 1:5 0:1</Mask>
-      <Outlinks>12 24 26</Outlinks>
-      <Inlinks>13</Inlinks>
-    </Node>
-
-The Nodes are themselves kept as a list::
-
-    <Nodes>
-      <Node> ... </Node>
-      <Node> ... </Node>
-    </Nodes>
-
-Parsing is only implemented for files that consist of a single
-``<Nodes>``.
-
-Additional information
-^^^^^^^^^^^^^^^^^^^^^^
-
-.. caution::
-
-    This part may easily be deprecated.
-
-Arbitrary data can be added to the Node using the optional
-``<Data>`` element. It should encode a dictionary of additional
-information about the Node that may only apply to a subset
-of Nodes (this facultativeness is what distinguishes the
-purpose of the ``<Data>`` element from just subclassing ``Node``).
-
-For example, encoding the pitch, duration and precedence information
-about a notehead could look like this::
-
-    <Node>
-        ...
-        <Data>
-            <DataItem key="pitch_step" type="str">D</DataItem>
-            <DataItem key="pitch_modification" type="int">1</DataItem>
-            <DataItem key="pitch_octave" type="int">4</DataItem>
-            <DataItem key="midi_pitch_code" type="int">63</DataItem>
-            <DataItem key="midi_duration" type="int">128</DataItem>
-            <DataItem key="precedence_inlinks" type="list[int]">23 24 25</DataItem>
-            <DataItem key="precedence_outlinks" type="list[int]">27</DataItem>
-        </Data>
-    </Node
-
-The ``Node`` will then contain in its ``data`` attribute
-the dictionary::
-
-    self.data = {'pitch_step': 'D',
-                 'pitch_modification': 1,
-                 'pitch_octave': 4,
-                 'midi_pitch_code': 63,
-                 'midi_pitch_duration': 128,
-                 'precedence_inlinks': [23, 24, 25],
-                 'precedence_outlinks': [27]}
-
-
-This is also a basic mechanism to allow you to subclass
-Node with extra attributes without having to re-implement
-parsing and export.
-
-.. warning::
-
-    Do not misuse this! The ``<Data>`` mechanism is primarily
-    intended to encode extra information for MUSCIMarker to
-    display.
-
-
-Individual elements of a ``<Node>``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-* ``<Id>`` is the unique integer ID of the Node inside this document
-* ``<ClassName>`` is the name of the object's class (such as
-  ``noteheadFull``, ``beam``, ``numeral3``, etc.).
-* ``<Top>`` is the vertical coordinate of the upper left corner of the object's
-  bounding box.
-* ``<Left>`` is the horizontal coordinate of the upper left corner of
-  the object's bounding box.
-* ``<Width>``: the amount of rows that the Node spans.
-* ``<Height>``: the amount of columns that the Node spans.
-* ``<Mask>``: a run-length-encoded binary (0/1) array that denotes the area
-  within the Node's bounding box (specified by ``top``, ``left``,
-  ``height`` and ``width``) that the Node actually occupies. If
-  the mask is not given, the object is understood to occupy the entire
-  bounding box. For the representation, see Implementation notes
-  below.
-* ``<Inlinks>``: whitespace-separate ``id`` list, representing Nodes
-  **from** which a relationship leads to this Node. (Relationships are
-  directed edges, forming a directed graph of Nodes.) The ids are
-  valid in the same scope as the Node's ``id``: don't mix
-  Nodes from multiple scopes (e.g., multiple documents)!
-  If you are using Nodes from multiple documents at the same
-  time, make sure to check against the ``unique_id``s.
-* ``<Outlinks>``: whitespace-separate ``id`` list, representing Nodes
-  **to** which a relationship leads to this Node. (Relationships are
-  directed edges, forming a directed graph of Nodes.) The ids are
-  valid in the same scope as the Node's ``id``: don't mix
-  Nodes from multiple scopes (e.g., multiple documents)!
-  If you are using Nodes from multiple documents at the same
-  time, make sure to check against the ``unique_id``s.
-* ``<Data>``: a list of ``<DataItem>`` elements. The elements have
-  two attributes: ``key``, and ``type``. The ``key`` is what the item
-  should be called in the ``data`` dict of the loaded Node.
-  The ``type`` attribute encodes the Python type of the item and gets
-  applied to the text of the ``<DataItem>`` to produce the value.
-  Currently supported types are ``int``, ``float``, and ``str``,
-  and ``list[int]``, ``list[float]`` and ``list[str]``. The lists
-  are whitespace-separated.
-
-The parser function provided for Nodes does *not* check against
-the presence of other elements. You can extend Nodes for your
-own purposes -- but you will have to implement parsing.
-
-Implementation notes on the mask
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-The mask is a numpy array that will be saved using run-length encoding.
-The numpy array is first flattened, then runs of successive 0's and 1's
-are encoded as e.g. ``0:10 `` for a run of 10 zeros.
-
-How much space does this take?
-
-Objects tend to be relatively convex, so after flattening, we can expect
-more or less two runs per row (flattening is done in ``C`` order). Because
-each run takes (approximately) 5 characters, each mask takes roughly ``5 * n_rows``
-bytes to encode. This makes it efficient for objects wider than 5 pixels, with
-a compression ratio approximately ``n_cols / 5``.
-(Also, the numpy array needs to be made C-contiguous for that, which
-explains the `NODE_MASK_ORDER='C'` hack in `set_mask()`.)
-
-
-NodeClass
----------------
-
-This is what a single NodeClass element might look like::
-
-    <NodeClass>
-        <Id>1</Id>
-        <Name>notehead-empty</Name>
-        <GroupName>note-primitive/notehead-empty</GroupName>
-        <Color>#FF7566</Color>
-    </NodeClass>
-
-See e.g. ``test/test_data/mff-muscima-classes-annot.xml``,
-which is incidentally the real NodeClass list used
-for annotating MUSCIMA++.
-
-Similarly to a ``<Nodes>``, the ``<NodeClass>``
-elements are organized inside a ``<NodeClasses>``::
-
-   <NodeClasses>
-      <NodeClass> ... </NodeClass>
-      <NodeClass> ... </NodeClass>
-   </NodeClasses>
-
-The :class:`NodeClass` represents one possible :class:`Node`
-symbol class, such as a notehead or a time signature. Aside from defining
-the "vocabulary" of available object classes for annotation, it also contains
-some information about how objects of the given class should
-be displayed in the MUSCIMarker annotation software (ordering
-related object classes together in menus, implementing a sensible
-color scheme, etc.). There is nothing interesting about this class,
-we pulled it into the ``mung`` package because the object
-grammar (i.e. which relationships are allowed and which are not)
-depends on having NodeClass object as its "vocabulary",
-and you will probably want to manipulate the data somehow based
-on the objects' relationships (like reassembling notes from notation
-primitives: notehead plus stem plus flags...), and the grammar
-file is a reference for doing that.
-
-"""
-import logging
-import os
-
-import collections
-from typing import List, Tuple
-
-from lxml import etree
-
-from mung.node import Node
-from mung.node_class import NodeClass
-
-
-def read_nodes_from_file(filename: str) -> List[Node]:
-    """From a xml file with a Nodes as the top element, parse
-    a list of nodes. (See ``Node`` class documentation
-    for a description of the XMl format.)
-
-    Let's test whether the parsing function works:
-
-    >>> test_data_dir = os.path.join(os.path.dirname(os.path.dirname(__file__)),
-    ...                              'test', 'test_data')
-    >>> file = os.path.join(test_data_dir, '01_basic.xml')
-    >>> nodes = read_nodes_from_file(file)
-    >>> len(nodes)
-    48
-
-    Let's also test the ``data`` attribute:
-    >>> file_with_data = os.path.join(test_data_dir, '01_basic_binary.xml')
-    >>> nodes = read_nodes_from_file(file_with_data)
-    >>> nodes[0].data['pitch_step']
-    'G'
-    >>> nodes[0].data['midi_pitch_code']
-    79
-    >>> nodes[0].data['precedence_outlinks']
-    [8, 17]
-    >>> nodes[0].dataset
-    'testdataset'
-    >>> nodes[0].document
-    '01_basic_binary'
-
-    :returns: A list of ``Node``s.
-    """
-    tree = etree.parse(filename)
-    root = tree.getroot()
-    logging.debug('XML parsed.')
-    nodes = []
-    dataset = root.attrib['dataset']
-    document = root.attrib['document']
-
-    for i, node in enumerate(root.iter('Node')):
-        ######################################################
-        logging.debug('Parsing Node {0}'.format(i))
-
-        node_id = int(float(node.findall('Id')[0].text))
-        class_name = node.findall('ClassName')[0].text
-        top = int(node.findall('Top')[0].text)
-        left = int(node.findall('Left')[0].text)
-        width = int(node.findall('Width')[0].text)
-        height = int(node.findall('Height')[0].text)
-
-        #################################
-        # Parsing the graph structure (Can deal with missing Inlinks/Outlinks)
-        inlinks = []
-        i_s = node.findall('Inlinks')
-        if len(i_s) > 0:
-            i_s_text = node.findall('Inlinks')[0].text
-            if i_s_text is not None:  # Zero-length links
-                inlinks = list(map(int, i_s_text.split(' ')))
-
-        outlinks = []
-        o_s = node.findall('Outlinks')
-        if len(o_s) > 0:
-            o_s_text = node.findall('Outlinks')[0].text
-            if o_s_text is not None:
-                outlinks = list(map(int, o_s_text.split(' ')))
-
-        #################################
-        data = node.findall('Data')
-        data_dict = None
-        if len(data) > 0:
-            data = data[0]
-            data_dict = {}
-            for data_item in data.findall('DataItem'):
-                key = data_item.get('key')
-                value_type = data_item.get('type')
-                value = data_item.text
-
-                # logging.debug('Creating data entry: key={0}, type={1},'
-                #              ' value={2}'.format(key, value_type, value))
-
-                if value_type == 'int':
-                    value = int(value)
-                elif value_type == 'float':
-                    value = float(value)
-                elif value_type.startswith('list'):
-                    if value is None:
-                        value = []
-                    else:
-                        vt_factory = str
-                        if value_type.endswith('[int]'):
-                            vt_factory = int
-                        elif value_type.endswith('[float]'):
-                            vt_factory = float
-                        value = list(map(vt_factory, value.split()))
-
-                data_dict[key] = value
-
-        #################################
-        # Create the object.
-        new_node = Node(id_=node_id,
-                        class_name=class_name,
-                        top=top,
-                        left=left,
-                        width=width,
-                        height=height,
-                        inlinks=inlinks,
-                        outlinks=outlinks,
-                        dataset=dataset,
-                        document=document,
-                        data=data_dict)
-
-        #################################
-        # Add mask.
-        # We do this only after the Node has been created,
-        # to make sure that the width & height used to reshape
-        # the flattened mask reflects what is in the Node.
-        mask = None
-        mask_elements = node.findall('Mask')
-        if len(mask_elements) > 0:
-            mask = Node.decode_mask(mask_elements[0].text, shape=(new_node.height, new_node.width))
-        new_node.set_mask(mask)
-        nodes.append(new_node)
-
-    logging.debug('Nodes loaded.')
-
-    if not validate_nodes_graph_structure(nodes):
-        raise ValueError('Invalid Node graph structure! Check warnings'
-                         ' in log for the individual errors.')
-
-    return nodes
-
-
-def validate_nodes_graph_structure(nodes: List[Node]) -> bool:
-    """Check that the graph defined by the ``inlinks`` and ``outlinks``
-    in the given list of Nodes is valid: no relationships
-    leading from or to objects with non-existent ``id``s.
-
-    Can deal with ``Nodes`` coming from a combination
-    of documents, through the Node ``document`` property.
-    Warns about documents which are found inconsistent.
-
-    :param nodes: A list of :class:`Node` instances.
-
-    :returns: ``True`` if graph is valid, ``False`` otherwise.
-    """
-    # Split into lists by document
-    nodes_by_document = collections.defaultdict(list)
-    for node in nodes:
-        nodes_by_document[node.document].append(node)
-
-    is_valid = True
-    for doc, document_nodes in list(nodes_by_document.items()):
-        document_is_valid = validate_document_graph_structure(document_nodes)
-        if not document_is_valid:
-            logging.warning('Document {0} has invalid Node graph!'.format(doc))
-            is_valid = False
-    return is_valid
-
-
-def validate_document_graph_structure(nodes: List[Node]) -> bool:
-    """Check that the graph defined by the ``inlinks`` and ``outlinks``
-    in the given list of Nodes is valid: no relationships
-    leading from or to objects with non-existent ``id``s.
-
-    Checks that all the Nodes come from one document. (Raises
-    a ``ValueError`` otherwise.)
-
-    :param nodes: A list of :class:`Node` instances.
-
-    :returns: ``True`` if graph is valid, ``False`` otherwise.
-    """
-    docs = [node.document for node in nodes]
-    if len(set(docs)) != 1:
-        raise ValueError('Got Nodes from multiple documents!')
-
-    is_valid = True
-    node_ids = frozenset([node.id for node in nodes])
-    for c in nodes:
-        inlinks = c.inlinks
-        for i in inlinks:
-            if i not in node_ids:
-                logging.warning('Invalid graph structure in NodeList:'
-                                ' object {0} has inlink from non-existent'
-                                ' object {1}'.format(c, i))
-                is_valid = False
-
-        outlinks = c.outlinks
-        for o in outlinks:
-            if o not in node_ids:
-                logging.warning('Invalid graph structure in NodeList:'
-                                ' object {0} has outlink to non-existent'
-                                ' object {1}'.format(c, o))
-                is_valid = False
-
-    return is_valid
-
-
-def get_edges(nodes: List[Node], validate: bool = True) -> List[Tuple[int, int]]:
-    """Collects the inlink/outlink Node graph
-    and returns it as a list of ``(from, to)`` edges.
-
-    :param nodes: A list of Node instances.
-        All are expected to be within one document.
-
-    :param validate: If set, will raise a ValueError
-        if the graph defined by the Nodes is
-        invalid.
-
-    :returns: A list of ``(from, to)`` id pairs
-        that represent edges in the Node graph.
-    """
-    if validate:
-        validate_nodes_graph_structure(nodes)
-
-    edges = []
-    for c in nodes:
-        for o in c.outlinks:
-            edges.append((c.id, o))
-    return edges
-
-
-def export_node_list(nodes: List[Node], document: str = None, dataset: str = None) -> str:
-    """Writes the Node data as a XML string. Does not write
-    to a file -- use ``with open(output_file) as out_stream:`` etc.
-
-    """
-    # This is the data string, the rest is formalities
-    nodes_string = '\n'.join([str(c) for c in nodes])
-
-    lines = list()
-    lines.append('<?xml version="1.0" encoding="utf-8"?>')
-    lines.append('<Nodes dataset={0} document={1}'
-                 ' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"'
-                 ' xmlns:xsd="http://www.w3.org/2001/XMLSchema"'
-                 ' xsi:noNamespaceSchemaLocation="CVC-MUSCIMA_Schema.xsd">'.format(dataset, document))
-    lines.append(nodes_string)
-    lines.append('</Nodes>')
-    return '\n'.join(lines)
-
-
-##############################################################################
-# Parsing NodeClass lists, mostly for grammars.
-
-def parse_node_classes(filename: str) -> List[NodeClass]:
-    """ Extract the list of :class:`NodeClass` objects from
-        an xml file with a NodeClasses as the top element and NodeClass children.
-    """
-    tree = etree.parse(filename)
-    node_classes_xml = tree.getroot()
-    node_classes = []
-    for node_class_xml in node_classes_xml:
-        if node_class_xml.tag != "NodeClass":
-            continue
-        node_class = NodeClass(class_id=int(node_class_xml.findall('Id')[0].text),
-                               name=node_class_xml.findall('Name')[0].text,
-                               group_name=node_class_xml.findall('GroupName')[0].text,
-                               color=node_class_xml.findall('Color')[0].text)
-        node_classes.append(node_class)
-    return node_classes
-
-
-def export_nodeclass_list(node_classes: List[NodeClass]) -> str:
-    """Writes the Node data as a XML string. Does not write
-    to a file -- use ``with open(output_file) as out_stream:`` etc.
-    """
-    # This is the data string, the rest is formalities
-    node_classes_string = '\n'.join([str(c) for c in node_classes])
-
-    lines = list()
-
-    lines.append('<?xml version="1.0" encoding="utf-8"?>')
-    lines.append('<NodeClasses noNamespaceSchema="mff-muscima-mlclasses.xsd">')
-    lines.append(node_classes_string)
-    lines.append('</NodeClasses>')
-    return '\n'.join(lines)
+"""This module implements functions for reading and writing the data formats used by MUSCIMA++.
+
+Data formats
+============
+
+All MUSCIMA++ data is stored as XML, in ``<Node>`` elements.
+These are grouped into ``<Nodes>`` elements, which are
+the top-level elements in the ``*.xml`` dataset files.
+
+The list of object classes used in the dataset is also stored as XML,
+in ``<NodeClass>`` elements (within a ``<NodeClasses>``
+element).
+
+Node
+----------
+
+To read a Node list file (in this case, a test data file):
+
+    >>> from mung.io import read_nodes_from_file
+    >>> import os
+    >>> file = os.path.join(os.path.dirname(__file__), '../test/test_data/01_basic.xml')
+    >>> nodes = read_nodes_from_file(file)
+
+The ``Node`` string representation is a XML object::
+
+    <Node xml:id="MUSCIMA-pp_1.0___CVC-MUSCIMA_W-01_N-10_D-ideal___25">
+      <Id>25</Id>
+      <ClassName>grace-notehead-full</ClassName>
+      <Top>119</Top>
+      <Left>413</Left>
+      <Width>16</Width>
+      <Height>6</Height>
+      <Mask>1:5 0:11 (...) 1:4 0:6 1:5 0:1</Mask>
+      <Outlinks>12 24 26</Outlinks>
+      <Inlinks>13</Inlinks>
+    </Node>
+
+The Nodes are themselves kept as a list::
+
+    <Nodes>
+      <Node> ... </Node>
+      <Node> ... </Node>
+    </Nodes>
+
+Parsing is only implemented for files that consist of a single
+``<Nodes>``.
+
+Additional information
+^^^^^^^^^^^^^^^^^^^^^^
+
+.. caution::
+
+    This part may easily be deprecated.
+
+Arbitrary data can be added to the Node using the optional
+``<Data>`` element. It should encode a dictionary of additional
+information about the Node that may only apply to a subset
+of Nodes (this facultativeness is what distinguishes the
+purpose of the ``<Data>`` element from just subclassing ``Node``).
+
+For example, encoding the pitch, duration and precedence information
+about a notehead could look like this::
+
+    <Node>
+        ...
+        <Data>
+            <DataItem key="pitch_step" type="str">D</DataItem>
+            <DataItem key="pitch_modification" type="int">1</DataItem>
+            <DataItem key="pitch_octave" type="int">4</DataItem>
+            <DataItem key="midi_pitch_code" type="int">63</DataItem>
+            <DataItem key="midi_duration" type="int">128</DataItem>
+            <DataItem key="precedence_inlinks" type="list[int]">23 24 25</DataItem>
+            <DataItem key="precedence_outlinks" type="list[int]">27</DataItem>
+        </Data>
+    </Node
+
+The ``Node`` will then contain in its ``data`` attribute
+the dictionary::
+
+    self.data = {'pitch_step': 'D',
+                 'pitch_modification': 1,
+                 'pitch_octave': 4,
+                 'midi_pitch_code': 63,
+                 'midi_pitch_duration': 128,
+                 'precedence_inlinks': [23, 24, 25],
+                 'precedence_outlinks': [27]}
+
+
+This is also a basic mechanism to allow you to subclass
+Node with extra attributes without having to re-implement
+parsing and export.
+
+.. warning::
+
+    Do not misuse this! The ``<Data>`` mechanism is primarily
+    intended to encode extra information for MUSCIMarker to
+    display.
+
+
+Individual elements of a ``<Node>``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+* ``<Id>`` is the unique integer ID of the Node inside this document
+* ``<ClassName>`` is the name of the object's class (such as
+  ``noteheadFull``, ``beam``, ``numeral3``, etc.).
+* ``<Top>`` is the vertical coordinate of the upper left corner of the object's
+  bounding box.
+* ``<Left>`` is the horizontal coordinate of the upper left corner of
+  the object's bounding box.
+* ``<Width>``: the amount of rows that the Node spans.
+* ``<Height>``: the amount of columns that the Node spans.
+* ``<Mask>``: a run-length-encoded binary (0/1) array that denotes the area
+  within the Node's bounding box (specified by ``top``, ``left``,
+  ``height`` and ``width``) that the Node actually occupies. If
+  the mask is not given, the object is understood to occupy the entire
+  bounding box. For the representation, see Implementation notes
+  below.
+* ``<Inlinks>``: whitespace-separate ``id`` list, representing Nodes
+  **from** which a relationship leads to this Node. (Relationships are
+  directed edges, forming a directed graph of Nodes.) The ids are
+  valid in the same scope as the Node's ``id``: don't mix
+  Nodes from multiple scopes (e.g., multiple documents)!
+  If you are using Nodes from multiple documents at the same
+  time, make sure to check against the ``unique_id``s.
+* ``<Outlinks>``: whitespace-separate ``id`` list, representing Nodes
+  **to** which a relationship leads to this Node. (Relationships are
+  directed edges, forming a directed graph of Nodes.) The ids are
+  valid in the same scope as the Node's ``id``: don't mix
+  Nodes from multiple scopes (e.g., multiple documents)!
+  If you are using Nodes from multiple documents at the same
+  time, make sure to check against the ``unique_id``s.
+* ``<Data>``: a list of ``<DataItem>`` elements. The elements have
+  two attributes: ``key``, and ``type``. The ``key`` is what the item
+  should be called in the ``data`` dict of the loaded Node.
+  The ``type`` attribute encodes the Python type of the item and gets
+  applied to the text of the ``<DataItem>`` to produce the value.
+  Currently supported types are ``int``, ``float``, and ``str``,
+  and ``list[int]``, ``list[float]`` and ``list[str]``. The lists
+  are whitespace-separated.
+
+The parser function provided for Nodes does *not* check against
+the presence of other elements. You can extend Nodes for your
+own purposes -- but you will have to implement parsing.
+
+Implementation notes on the mask
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+The mask is a numpy array that will be saved using run-length encoding.
+The numpy array is first flattened, then runs of successive 0's and 1's
+are encoded as e.g. ``0:10 `` for a run of 10 zeros.
+
+How much space does this take?
+
+Objects tend to be relatively convex, so after flattening, we can expect
+more or less two runs per row (flattening is done in ``C`` order). Because
+each run takes (approximately) 5 characters, each mask takes roughly ``5 * n_rows``
+bytes to encode. This makes it efficient for objects wider than 5 pixels, with
+a compression ratio approximately ``n_cols / 5``.
+(Also, the numpy array needs to be made C-contiguous for that, which
+explains the `NODE_MASK_ORDER='C'` hack in `set_mask()`.)
+
+
+NodeClass
+---------------
+
+This is what a single NodeClass element might look like::
+
+    <NodeClass>
+        <Id>1</Id>
+        <Name>notehead-empty</Name>
+        <GroupName>note-primitive/notehead-empty</GroupName>
+        <Color>#FF7566</Color>
+    </NodeClass>
+
+See e.g. ``test/test_data/mff-muscima-classes-annot.xml``,
+which is incidentally the real NodeClass list used
+for annotating MUSCIMA++.
+
+Similarly to a ``<Nodes>``, the ``<NodeClass>``
+elements are organized inside a ``<NodeClasses>``::
+
+   <NodeClasses>
+      <NodeClass> ... </NodeClass>
+      <NodeClass> ... </NodeClass>
+   </NodeClasses>
+
+The :class:`NodeClass` represents one possible :class:`Node`
+symbol class, such as a notehead or a time signature. Aside from defining
+the "vocabulary" of available object classes for annotation, it also contains
+some information about how objects of the given class should
+be displayed in the MUSCIMarker annotation software (ordering
+related object classes together in menus, implementing a sensible
+color scheme, etc.). There is nothing interesting about this class,
+we pulled it into the ``mung`` package because the object
+grammar (i.e. which relationships are allowed and which are not)
+depends on having NodeClass object as its "vocabulary",
+and you will probably want to manipulate the data somehow based
+on the objects' relationships (like reassembling notes from notation
+primitives: notehead plus stem plus flags...), and the grammar
+file is a reference for doing that.
+
+"""
+import logging
+import os
+
+import collections
+from typing import List, Tuple
+
+from lxml import etree
+
+from mung.node import Node
+from mung.node_class import NodeClass
+
+
+def read_nodes_from_file(filename: str) -> List[Node]:
+    """From a xml file with a Nodes as the top element, parse
+    a list of nodes. (See ``Node`` class documentation
+    for a description of the XMl format.)
+
+    Let's test whether the parsing function works:
+
+    >>> test_data_dir = os.path.join(os.path.dirname(os.path.dirname(__file__)),
+    ...                              'test', 'test_data')
+    >>> file = os.path.join(test_data_dir, '01_basic.xml')
+    >>> nodes = read_nodes_from_file(file)
+    >>> len(nodes)
+    48
+
+    Let's also test the ``data`` attribute:
+    >>> file_with_data = os.path.join(test_data_dir, '01_basic_binary_2.0.xml')
+    >>> nodes = read_nodes_from_file(file_with_data)
+    >>> nodes[0].data['pitch_step']
+    'G'
+    >>> nodes[0].data['midi_pitch_code']
+    79
+    >>> nodes[0].data['precedence_outlinks']
+    [8, 17]
+    >>> nodes[0].dataset
+    'MUSCIMA-pp_2.0'
+    >>> nodes[0].document
+    '01_basic_binary'
+
+    :returns: A list of ``Node``s.
+    """
+    if not os.path.exists(filename):
+        print("Could not find {0} on disk. Absolute path: {1}".format(filename, os.path.abspath(filename)))
+        return None
+
+    tree = etree.parse(filename)
+    root = tree.getroot()
+    logging.debug('XML parsed.')
+    nodes = []
+    dataset = root.attrib['dataset']
+    document = root.attrib['document']
+
+    for i, node in enumerate(root.iter('Node')):
+        ######################################################
+        logging.debug('Parsing Node {0}'.format(i))
+
+        node_id = int(float(node.findall('Id')[0].text))
+        class_name = node.findall('ClassName')[0].text
+        top = int(node.findall('Top')[0].text)
+        left = int(node.findall('Left')[0].text)
+        width = int(node.findall('Width')[0].text)
+        height = int(node.findall('Height')[0].text)
+
+        #################################
+        # Parsing the graph structure (Can deal with missing Inlinks/Outlinks)
+        inlinks = []
+        i_s = node.findall('Inlinks')
+        if len(i_s) > 0:
+            i_s_text = node.findall('Inlinks')[0].text
+            if i_s_text is not None:  # Zero-length links
+                inlinks = list(map(int, i_s_text.split(' ')))
+
+        outlinks = []
+        o_s = node.findall('Outlinks')
+        if len(o_s) > 0:
+            o_s_text = node.findall('Outlinks')[0].text
+            if o_s_text is not None:
+                outlinks = list(map(int, o_s_text.split(' ')))
+
+        #################################
+        data = node.findall('Data')
+        data_dict = None
+        if len(data) > 0:
+            data = data[0]
+            data_dict = {}
+            for data_item in data.findall('DataItem'):
+                key = data_item.get('key')
+                value_type = data_item.get('type')
+                value = data_item.text
+
+                # logging.debug('Creating data entry: key={0}, type={1},'
+                #              ' value={2}'.format(key, value_type, value))
+
+                if value_type == 'int':
+                    value = int(value)
+                elif value_type == 'float':
+                    value = float(value)
+                elif value_type.startswith('list'):
+                    if value is None:
+                        value = []
+                    else:
+                        vt_factory = str
+                        if value_type.endswith('[int]'):
+                            vt_factory = int
+                        elif value_type.endswith('[float]'):
+                            vt_factory = float
+                        value = list(map(vt_factory, value.split()))
+
+                data_dict[key] = value
+
+        #################################
+        # Create the object.
+        new_node = Node(id_=node_id,
+                        class_name=class_name,
+                        top=top,
+                        left=left,
+                        width=width,
+                        height=height,
+                        inlinks=inlinks,
+                        outlinks=outlinks,
+                        dataset=dataset,
+                        document=document,
+                        data=data_dict)
+
+        #################################
+        # Add mask.
+        # We do this only after the Node has been created,
+        # to make sure that the width & height used to reshape
+        # the flattened mask reflects what is in the Node.
+        mask = None
+        mask_elements = node.findall('Mask')
+        if len(mask_elements) > 0:
+            mask = Node.decode_mask(mask_elements[0].text, shape=(new_node.height, new_node.width))
+        new_node.set_mask(mask)
+        nodes.append(new_node)
+
+    logging.debug('Nodes loaded.')
+
+    if not validate_nodes_graph_structure(nodes):
+        raise ValueError('Invalid Node graph structure! Check warnings'
+                         ' in log for the individual errors.')
+
+    return nodes
+
+
+def validate_nodes_graph_structure(nodes: List[Node]) -> bool:
+    """Check that the graph defined by the ``inlinks`` and ``outlinks``
+    in the given list of Nodes is valid: no relationships
+    leading from or to objects with non-existent ``id``s.
+
+    Can deal with ``Nodes`` coming from a combination
+    of documents, through the Node ``document`` property.
+    Warns about documents which are found inconsistent.
+
+    :param nodes: A list of :class:`Node` instances.
+
+    :returns: ``True`` if graph is valid, ``False`` otherwise.
+    """
+    # Split into lists by document
+    nodes_by_document = collections.defaultdict(list)
+    for node in nodes:
+        nodes_by_document[node.document].append(node)
+
+    is_valid = True
+    for doc, document_nodes in list(nodes_by_document.items()):
+        document_is_valid = validate_document_graph_structure(document_nodes)
+        if not document_is_valid:
+            logging.warning('Document {0} has invalid Node graph!'.format(doc))
+            is_valid = False
+    return is_valid
+
+
+def validate_document_graph_structure(nodes: List[Node]) -> bool:
+    """Check that the graph defined by the ``inlinks`` and ``outlinks``
+    in the given list of Nodes is valid: no relationships
+    leading from or to objects with non-existent ``id``s.
+
+    Checks that all the Nodes come from one document. (Raises
+    a ``ValueError`` otherwise.)
+
+    :param nodes: A list of :class:`Node` instances.
+
+    :returns: ``True`` if graph is valid, ``False`` otherwise.
+    """
+    docs = [node.document for node in nodes]
+    if len(set(docs)) != 1:
+        raise ValueError('Got Nodes from multiple documents!')
+
+    is_valid = True
+    node_ids = frozenset([node.id for node in nodes])
+    for c in nodes:
+        inlinks = c.inlinks
+        for i in inlinks:
+            if i not in node_ids:
+                logging.warning('Invalid graph structure in NodeList:'
+                                ' object {0} has inlink from non-existent'
+                                ' object {1}'.format(c, i))
+                is_valid = False
+
+        outlinks = c.outlinks
+        for o in outlinks:
+            if o not in node_ids:
+                logging.warning('Invalid graph structure in NodeList:'
+                                ' object {0} has outlink to non-existent'
+                                ' object {1}'.format(c, o))
+                is_valid = False
+
+    return is_valid
+
+
+def get_edges(nodes: List[Node], validate: bool = True) -> List[Tuple[int, int]]:
+    """Collects the inlink/outlink Node graph
+    and returns it as a list of ``(from, to)`` edges.
+
+    :param nodes: A list of Node instances.
+        All are expected to be within one document.
+
+    :param validate: If set, will raise a ValueError
+        if the graph defined by the Nodes is
+        invalid.
+
+    :returns: A list of ``(from, to)`` id pairs
+        that represent edges in the Node graph.
+    """
+    if validate:
+        validate_nodes_graph_structure(nodes)
+
+    edges = []
+    for c in nodes:
+        for o in c.outlinks:
+            edges.append((c.id, o))
+    return edges
+
+
+def write_nodes_to_file(nodes: List[Node], file_path: str, document: str = None, dataset: str = None) -> None:
+    output = write_nodes_to_string(nodes, document, dataset)
+    os.makedirs(os.path.dirname(file_path), exist_ok=True)
+    with open(file_path, mode="w") as output_file:
+        output_file.write(output)
+
+
+def write_nodes_to_string(nodes: List[Node], document: str = None, dataset: str = None) -> str:
+    """Writes the Node data as an XML string. Does not write
+    to a file -- use ``write_nodes_to_file`` if you want that behavior.
+
+    """
+    # This is the data string, the rest is formalities
+    nodes_string = '\n'.join([str(c) for c in nodes])
+
+    lines = list()
+    lines.append('<?xml version="1.0" encoding="utf-8"?>')
+    lines.append('<Nodes dataset="{0}" document="{1}"'
+                 ' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"'
+                 ' xsi:noNamespaceSchemaLocation="CVC-MUSCIMA_Schema.xsd">'.format(dataset, document))
+    lines.append(nodes_string)
+    lines.append('</Nodes>')
+    return '\n'.join(lines)
+
+# For compatibility reasons, keep the old name, even though write_nodes_to_file matches read_nodes_from_file better
+export_node_list = write_nodes_to_file
+
+##############################################################################
+# Parsing NodeClass lists, mostly for grammars.
+
+def parse_node_classes(filename: str) -> List[NodeClass]:
+    """ Extract the list of :class:`NodeClass` objects from
+        an xml file with a NodeClasses as the top element and NodeClass children.
+    """
+    tree = etree.parse(filename)
+    node_classes_xml = tree.getroot()
+    node_classes = []
+    for node_class_xml in node_classes_xml:
+        if node_class_xml.tag != "NodeClass":
+            continue
+        node_class = NodeClass(class_id=int(node_class_xml.findall('Id')[0].text),
+                               name=node_class_xml.findall('Name')[0].text,
+                               group_name=node_class_xml.findall('GroupName')[0].text,
+                               color=node_class_xml.findall('Color')[0].text)
+        node_classes.append(node_class)
+    return node_classes
+
+
+def export_nodeclass_list(node_classes: List[NodeClass]) -> str:
+    """Writes the Node data as a XML string. Does not write
+    to a file -- use ``with open(output_file) as out_stream:`` etc.
+    """
+    # This is the data string, the rest is formalities
+    node_classes_string = '\n'.join([str(c) for c in node_classes])
+
+    lines = list()
+
+    lines.append('<?xml version="1.0" encoding="utf-8"?>')
+    lines.append('<NodeClasses noNamespaceSchema="mff-muscima-mlclasses.xsd">')
+    lines.append(node_classes_string)
+    lines.append('</NodeClasses>')
+    return '\n'.join(lines)
```

### Comparing `mung-1.1/mung/mungmatcher.py` & `mung-1.2/mung/mungmatcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,268 +1,270 @@
-import collections
-import copy
-
-from typing import List, Dict, Tuple, Iterable, Any
-
-from mung.constants import InferenceEngineConstants as _CONST
-from mung.graph import NotationGraph
-from mung.node import Node
-
-
-class MungMatcher(object):
-    """The MungMatcher class takes two MuNG notation graphs
-    and outputs an optimal mapping between the graphs.
-
-    It relies on the semantics being present.
-    """
-
-    def run(self, g1: NotationGraph, g2: NotationGraph):
-        """Runs the MuNG graph matching algorithm.
-
-        Assumes noteheads have pitches, durations and onsets filled in.
-        Assumes the input graphs are nearly equal. (So far, we're only
-        trying to match two graphs of the same music.)
-
-        :param g1: The first NotationGraph.
-
-        :param g2: The second NotationGraph.
-
-        :return: A dict of ``(n1.id, n2.id) --> weight``.
-        """
-        # Starts from noteheads with onset/pitch/duration.
-        noteheads_1 = self.collect_fully_defined_noteheads(g1)
-        noteheads_2 = self.collect_fully_defined_noteheads(g2)
-
-        # Matching data structure: dict with id tuples as keys, weights as values.
-        # Currently, weights will only be 1 (zero weights are not in the dict).
-        initial_matching = self.match_fully_defined_noteheads(noteheads_1, noteheads_2)
-        _matched_prev = copy.deepcopy(set(initial_matching.keys()))
-
-        print('Initialized matching: {0} noteheads, running growth iterations.'
-              ''.format(len(_matched_prev)))
-        partial_matching = self.grow_iteration(g1, g2, initial_matching)
-        # Add debugprints!
-        print('First growth iteration done.')
-        _n_iters = 1
-        while _matched_prev != set(partial_matching.keys()):
-            _matched_prev = set(partial_matching.keys())
-
-            partial_matching = self.grow_iteration(g1, g2, partial_matching)
-            _n_iters += 1
-            print('Growth iterations: {0}'.format(_n_iters))
-
-        return partial_matching
-
-    def grow_iteration(self, g1: NotationGraph, g2: NotationGraph, matching: Dict[Tuple[int, int], float]) -> \
-            Dict[Tuple[int, int], float]:
-        """One iteration of graph isomorphism growing.
-        Algorithm:
-
-        1. Connectivity signature matching
-
-        * For both graphs:
-            * For each vertex:
-                * Find connectivity signature to already matched vertices
-
-        * For each vertex u_i in g1 with non-empty connectivity signature:
-            * For each vertex v_j in g2 of the same class as u_i:
-                * If their connectivity signatures match, add them to potential
-                  matches pool. (Will then resolve ties.)
-
-        2. Within pools that share connectivity signatures:
-
-        This is what we want to resolve with EMD. Note that these groups will be
-        fairly small - at most 4 or 5 flags/beams or leger lines.
-
-        """
-        # TODO: factorize compatibility sets by object class!
-        anchor_mapping_1_to_2 = {k[0]: k[1] for k in matching.keys()}
-
-        csigs_1 = self.compute_connectivity_signatures(g1, anchors=[g1[k[0]] for k in matching.keys()])
-        csigs_2 = self.compute_connectivity_signatures(g2, anchors=[g2[k[1]] for k in matching.keys()])
-
-        # csigs contains for each vertex with a non-empty connectivity signature
-        # to the current anchors the list of anchor point outlinks and inlinks.
-
-        inverse_csigs_1 = collections.defaultdict(list)
-        for v1_objid in csigs_1:
-            inverse_csigs_1[csigs_1[v1_objid]].append(v1_objid)
-
-        inverse_csigs_2 = collections.defaultdict(list)
-        for v2_objid in csigs_2:
-            inverse_csigs_2[csigs_2[v2_objid]].append(v2_objid)
-
-        # We will keep the index of match-able vertices indexed
-        # by their connectivity signature w.r.t g2, so we project
-        # the connectivity signature from g1 through the anchor
-        # mapping.
-
-        # The compatible sets are a dict keyed by the corresponding csig_2.
-        # The values are tuples of lists: first list for a given csig_2
-        # contains the compatible vertices from graph 1, the second list
-        # contains compatible vertices from graph 2.
-        compatible_sets = collections.defaultdict(tuple)
-
-        for v1_objid, csig_1 in csigs_1.items():
-            inlinks, outlinks = csig_1
-            iso_inlinks = tuple([anchor_mapping_1_to_2[i] for i in inlinks])
-            iso_outlinks = tuple([anchor_mapping_1_to_2[i] for i in outlinks])
-            iso_csig = (iso_inlinks, iso_outlinks)
-
-            if iso_csig in inverse_csigs_2:
-                if iso_csig not in compatible_sets:
-                    compatible_sets[iso_csig] = [[], []]
-
-                compatible_sets[iso_csig][0].append(v1_objid)
-                for v2_objid in inverse_csigs_2[iso_csig]:
-                    if v2_objid not in compatible_sets[iso_csig][1]:
-                        compatible_sets[iso_csig][1].append(v2_objid)
-
-        output_matching = copy.deepcopy(matching)
-
-        # Now that we have the compatible sets, we resolve those that are
-        # larger than one.
-        for csig_2 in compatible_sets:
-            compatible_set_objids = compatible_sets[csig_2]
-            compatible_vertices_1 = [g1[node_id]
-                                     for node_id in compatible_set_objids[0]]
-            compatible_vertices_2 = [g2[node_id]
-                                     for node_id in compatible_set_objids[1]]
-            cset_matching = self.resolve_compatible_set_matching(compatible_vertices_1, compatible_vertices_2)
-            # Update output matching dict
-            output_matching.update(cset_matching)
-
-        return output_matching
-
-    def resolve_compatible_set_matching(self, vs1: List[Node], vs2: List[Node]) -> Dict[Tuple[int, int], float]:
-        """Given two sets of vertices that have isomorphic
-        connectivity signatures, resolves how they should actually
-        be matched against each other.
-
-        :param vs1: A list of Nodes.
-
-        :param vs2: A list of Nodes.
-
-        :return: A matching of these two Node lists. The matching
-            is a dict of ``(n1.id, n2.id) --> weight``.
-        """
-        output = {}
-
-        class_names = set([c.class_name for c in vs1 + vs2])
-
-        for class_name in class_names:
-            vs1_by_class = [c for c in vs1 if c.class_name == class_name]
-            vs2_by_class = [c for c in vs2 if c.class_name == class_name]
-
-            for v1, v2 in zip(sorted(vs1_by_class, key=lambda x: x.top),
-                              sorted(vs2_by_class, key=lambda y: y.top)):
-                output[(v1.id, v2.id)] = 1.0
-        return output
-
-    def compute_connectivity_signatures(self, g: NotationGraph, anchors: Iterable[Node]) -> \
-            Dict[int, Tuple[Tuple[int, ...], Tuple[int, ...]]]:
-        """Computes connectivity signatures for vertices in ``g`` to the given
-        ``anchors``.
-
-        :returns: Connectivity signature dict: ``v.id --> (inlinks_tuple, outlinks_tuple)``
-        """
-        output = dict()
-        anchor_set = set(anchors)
-        for c in g.vertices:
-            if c.id in anchor_set:
-                continue
-            anchor_outlinks = tuple([o for o in c.outlinks if o in anchor_set])
-            anchor_inlinks = tuple([i for i in c.inlinks if i in anchor_set])
-            if len(anchor_inlinks) + len(anchor_outlinks) > 0:
-                csig = (anchor_inlinks, anchor_outlinks)
-                output[c.id] = csig
-        return output
-
-    def collect_fully_defined_noteheads(self, graph: NotationGraph) -> List[Node]:
-        return [c for c in graph.vertices if self.__is_fully_defined_notehead(c)]
-
-    @staticmethod
-    def __is_fully_defined_notehead(node: Node) -> bool:
-        isdef = False
-        if (node.class_name in _CONST.NONGRACE_NOTEHEAD_CLASS_NAMES) \
-                and ('onset_beats' in node.data) \
-                and ('midi_pitch_code' in node.data):
-            isdef = True
-        return isdef
-
-    @staticmethod
-    def _notehead_signature(c: Node) -> Tuple[Any, Any, Any]:
-        return c.data['onset_beats'], c.data['midi_pitch_code'], c.data['duration_beats']
-
-    def match_fully_defined_noteheads(self, noteheads_1: List[Node], noteheads_2: List[Node]) -> \
-            Dict[Tuple[int, int], float]:
-        """Matches two lists of fully defined noteheads. Only matches those
-        that exactly share pitch, duration, and onset.
-
-        :returns: A matching: dict of ``(n1.id, n2.id) --> weight``.
-        """
-        output = {}
-        if (len(noteheads_1) == 0) or (len(noteheads_2) == 0):
-            return output
-
-        # Sort & slide algorithm makes this linear, not quadratic.
-        # With more than 500 noteheads, this starts to be felt.
-        ns1 = sorted(noteheads_1, key=lambda x: self._notehead_signature(x))
-        ns2 = sorted(noteheads_2, key=lambda x: self._notehead_signature(x))
-
-        j = 0
-        for n1 in ns1:
-            onset_1 = n1.data['onset_beats']
-
-            n2 = ns2[j]
-            # Make ns2 pointer catch up with the current note
-            while onset_1 > n2.data['onset_beats']:
-                j += 1
-                if j >= len(ns2):
-                    # We will not match anything anymore: noteheads_2 are exhausted.
-                    return output
-                n2 = ns2[j]
-
-            if onset_1 == n2.data['onset_beats']:
-                if self._notehead_signature(n1) == self._notehead_signature(n2):
-                    output[(n1.id, n2.id)] = 1.0
-                    j += 1
-                    continue
-
-            elif onset_1 < n2.data['onset_beats']:
-                continue
-
-        return output
-
-
-if __name__ == '__main__':
-    import os
-    from mung.io import read_nodes_from_file
-    from mung.graph import NotationGraph, NotationGraph, NotationGraph, NotationGraph
-
-    test_data_root = os.path.join(os.path.dirname(os.path.abspath(__file__)),
-                                  '..', 'test',
-                                  'test_data',
-                                  'mungmatcher')
-    gt_root = os.path.join(test_data_root, 'gt')
-    de_root = os.path.join(test_data_root, 'detected')
-    wc_root = os.path.join(test_data_root, 'without_contained')
-
-    names = ['minifull.xml',
-             'mini2full.xml']
-
-    gt = NotationGraph(read_nodes_from_file(os.path.join(test_data_root, names[0])))
-    wc = NotationGraph(read_nodes_from_file(os.path.join(test_data_root, names[1])))
-
-    matcher = MungMatcher()
-
-    aln = matcher.run(gt, gt)
-    print('Matched GT against GT: {} gt, {} gt, {} matched'
-          ''.format(len(gt), len(gt), len(aln)))
-
-    aln = matcher.run(gt, wc)
-    print('Matched GT against WC: {} gt, {} wc, {} matched'
-          ''.format(len(gt), len(wc), len(aln)))
-
-    aln = matcher.run(gt, gt)
-    print('Matched WC against WC: {} wc, {} wc, {} matched'
-          ''.format(len(wc), len(wc), len(aln)))
+import collections
+import copy
+
+from typing import List, Dict, Tuple, Iterable, Any
+
+from mung.constants import InferenceEngineConstants
+from mung.graph import NotationGraph
+from mung.node import Node
+
+_CONST = InferenceEngineConstants()
+
+
+class MungMatcher(object):
+    """The MungMatcher class takes two MuNG notation graphs
+    and outputs an optimal mapping between the graphs.
+
+    It relies on the semantics being present.
+    """
+
+    def run(self, g1: NotationGraph, g2: NotationGraph):
+        """Runs the MuNG graph matching algorithm.
+
+        Assumes noteheads have pitches, durations and onsets filled in.
+        Assumes the input graphs are nearly equal. (So far, we're only
+        trying to match two graphs of the same music.)
+
+        :param g1: The first NotationGraph.
+
+        :param g2: The second NotationGraph.
+
+        :return: A dict of ``(n1.id, n2.id) --> weight``.
+        """
+        # Starts from noteheads with onset/pitch/duration.
+        noteheads_1 = self.collect_fully_defined_noteheads(g1)
+        noteheads_2 = self.collect_fully_defined_noteheads(g2)
+
+        # Matching data structure: dict with id tuples as keys, weights as values.
+        # Currently, weights will only be 1 (zero weights are not in the dict).
+        initial_matching = self.match_fully_defined_noteheads(noteheads_1, noteheads_2)
+        _matched_prev = copy.deepcopy(set(initial_matching.keys()))
+
+        print('Initialized matching: {0} noteheads, running growth iterations.'
+              ''.format(len(_matched_prev)))
+        partial_matching = self.grow_iteration(g1, g2, initial_matching)
+        # Add debugprints!
+        print('First growth iteration done.')
+        _n_iters = 1
+        while _matched_prev != set(partial_matching.keys()):
+            _matched_prev = set(partial_matching.keys())
+
+            partial_matching = self.grow_iteration(g1, g2, partial_matching)
+            _n_iters += 1
+            print('Growth iterations: {0}'.format(_n_iters))
+
+        return partial_matching
+
+    def grow_iteration(self, g1: NotationGraph, g2: NotationGraph, matching: Dict[Tuple[int, int], float]) -> \
+            Dict[Tuple[int, int], float]:
+        """One iteration of graph isomorphism growing.
+        Algorithm:
+
+        1. Connectivity signature matching
+
+        * For both graphs:
+            * For each vertex:
+                * Find connectivity signature to already matched vertices
+
+        * For each vertex u_i in g1 with non-empty connectivity signature:
+            * For each vertex v_j in g2 of the same class as u_i:
+                * If their connectivity signatures match, add them to potential
+                  matches pool. (Will then resolve ties.)
+
+        2. Within pools that share connectivity signatures:
+
+        This is what we want to resolve with EMD. Note that these groups will be
+        fairly small - at most 4 or 5 flags/beams or leger lines.
+
+        """
+        # TODO: factorize compatibility sets by object class!
+        anchor_mapping_1_to_2 = {k[0]: k[1] for k in matching.keys()}
+
+        csigs_1 = self.compute_connectivity_signatures(g1, anchors=[g1[k[0]] for k in matching.keys()])
+        csigs_2 = self.compute_connectivity_signatures(g2, anchors=[g2[k[1]] for k in matching.keys()])
+
+        # csigs contains for each vertex with a non-empty connectivity signature
+        # to the current anchors the list of anchor point outlinks and inlinks.
+
+        inverse_csigs_1 = collections.defaultdict(list)
+        for v1_objid in csigs_1:
+            inverse_csigs_1[csigs_1[v1_objid]].append(v1_objid)
+
+        inverse_csigs_2 = collections.defaultdict(list)
+        for v2_objid in csigs_2:
+            inverse_csigs_2[csigs_2[v2_objid]].append(v2_objid)
+
+        # We will keep the index of match-able vertices indexed
+        # by their connectivity signature w.r.t g2, so we project
+        # the connectivity signature from g1 through the anchor
+        # mapping.
+
+        # The compatible sets are a dict keyed by the corresponding csig_2.
+        # The values are tuples of lists: first list for a given csig_2
+        # contains the compatible vertices from graph 1, the second list
+        # contains compatible vertices from graph 2.
+        compatible_sets = collections.defaultdict(tuple)
+
+        for v1_objid, csig_1 in csigs_1.items():
+            inlinks, outlinks = csig_1
+            iso_inlinks = tuple([anchor_mapping_1_to_2[i] for i in inlinks])
+            iso_outlinks = tuple([anchor_mapping_1_to_2[i] for i in outlinks])
+            iso_csig = (iso_inlinks, iso_outlinks)
+
+            if iso_csig in inverse_csigs_2:
+                if iso_csig not in compatible_sets:
+                    compatible_sets[iso_csig] = [[], []]
+
+                compatible_sets[iso_csig][0].append(v1_objid)
+                for v2_objid in inverse_csigs_2[iso_csig]:
+                    if v2_objid not in compatible_sets[iso_csig][1]:
+                        compatible_sets[iso_csig][1].append(v2_objid)
+
+        output_matching = copy.deepcopy(matching)
+
+        # Now that we have the compatible sets, we resolve those that are
+        # larger than one.
+        for csig_2 in compatible_sets:
+            compatible_set_objids = compatible_sets[csig_2]
+            compatible_vertices_1 = [g1[node_id]
+                                     for node_id in compatible_set_objids[0]]
+            compatible_vertices_2 = [g2[node_id]
+                                     for node_id in compatible_set_objids[1]]
+            cset_matching = self.resolve_compatible_set_matching(compatible_vertices_1, compatible_vertices_2)
+            # Update output matching dict
+            output_matching.update(cset_matching)
+
+        return output_matching
+
+    def resolve_compatible_set_matching(self, vs1: List[Node], vs2: List[Node]) -> Dict[Tuple[int, int], float]:
+        """Given two sets of vertices that have isomorphic
+        connectivity signatures, resolves how they should actually
+        be matched against each other.
+
+        :param vs1: A list of Nodes.
+
+        :param vs2: A list of Nodes.
+
+        :return: A matching of these two Node lists. The matching
+            is a dict of ``(n1.id, n2.id) --> weight``.
+        """
+        output = {}
+
+        class_names = set([c.class_name for c in vs1 + vs2])
+
+        for class_name in class_names:
+            vs1_by_class = [c for c in vs1 if c.class_name == class_name]
+            vs2_by_class = [c for c in vs2 if c.class_name == class_name]
+
+            for v1, v2 in zip(sorted(vs1_by_class, key=lambda x: x.top),
+                              sorted(vs2_by_class, key=lambda y: y.top)):
+                output[(v1.id, v2.id)] = 1.0
+        return output
+
+    def compute_connectivity_signatures(self, g: NotationGraph, anchors: Iterable[Node]) -> \
+            Dict[int, Tuple[Tuple[int, ...], Tuple[int, ...]]]:
+        """Computes connectivity signatures for vertices in ``g`` to the given
+        ``anchors``.
+
+        :returns: Connectivity signature dict: ``v.id --> (inlinks_tuple, outlinks_tuple)``
+        """
+        output = dict()
+        anchor_set = set(anchors)
+        for c in g.vertices:
+            if c.id in anchor_set:
+                continue
+            anchor_outlinks = tuple([o for o in c.outlinks if o in anchor_set])
+            anchor_inlinks = tuple([i for i in c.inlinks if i in anchor_set])
+            if len(anchor_inlinks) + len(anchor_outlinks) > 0:
+                csig = (anchor_inlinks, anchor_outlinks)
+                output[c.id] = csig
+        return output
+
+    def collect_fully_defined_noteheads(self, graph: NotationGraph) -> List[Node]:
+        return [c for c in graph.vertices if self.__is_fully_defined_notehead(c)]
+
+    @staticmethod
+    def __is_fully_defined_notehead(node: Node) -> bool:
+        isdef = False
+        if (node.class_name in _CONST.NONGRACE_NOTEHEAD_CLASS_NAMES) \
+                and ('onset_beats' in node.data) \
+                and ('midi_pitch_code' in node.data):
+            isdef = True
+        return isdef
+
+    @staticmethod
+    def _notehead_signature(c: Node) -> Tuple[Any, Any, Any]:
+        return c.data['onset_beats'], c.data['midi_pitch_code'], c.data['duration_beats']
+
+    def match_fully_defined_noteheads(self, noteheads_1: List[Node], noteheads_2: List[Node]) -> \
+            Dict[Tuple[int, int], float]:
+        """Matches two lists of fully defined noteheads. Only matches those
+        that exactly share pitch, duration, and onset.
+
+        :returns: A matching: dict of ``(n1.id, n2.id) --> weight``.
+        """
+        output = {}
+        if (len(noteheads_1) == 0) or (len(noteheads_2) == 0):
+            return output
+
+        # Sort & slide algorithm makes this linear, not quadratic.
+        # With more than 500 noteheads, this starts to be felt.
+        ns1 = sorted(noteheads_1, key=lambda x: self._notehead_signature(x))
+        ns2 = sorted(noteheads_2, key=lambda x: self._notehead_signature(x))
+
+        j = 0
+        for n1 in ns1:
+            onset_1 = n1.data['onset_beats']
+
+            n2 = ns2[j]
+            # Make ns2 pointer catch up with the current note
+            while onset_1 > n2.data['onset_beats']:
+                j += 1
+                if j >= len(ns2):
+                    # We will not match anything anymore: noteheads_2 are exhausted.
+                    return output
+                n2 = ns2[j]
+
+            if onset_1 == n2.data['onset_beats']:
+                if self._notehead_signature(n1) == self._notehead_signature(n2):
+                    output[(n1.id, n2.id)] = 1.0
+                    j += 1
+                    continue
+
+            elif onset_1 < n2.data['onset_beats']:
+                continue
+
+        return output
+
+
+if __name__ == '__main__':
+    import os
+    from mung.io import read_nodes_from_file
+    from mung.graph import NotationGraph, NotationGraph, NotationGraph, NotationGraph
+
+    test_data_root = os.path.join(os.path.dirname(os.path.abspath(__file__)),
+                                  '..', 'test',
+                                  'test_data',
+                                  'mungmatcher')
+    gt_root = os.path.join(test_data_root, 'gt')
+    de_root = os.path.join(test_data_root, 'detected')
+    wc_root = os.path.join(test_data_root, 'without_contained')
+
+    names = ['minifull.xml',
+             'mini2full.xml']
+
+    gt = NotationGraph(read_nodes_from_file(os.path.join(test_data_root, names[0])))
+    wc = NotationGraph(read_nodes_from_file(os.path.join(test_data_root, names[1])))
+
+    matcher = MungMatcher()
+
+    aln = matcher.run(gt, gt)
+    print('Matched GT against GT: {} gt, {} gt, {} matched'
+          ''.format(len(gt), len(gt), len(aln)))
+
+    aln = matcher.run(gt, wc)
+    print('Matched GT against WC: {} gt, {} wc, {} matched'
+          ''.format(len(gt), len(wc), len(aln)))
+
+    aln = matcher.run(gt, gt)
+    print('Matched WC against WC: {} wc, {} wc, {} matched'
+          ''.format(len(wc), len(wc), len(aln)))
```

### Comparing `mung-1.1/mung/node.py` & `mung-1.2/mung/node.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1352 +1,1355 @@
-import copy
-import itertools
-import logging
-from typing import List, Union, Tuple, Optional, Any
-
-import numpy
-from math import ceil
-
-from mung.utils import compute_connected_components
-
-
-class Node(object):
-    """One annotated object.
-
-    The Node represents one instance of an annotation. It implements
-    the following attributes:
-
-    * ``node_id``: the unique number of the given annotation instance in the set
-      of annotations encoded in the containing `NodeList`.
-    * ``dataset``: the name of the dataset this Node belongs to, e.g., MUSCIMA++_2.0
-    * ``document``: the name of the document this Node belongs to, e.g., CVC-MUSCIMA_W-05_N-19_D-ideal
-    * ``class_name``: the name of the label that was given to the annotation
-      (this is the human-readable string such as ``notehead-full``).
-    * ``top``: the vertical dimension (row) of the upper left corner pixel.
-    * ``left``: the horizontal dimension (column) of the upper left corner pixel.
-    * ``bottom``: the vertical dimension (row) of the lower right corner pixel + 1,
-      so that you can index the corresponding image rows using
-      ``img[c.top:c.bottom]``.
-    * ``right``: the horizontal dimension (row) of the lower right corner pixel + 1,
-      so that you can index the corresponding image columns using
-      ``img[:, c.left:c.right]``.
-    * ``width``: the amount of rows that the Node spans.
-    * ``height``: the amount of columns that the Node spans.
-    * ``mask``: a binary (0/1) numpy array that denotes the area within the
-      Node's bounding box (specified by ``top``, ``left``, ``height``
-      and ``width``) that the Node actually occupies. If the mask is
-      ``None``, the object is understood to occupy the entire bounding box.
-    * ``data``: a dictionary that can be empty, or can contain anything. It is
-      generated from the optional ``<Data>`` element of a Node.
-
-    Constructing a simple Node that consists of the "b"-like flat music
-    notation symbol (never mind the ``unique_id`` for now):
-
-    >>> top = 10
-    >>> left = 15
-    >>> height = 10
-    >>> width = 4
-    >>> mask = numpy.array([[1, 1, 0, 0],
-    ...                     [1, 0, 0, 0],
-    ...                     [1, 0, 0, 0],
-    ...                     [1, 0, 0, 0],
-    ...                     [1, 0, 1, 1],
-    ...                     [1, 1, 1, 1],
-    ...                     [1, 0, 0, 1],
-    ...                     [1, 0, 1, 1],
-    ...                     [1, 1, 1, 0],
-    ...                     [0, 1, 0, 0]])
-    >>> class_name = 'flat'
-    >>> dataset = 'MUSCIMA-pp_2.0'
-    >>> document = 'CVC-MUSCIMA_W-35_N-08_D-ideal'
-    >>> node = Node(611, class_name=class_name,
-    ...                top=top, left=left, height=height, width=width,
-    ...                inlinks=[], outlinks=[],
-    ...                mask=mask,
-    ...                dataset=dataset, document=document)
-
-    Nodes can also form graphs, using the following attributes:
-
-    * ``outlinks``: Outgoing edges. A list of integers; it is assumed they are
-      valid ``node_id`` within the same global/doc namespace.
-    * ``inlinks``: Incoming edges. A list of integers; it is assumed they are
-      valid ``node_id`` within the same global/doc namespace.
-
-    So far, Node graphs do not support multiple relationship types.
-
-    **Unique identification**
-
-    The ``unique_id`` serves to identify the Node uniquely,
-    at least within the MUSCIMA dataset system. (We anticipate further
-    versions of the dataset, and need to plan for that.)
-
-    To uniquely identify a Node, there are three "levels":
-
-    * The "global", **dataset-level identification**: which dataset is this
-      Node coming from? (For this dataset: ``MUSCIMA++_1.0``)
-    * The "local", **document-level identification**: which document
-      (within the given dataset) is this Node coming from?
-      For MUSCIMA++ 1.0, this will usually be a string like
-      ``CVC-MUSCIMA_W-35_N-08_D-ideal``, derived from the filename
-      under which the Nodes containing the given Node
-      is stored.
-    * The **within-document identification**, which is the ``node_id``.
-
-    These three components are joined together into one string by
-    a delimiter: ``___``
-
-    The full ``unique_id`` of a Node then might look like this::
-    >>> node.unique_id
-    'MUSCIMA-pp_2.0___CVC-MUSCIMA_W-35_N-08_D-ideal___611'
-
-    And it consists of these three parts:
-
-    >>> node.document
-    'CVC-MUSCIMA_W-35_N-08_D-ideal'
-    >>> node.dataset
-    'MUSCIMA-pp_2.0'
-    >>> node.id
-    611
-
-    **Nodes and images**
-
-    Nodes and images are not tightly bound. This is because the same
-    object can apply to multiple images: in the case of the CVC-MUSCIMA dataset,
-    for example, the same Nodes are present both in the full image
-    and in the staff-less image. The limitation here is that Nodes
-    are based on exact pixels, so in order to retain validity, the images
-    must correspond to each other exactly, as "layers".
-
-    Because Nodes do not correspond to any given image, there is
-    no facility in the data format to link them to a specific one. You have to
-    take care of matching Node annotations to the right images by yourself.
-
-    The ``Node`` class implements some interactions with images.
-
-    To recover the area corresponding to a Node `c`, use:
-
-    >>> image = numpy.array([]) #doctest: +SKIP
-    >>> if node.mask is not None: crop = image[node.top:node.bottom, node.left:node.right] * node.mask  #doctest: +SKIP
-    >>> if node.mask is None: crop = image[node.top:node.bottom, node.left:node.right]               #doctest: +SKIP
-
-    Because this is clunky, we have implemented the following to get the crop:
-
-    >>> crop = node.project_to(image)    #doctest: +SKIP
-
-    And to get the Node projected onto the entire image:
-
-    >>> crop = node.project_on(image)    #doctest: +SKIP
-
-    Above, note the multiplicative role of the mask: while we typically would
-    expect the mask to be binary, in principle, this is not strictly necessary.
-    You could supply a different mask interpration, such as probabilistic.
-    However, we strongly advise not to misuse this feature unless you have
-    a really good reason; remember that the Node is supposed to represent
-    an annotation of a given image. (One possible use for a non-binary mask
-    that we can envision is aggregating multiple annotations of the same
-    image.)
-
-    For visualization, there is a more sophisticated method that renders
-    the Node as a transparent colored transparent rectangle over
-    an RGB image. (NOTE: this really changes the input image!)
-
-    >>> import matplotlib.pyplot as plt #doctest: +SKIP
-    >>> node.render(image)           #doctest: +SKIP
-    >>> plt.imshow(image); plt.show() #doctest: +SKIP
-
-    However, `Node.render()` currently does not support rendering
-    the mask.
-
-    **Disambiguating class names**
-
-    Since the class names are present
-    through the ``class_name`` attribute (``<ClassName>`` element),
-    matching the list is no longer necessary for general understanding
-    of the file. The NodeClasses file serves as a disambiguation tool:
-    there may be multiple annotation projects that use the same names
-    but maybe define them differently and use different guidelines,
-    and their respective NodeClasses allow you to interpret the symbol
-    names correctly, in light of the corresponding set of definitions.
-
-    .. note::
-
-        In MUSCIMarker, the NodeClasses is currently necessary to define
-        how Nodes are displayed: their color. (All noteheads are red,
-        all barlines are green, etc.) The other function, matching names
-        to ``clsid``, has been superseeded by the ``class_name`` Node
-        attribute.
-
-    **Merging Nodes**
-
-    To merge a list of Nodes into a new one, you need to:
-
-    * Compute the new object's bounding box: ``compute_unifying_bounding_box()``
-    * Compute the new object's mask: ``compute_unifying_mask()``
-    * Determine the class_name and node_id of the new object.
-
-    Since node_id and class_name of merges may depend on external settings
-    and generally cannot be reliably determined from the merged
-    objects themselves (e.g. the merge of a notehead and a stem
-    should be a new note symbol), you need to supply them externally.
-    However, the bounding box and mask can be determined. The bounding
-    box is computed simply as the smallest bounding box that
-    encompasses all the Nodes, and the mask is an OR operation
-    over the individual masks (or None, if the Nodes don't
-    have masks). Note that the merge cannot deal with a situation
-    where only some of the objects have a mask.
-
-    **Implementation notes on the mask**
-
-    The mask is a numpy array that will be saved using run-length encoding.
-    The numpy array is first flattened, then runs of successive 0's and 1's
-    are encoded as e.g. ``0:10`` for a run of 10 zeros.
-
-    How much space does this take?
-
-    Objects tend to be relatively convex, so after flattening, we can expect
-    more or less two runs per row (flattening is done in ``C`` order). Because
-    each run takes (approximately) 5 characters, each mask takes roughly ``5 * n_rows``
-    bytes to encode. This makes it efficient for objects wider than 5 pixels, with
-    a compression ratio approximately ``n_cols / 5``.
-    (Also, the numpy array needs to be made C-contiguous for that, which
-    explains the ``order='C'`` hack in ``set_mask()``.)
-    """
-
-    # Delimits the Node UID fields (global, document namespaces, id)
-    UID_DELIMITER = '___'
-    DEFAULT_DATASET = 'MUSCIMA_DEFAULT_DATASET_PLACEHOLDER'
-    DEFAULT_DOCUMENT = 'default-document'
-
-    def __init__(self, id_: int,
-                 class_name: str,
-                 top: int,
-                 left: int,
-                 width: int,
-                 height: int,
-                 outlinks: List[int] = None,
-                 inlinks: List[int] = None,
-                 mask: numpy.ndarray = None,
-                 dataset: str = None,
-                 document: str = None,
-                 data=None):
-        self.__id = id_
-        self.__class_name = class_name
-        self.__top = top
-        self.__left = left
-        self.__width = width
-        self.__height = height
-
-        # The mask presupposes integer bounds.
-        # Applied relative to Node bounds, not the whole image.
-        self.__to_integer_bounds()
-        self.__mask = None
-        self.set_mask(mask)
-
-        if inlinks is None:
-            inlinks = []
-        self.inlinks = inlinks  # type: List[int]
-
-        if outlinks is None:
-            outlinks = []
-        self.outlinks = outlinks  # type: List[int]
-
-        if dataset is None:
-            dataset = self.DEFAULT_DATASET
-        self.__dataset = dataset
-
-        if document is None:
-            document = self.DEFAULT_DOCUMENT
-        self.__document = document
-
-        self.is_selected = False
-
-        if data is None:
-            data = dict()
-        self.data = data
-
-    @property
-    def unique_id(self) -> str:
-        """Returns the ``unique_id`` of this Node
-
-        >>> node = Node(0, "", 0, 0, 0, 0)
-        >>> node.unique_id
-        'MUSCIMA_DEFAULT_DATASET_PLACEHOLDER___default-document___0'
-        """
-        return self.UID_DELIMITER.join([self.dataset,
-                                        self.document,
-                                        str(self.id)])
-
-    @staticmethod
-    def parse_unique_id(uid: str) -> (str, str, int):
-        """Parse a unique identifier. This breaks down the UID into the dataset name,
-        document name, and id
-
-        The delimiter is expected to be ``___``
-        (kept as ``Node.UID_DELIMITER``)
-
-        >>> Node.parse_unique_id('MUSCIMA++_2.0___CVC-MUSCIMA_W-05_N-19_D-ideal___424')
-        ('MUSCIMA++_2.0', 'CVC-MUSCIMA_W-05_N-19_D-ideal', 424)
-
-        :returns: ``global_namespace, document_namespace, id`` triplet.
-            The namespaces are strings, ``id`` is an integer. If ``unique_id``
-            is ``None``, returns ``None`` as ``id`` and expects it
-            to be filled in from the caller Node instance.
-        """
-        if uid is None:
-            global_namespace = Node.DEFAULT_DATASET
-            document_namespace = Node.DEFAULT_DOCUMENT
-            node_id = None
-        else:
-            global_namespace, document_namespace, node_id_string = uid.split(Node.UID_DELIMITER)
-            node_id = int(node_id_string)
-        return global_namespace, document_namespace, node_id
-
-    @property
-    def id(self) -> int:
-        return self.__id
-
-    def set_id(self, id_):
-        self.__id = id_
-
-    @property
-    def class_name(self) -> str:
-        return self.__class_name
-
-    @property
-    def dataset(self) -> str:
-        return self.__dataset
-
-    @property
-    def document(self) -> str:
-        return self.__document
-
-    @property
-    def top(self) -> int:
-        """Row coordinate of upper left corner."""
-        return self.__top
-
-    @property
-    def bottom(self) -> int:
-        """Row coordinate 1 beyond bottom right corner, so that indexing
-        in the form ``img[node.top:node.bottom]`` is possible."""
-        return self.__top + self.__height
-
-    @property
-    def left(self) -> int:
-        """Column coordinate of upper left corner."""
-        return self.__left
-
-    @property
-    def right(self) -> int:
-        """Column coordinate 1 beyond bottom right corner, so that indexing
-        in the form ``img[:, node.left:node.right]`` is possible."""
-        return self.__left + self.__width
-
-    @property
-    def width(self) -> int:
-        return self.__width
-
-    @property
-    def height(self) -> int:
-        return self.__height
-
-    @property
-    def bounding_box(self) -> Tuple[int, int, int, int]:
-        """The ``top, left, bottom, right`` tuple of the Node's coordinates."""
-        return self.top, self.left, self.bottom, self.right
-
-    @property
-    def middle(self) -> Tuple[int, int]:
-        """Returns the integer representation of where the middle
-        of the Node lies, as a ``(m_vert, m_horz)`` tuple.
-
-        The integers just get rounded down.
-
-        >>> node = Node(0,'', 10, 20, 30, 40)
-        >>> node.middle
-        (30, 35)
-        """
-        vertical_center = self.top + self.height // 2
-        horizontal_center = self.left + self.width // 2
-        return int(vertical_center), int(horizontal_center)
-
-    @property
-    def mask(self) -> numpy.ndarray:
-        return self.__mask
-
-    def set_mask(self, mask: numpy.ndarray):
-        """Sets the Node's mask to the given array. Performs
-        some compatibility checks: size, dtype (converts to ``uint8``)."""
-        if mask is None:
-            self.__mask = None
-        else:
-            # Check dimension
-            t, l, b, r = self.round_bounding_box_to_integer(self.top,
-                                                            self.left,
-                                                            self.bottom,
-                                                            self.right)
-            if mask.shape != (b - t, r - l):
-                raise ValueError('Mask shape {0} does not correspond'
-                                 ' to integer shape {1} of Node.'
-                                 ''.format(mask.shape, (b - t, r - l)))
-            if str(mask.dtype) != 'uint8':
-                logging.debug('Node.set_mask(): Supplied non-integer mask'
-                              ' with dtype={0}'.format(mask.dtype))
-
-            self.__mask = mask.astype('uint8')
-
-    @staticmethod
-    def round_bounding_box_to_integer(top: float, left: float, bottom: float, right: float) \
-            -> (int, int, int, int):
-        """Rounds off the Node bounds to the nearest integer
-        so that no area is lost (e.g. bottom and right bounds are
-        rounded up, top and left bounds are rounded down).
-
-        Returns the rounded-off integers (top, left, bottom, right)
-        as integers.
-
-        >>> Node.round_bounding_box_to_integer(44.2, 18.9, 55.1, 92.99)
-        (44, 18, 56, 93)
-        >>> Node.round_bounding_box_to_integer(44, 18, 56, 92.99)
-        (44, 18, 56, 93)
-
-        """
-        return int(top), int(left), int(ceil(bottom)), int(ceil(right))
-
-    def project_to(self, image: numpy.ndarray):
-        """This function returns the *crop* of the input image
-        corresponding to the Node (incl. masking).
-        Assumes zeros are background."""
-        # Make a copy! We don't want to modify the original image by the mask.
-        # Copy forced by the "* 1" part.
-        crop = image[self.top:self.bottom, self.left:self.right] * 1
-        if self.__mask is not None:
-            crop *= self.__mask
-        return crop
-
-    def project_on(self, image: numpy.ndarray):
-        """This function returns only those parts of the input image
-        that correspond to the Node and masks out everything else
-        with zeros. The dimension of the returned array is the same
-        as of the input image. This function basically reconstructs
-        the symbol as an indicator function over the pixels of
-        the annotated image."""
-        output = numpy.zeros(image.shape, image.dtype)
-        crop = self.project_to(image)
-        output[self.top:self.bottom, self.left:self.right] = crop
-        return output
-
-    def render(self, image: numpy.ndarray, alpha: float = 0.3,
-               rgb: Tuple[float, float, float] = (1.0, 0.0, 0.0)) -> numpy.ndarray:
-        """Renders itself upon the given image as a rectangle
-        of the given color and transparency. Might help visualization.
-        """
-        color = numpy.array(rgb)
-        logging.debug('Rendering object {0}, class_name {1}, t/b/l/r: {2}'
-                      ''.format(self.id, self.class_name,
-                                (self.top, self.bottom, self.left, self.right)))
-        # logging.debug('Shape: {0}'.format((self.height, self.width, 3)))
-        mask = numpy.ones((self.__height, self.__width, 3)) * color
-        crop = image[self.top:self.bottom, self.left:self.right]
-        # logging.debug('Mask done, creating crop')
-        logging.debug('Shape: {0}. Got crop. Crop shape: {1}, img shape: {2}'
-                      ''.format((self.__height, self.__width, 3), crop.shape, image.shape))
-        mix = (crop + alpha * mask) / (1 + alpha)
-
-        image[self.top:self.bottom, self.left:self.right] = mix
-        return image
-
-    def overlaps(self, bounding_box_or_node):
-        # type: (Union[Tuple[int, int, int, int], Node]) -> bool
-        """Check whether this Node overlaps the given bounding box or Node.
-
-        >>> node = Node(0, 'test', 10, 100, height=20, width=10)
-        >>> node.bounding_box
-        (10, 100, 30, 110)
-        >>> node.overlaps((10, 100, 30, 110))  # Exact match
-        True
-        >>> node.overlaps((0, 100, 8, 110))    # Row mismatch
-        False
-        >>> node.overlaps((10, 0, 30, 89))     # Column mismatch
-        False
-        >>> node.overlaps((0, 0, 8, 89))       # Total mismatch
-        False
-        >>> node.overlaps((9, 99, 31, 111))    # Encompasses Node
-        True
-        >>> node.overlaps((11, 101, 29, 109))  # Within Node
-        True
-        >>> node.overlaps((9, 101, 31, 109))   # Encompass horz., within vert.
-        True
-        >>> node.overlaps((11, 99, 29, 111))   # Encompasses vert., within horz.
-        True
-        >>> node.overlaps((11, 101, 31, 111))  # Corner within: top left
-        True
-        >>> node.overlaps((11, 99, 31, 109))   # Corner within: top right
-        True
-        >>> node.overlaps((9, 101, 29, 111))   # Corner within: bottom left
-        True
-        >>> node.overlaps((9, 99, 29, 109))    # Corner within: bottom right
-        True
-
-        """
-        if isinstance(bounding_box_or_node, Node):
-            t, l, b, r = bounding_box_or_node.bounding_box
-        else:
-            t, l, b, r = bounding_box_or_node
-        # Does it overlap vertically? Includes situations where the Node is inside the bounding box.
-        # Note that the bottom is +1 (fencepost), so the checks bottom vs. top need to be "less than",
-        # not leq. If one object's top would be equal to the other's bottom, they would be touching,
-        # not overlapping.
-        if max(t, self.top) < min(b, self.bottom):
-            if max(l, self.left) < min(r, self.right):
-                return True
-        return False
-
-    def contains(self, bounding_box_or_node):
-        # type: (Union[Tuple[int, int, int, int], Node]) -> bool
-        """Check if this Node entirely contains the other bounding
-        box (or, the other node's bounding box)."""
-        if isinstance(bounding_box_or_node, Node):
-            top, left, bottom, right = bounding_box_or_node.bounding_box
-        else:
-            top, left, bottom, right = bounding_box_or_node
-
-        if self.top <= top <= bottom <= self.bottom:
-            if self.left <= left <= right <= self.right:
-                return True
-        return False
-
-    def bounding_box_intersection(self, bounding_box: Tuple[int, int, int, int]) \
-            -> Optional[Tuple[int, int, int, int]]:
-        """Returns the sub-bounding box of this Node intersecting with the given bounding box.
-        If the intersection is empty, returns None.
-
-        >>> node = Node(0, 'test', 10, 100, height=20, width=10)
-        >>> node.bounding_box
-        (10, 100, 30, 110)
-        >>> other_bbox = 20, 100, 40, 105
-        >>> node.bounding_box_intersection(other_bbox)
-        (10, 0, 20, 5)
-        >>> containing_bbox = 4, 55, 44, 115
-        >>> node.bounding_box_intersection(containing_bbox)
-        (0, 0, 20, 10)
-        >>> contained_bbox = 12, 102, 22, 108
-        >>> node.bounding_box_intersection(contained_bbox)
-        (2, 2, 12, 8)
-        >>> non_overlapping_bbox = 0, 0, 3, 3
-        >>> node.bounding_box_intersection(non_overlapping_bbox) is None
-        True
-
-        """
-        t, l, b, r = bounding_box
-
-        out_top = max(t, self.top)
-        out_bottom = min(b, self.bottom)
-        out_left = max(l, self.left)
-        out_right = min(r, self.right)
-
-        if (out_top < out_bottom) and (out_left < out_right):
-            return out_top - self.top, \
-                   out_left - self.left, \
-                   out_bottom - self.top, \
-                   out_right - self.left
-        else:
-            return None
-
-    def crop_to_mask(self):
-        """Crops itself to the minimum bounding box that contains all
-        its pixels, as determined by its mask.
-
-        If the mask is all zeros, does not do anything, because
-        at this point, the is_empty check should be invoked anyway
-        in any situation where you care whether the object is empty
-        or not (e.g. delete it after trimming).
-
-        >>> mask = numpy.zeros((20, 10))
-        >>> mask[5:15, 3:8] = 1
-        >>> node = Node(0, 'test', 10, 100, width=10, height=20, mask=mask)
-        >>> node.bounding_box
-        (10, 100, 30, 110)
-        >>> node.crop_to_mask()
-        >>> node.bounding_box
-        (15, 103, 25, 108)
-        >>> node.height, node.width
-        (10, 5)
-
-        Assumes integer bounds, which is ensured during Node initialization.
-        """
-        if self.__mask is None:
-            return
-
-        mask_is_empty = self.__mask.sum() == 0
-        if mask_is_empty:
-            return
-
-        # We know the object is not empty.
-
-        # How many rows/columns to trim from top, bottom, etc.
-        trim_top = -1
-        for i in range(self.__mask.shape[0]):
-            if self.__mask[i, :].sum() != 0:
-                trim_top = i
-                break
-
-        trim_left = -1
-        for j in range(self.__mask.shape[1]):
-            if self.__mask[:, j].sum() != 0:
-                trim_left = j
-                break
-
-        trim_bottom = -1
-        for k in range(self.__mask.shape[0]):
-            if self.__mask[-(k + 1), :].sum() != 0:
-                trim_bottom = k
-                break
-
-        trim_right = -1
-        for l in range(self.__mask.shape[1]):
-            if self.__mask[:, -(l + 1)].sum() != 0:
-                trim_right = l
-                break
-
-        logging.debug('Node.crop: Trimming top={0}, left={1},'
-                      'bottom={2}, right={3}'
-                      ''.format(trim_top, trim_left, trim_bottom, trim_right))
-
-        # new bounding box relative to the current bounding box -- used to trim
-        # the mask
-        rel_t = trim_top
-        rel_l = trim_left
-        rel_b = self.__height - trim_bottom
-        rel_r = self.__width - trim_right
-
-        new_mask = self.__mask[rel_t:rel_b, rel_l:rel_r] * 1
-
-        logging.debug('Node.crop: Old mask shape {0}, new mask shape {1}'
-                      ''.format(self.__mask.shape, new_mask.shape))
-
-        # new bounding box, relative to image -- used to compute the Node's position and size
-        abs_t = self.top + trim_top
-        abs_l = self.left + trim_left
-        abs_b = self.bottom - trim_bottom
-        abs_r = self.right - trim_right
-
-        self.__top = abs_t
-        self.__left = abs_l
-        self.__height = abs_b - abs_t
-        self.__width = abs_r - abs_l
-
-        self.set_mask(new_mask)
-
-    def __str__(self):
-        """Format the Node as string representation. See the documentation
-        of :module:`mung.io` for details."""
-        lines = []
-        lines.append('<Node>')
-        lines.append('\t<Id>{0}</Id>'.format(self.id))
-        lines.append('\t<ClassName>{0}</ClassName>'.format(self.class_name))
-        lines.append('\t<Top>{0}</Top>'.format(self.top))
-        lines.append('\t<Left>{0}</Left>'.format(self.left))
-        lines.append('\t<Width>{0}</Width>'.format(self.__width))
-        lines.append('\t<Height>{0}</Height>'.format(self.__height))
-
-        mask_string = self.encode_mask()
-        lines.append('\t<Mask>{0}</Mask>'.format(mask_string))
-
-        if len(self.inlinks) > 0:
-            inlinks_string = ' '.join(list(map(str, self.inlinks)))
-            lines.append('\t<Inlinks>{0}</Inlinks>'.format(inlinks_string))
-        if len(self.outlinks) > 0:
-            outlinks_string = ' '.join(list(map(str, self.outlinks)))
-            lines.append('\t<Outlinks>{0}</Outlinks>'.format(outlinks_string))
-
-        data_string = self.encode_data()
-        if data_string is not None:
-            lines.append('\t<Data>\n{0}\n\t</Data>'.format(data_string))
-
-        lines.append('</Node>')
-        return '\n'.join(lines)
-
-    def encode_mask(self, mode: str = 'rle') -> str:
-        """Encode a binary array ``mask`` as a string, compliant
-        with the Node format specification in :mod:`mung.io`.
-        """
-        if mode == 'rle':
-            return self.encode_mask_rle(self.mask)
-        elif mode == 'bitmap':
-            return self.encode_mask_bitmap(self.mask)
-
-    def encode_data(self) -> Optional[str]:
-        if self.data is None:
-            return None
-        if len(self.data) == 0:
-            return None
-
-        lines = []
-        for k, v in list(self.data.items()):
-            vtype = 'str'
-            vval = v
-            if isinstance(v, int):
-                vtype = 'int'
-                vval = str(v)
-            elif isinstance(v, float):
-                vtype = 'float'
-                vval = str(v)
-            elif isinstance(v, list):
-                vtype = 'list[str]'
-                if len(v) > 0:
-                    if isinstance(v[0], int):
-                        vtype = 'list[int]'
-                    elif isinstance(v[0], float):
-                        vtype = 'list[float]'
-                vval = ' '.join([str(vv) for vv in v])
-
-            line = '\t\t<DataItem key="{0}" type="{1}">{2}</DataItem>' \
-                   ''.format(k, vtype, vval)
-            lines.append(line)
-
-        return '\n'.join(lines)
-
-    def data_display_text(self) -> str:
-        if self.data is None:
-            return '[No data]'
-        if len(self.data) == 0:
-            return '[No data]'
-
-        lines = []
-        for k, v in list(self.data.items()):
-            lines.append('{0}:      {1}'.format(k, v))
-        return '\n'.join(lines)
-
-    @staticmethod
-    def encode_mask_bitmap(mask: numpy.ndarray) -> str:
-        """Encodes the mask array in a compact form. Returns 'None' if mask
-        is None. If the mask is not None, uses the following algorithm:
-
-        * Flatten the mask (then use width and height of Node for reshaping).
-        * Record as string, with whitespace separator
-        * Return resulting string
-        """
-        if mask is None:
-            return 'None'
-        # By default works in row-major order.
-        # So we can just prescribe 'C' without losing data.
-        mask_flat = mask.flatten(order='C')
-        output = ' '.join(list(map(str, mask_flat)))
-        return output
-
-    @staticmethod
-    def encode_mask_rle(mask: numpy.ndarray) -> str:
-        """Encodes the mask array in Run-Length Encoding. Instead of
-        having the bitmap ``0 0 1 1 1 0 0 0 1 1``, the RLE encodes
-        the mask as ``0:2 1:3 0:3 1:2``. This is much more compact.
-
-        Currently, the rows of the mask are not treated in any special
-        way. The mask just gets flattened and then encoded.
-
-        """
-        if mask is None:
-            return 'None'
-        mask_flat = mask.flatten(order='C')
-
-        output_strings = []
-        current_run_type = 0
-        current_run_length = 0
-        for i in mask_flat:
-            if i == current_run_type:
-                current_run_length += 1
-            else:
-                s = '{0}:{1}'.format(current_run_type, current_run_length)
-                output_strings.append(s)
-                current_run_type = i
-                current_run_length = 1
-        s = '{0}:{1}'.format(current_run_type, current_run_length)
-        output_strings.append(s)
-        output = ' '.join(output_strings)
-        return output
-
-    @staticmethod
-    def decode_mask(mask_string: str, shape) -> Optional[numpy.ndarray]:
-        """Decodes a Node mask string into a binary
-        numpy array of the given shape."""
-        mode = Node.__determine_mask_mode(mask_string)
-        if mode == 'rle':
-            return Node.decode_mask_rle(mask_string, shape=shape)
-        elif mode == 'bitmap':
-            return Node.decode_mask_bitmap(mask_string, shape=shape)
-
-    @staticmethod
-    def __determine_mask_mode(mask_string: str):
-        """If the mask string starts with '0:' or '1:', or generally
-        if it contains a non-0 or 1 symbol, assume it is RLE."""
-        mode = 'bitmap'
-        if len(mask_string) < 3:
-            mode = 'bitmap'
-        elif ':' in mask_string[:3]:
-            mode = 'rle'
-        return mode
-
-    @staticmethod
-    def decode_mask_bitmap(mask_string: str, shape) -> Optional[numpy.ndarray]:
-        """Decodes the mask array from the encoded form to the 2D numpy array."""
-        if mask_string == 'None':
-            return None
-        try:
-            values = list(map(float, mask_string.split()))
-        except ValueError:
-            logging.info(
-                'Node.decode_mask_bitmap() Cannot decode mask values:\n{0}'.format(mask_string))
-            raise
-        mask = numpy.array(values).reshape(shape)
-        return mask
-
-    @staticmethod
-    def decode_mask_rle(mask_string: str, shape) -> Optional[numpy.ndarray]:
-        """Decodes the mask array from the RLE-encoded form
-        to the 2D numpy array.
-        """
-        if mask_string == 'None':
-            return None
-
-        mask_flat = numpy.zeros(shape[0]*shape[1], numpy.uint8)
-        index = 0
-        for kv in mask_string.split(' '):
-            k_string, v_string = kv.split(':')
-            k, v = int(k_string), int(v_string)
-            if k == 1:
-                mask_flat[index:index+v] = 1
-            index += v
-
-        mask = mask_flat.reshape(shape)
-        return mask
-
-    def join(self, other):
-        """Node "addition": performs an OR on this
-        and the ``other`` Nodes' masks and bounding boxes,
-        and assigns to this Node the result. Merges
-        also the inlinks and outlinks.
-
-        Works only if the document spaces for both Nodes
-        are the same. (Otherwise changes nothing.)
-
-        The ``class_name`` of the ``other`` is ignored.
-        """
-        if self.document != other.document:
-            logging.warning(
-                "Trying to join Node from different documents, which is forbidden. Skipping join.")
-            return
-
-        # Get combined bounding box
-        new_top = min(self.top, other.top)
-        new_left = min(self.left, other.left)
-        new_bottom = max(self.bottom, other.bottom)
-        new_right = max(self.right, other.right)
-
-        new_height = new_bottom - new_top
-        new_width = new_right - new_left
-
-        # Create mask of corresponding size
-        new_mask = numpy.zeros((new_height, new_width), dtype=self.__mask.dtype)
-
-        # Find coordinates where to paste the masks
-        spt = self.top - new_top
-        spl = self.left - new_left
-        opt = other.top - new_top
-        opl = other.left - new_left
-
-        # Paste the masks into these places
-        new_mask[spt:spt + self.__height, spl:spl + self.__width] += self.__mask
-        new_mask[opt:opt + other.height, opl:opl + other.width] += other.mask
-
-        # Normalize mask value
-        new_mask[new_mask != 0] = 1
-
-        # Assign the new variables to this Node
-        self.__top = new_top
-        self.__left = new_left
-        self.__height = new_height
-        self.__width = new_width
-        self.__mask = new_mask
-
-        # Add inlinks and outlinks (check for multiple and self-reference)
-        for o in other.outlinks:
-            if (o not in self.outlinks) and (o != self.id):
-                self.outlinks.append(o)
-        for i in other.inlinks:
-            if (i not in self.inlinks) and (i != self.id):
-                self.inlinks.append(i)
-
-    def get_outlink_objects(self, nodes):
-        # type: (List[Node]) -> List[Node]
-        """Out of the given ``nodes`` list, return a list
-        of those to which this Node has outlinks.
-        Can deal with Nodes from multiple documents.
-        """
-        return self.__check_nodes_that_have_links(self.outlinks, nodes)
-
-    def get_inlink_objects(self, nodes):
-        # type: (List[Node]) -> List[Node]
-        """Out of the given ``nodes`` list, return a list
-        of those from which this node has inlinks
-        Can deal with Nodes from multiple documents.
-        """
-        return self.__check_nodes_that_have_links(self.inlinks, nodes)
-
-    def __check_nodes_that_have_links(self, links, nodes):
-        # type: (List[int], List[Node]) -> List[Node]
-        output = []
-        if len(links) == 0:
-            return output
-
-        link_set = frozenset(links)
-
-        for node in nodes:
-            if node.document != self.document:
-                continue
-            if node.id in link_set:
-                output.append(node)
-            if len(output) == len(self.inlinks):
-                break
-        return output
-
-    def translate(self, down: int = 0, right: int = 0):
-        """Move the Node down and right by the given amount of pixels."""
-        self.__top += down
-        self.__left += right
-
-    def scale(self, zoom: float = 1.0):
-        """Re-compute the Node with the given scaling factor."""
-        mask = self.__mask * 1.0
-        import skimage.transform
-        new_mask_shape = max(int(self.__height * zoom), 1), max(int(self.__width * zoom), 1)
-        new_mask = skimage.transform.resize(mask,
-                                            output_shape=new_mask_shape)
-        new_mask[new_mask >= 0.5] = 1
-        new_mask[new_mask < 0.5] = 0
-        new_mask = new_mask.astype('uint8')
-
-        new_height, new_width = new_mask.shape
-        new_top = int(self.top * zoom)
-        new_left = int(self.left * zoom)
-
-        self.__top = new_top
-        self.__left = new_left
-        self.__height = new_height
-        self.__width = new_width
-        self.__mask = new_mask
-
-    def __to_integer_bounds(self):
-        """Ensures that the Node has an integer position and size.
-        (This is important whenever you want to use a mask, and reasonable
-        whenever you do not need sub-pixel resolution...)
-        """
-        bounding_box = self.bounding_box
-        top, left, bottom, right = self.round_bounding_box_to_integer(*bounding_box)
-        height = bottom - top
-        width = right - left
-
-        self.__top = top
-        self.__left = left
-        self.__height = height
-        self.__width = width
-
-    def distance_to(self, node) -> Any:
-        """Computes the distance between this node and another node.
-        Their minimum vertical and horizontal distances are each taken
-        separately, and the euclidean norm is computed from them."""
-        if self.document != node.document:
-            logging.warning('Cannot compute distances between Nodes'
-                            ' from different documents! ({0} vs. {1})'
-                            ''.format(self.document, node.document))
-
-        if (self.top <= node.top <= self.bottom) or (node.top <= self.top <= node.bottom):
-            delta_vert = 0
-        elif self.top < node.top:
-            delta_vert = node.top - self.bottom
-        else:
-            delta_vert = self.top - node.bottom
-
-        if (self.left <= node.left <= self.right) or (node.left <= self.left <= node.right):
-            delta_horz = 0
-        elif self.left < node.left:
-            delta_horz = node.left - self.right
-        else:
-            delta_horz = self.left - node.right
-
-        return numpy.sqrt(delta_vert ** 2 + delta_horz ** 2)
-
-    def compute_recall_precision_fscore_on_mask(self, other_node):
-        # type: (Node) -> Tuple[float, float, float]
-        """Compute the recall, precision and f-score of the predicted
-        Node's mask against another node's mask."""
-
-        if bounding_box_intersection(self.bounding_box, other_node.bounding_box) is None:
-            return 0.0, 0.0, 0.0
-
-        mask_intersection = compute_unifying_mask([(self), (other_node)], intersection=False)
-
-        gt_pasted_mask = mask_intersection * 1
-        t, l, b, r = compute_unifying_bounding_box([self, other_node])
-        h, w = b - t, r - l
-        ct, cl, cb, cr = self.top - t, \
-                         self.left - l, \
-                         h - (b - self.bottom), \
-                         w - (r - self.right)
-        gt_pasted_mask[ct:cb, cl:cr] += self.mask
-        gt_pasted_mask[gt_pasted_mask != 0] = 1
-
-        pred_pasted_mask = mask_intersection * 1
-        t, l, b, r = other_node.bounding_box
-        h, w = b - t, r - l
-        ct, cl, cb, cr = other_node.top - t, \
-                         other_node.left - l, \
-                         h - (b - other_node.bottom), \
-                         w - (r - other_node.right)
-        pred_pasted_mask[ct:cb, cl:cr] += other_node.mask
-        pred_pasted_mask[pred_pasted_mask != 0] = 1
-
-        true_positives = float(mask_intersection.sum())
-        false_positives = pred_pasted_mask.sum() - true_positives
-        false_negatives = gt_pasted_mask.sum() - true_positives
-        recall = true_positives / (true_positives + false_negatives)
-        precision = true_positives / (true_positives + false_positives)
-        f_score = (2 * recall * precision) / (recall + precision)
-
-        return recall, precision, f_score
-
-
-##############################################################################
-
-
-def split_node_by_its_connected_components(node: Node, next_node_id: int) -> List[Node]:
-    """Split the Node into one object per connected component
-    of the mask. All inlinks/outlinks are retained in all the newly
-    created Nodes, and the old object is not changed.
-    If there is only one connected component, the object is returned unchanged
-    in a list with one entry.
-
-    A ``id`` must be provided at which to start numbering the newly
-    created Nodes.
-
-    The ``data`` attribute is also retained.
-    """
-    # "Safety margin"
-    canvas = numpy.zeros((node.mask.shape[0] + 2, node.mask.shape[1] + 2))
-    canvas[1:-1, 1:-1] = node.mask
-    number_of_connected_components, labels, bounding_boxes = compute_connected_components(canvas)
-
-    logging.info('Node.split(): {0} connected components, bounding boxes: {1}'
-                 .format(number_of_connected_components, bounding_boxes))
-
-    if len(bounding_boxes) == 1:
-        return [node]
-
-    output = []
-
-    for label, (top, left, bottom, right) in list(bounding_boxes.items()):
-        # Background in compute_connected_components() doesn't work?
-        if label == 0:
-            continue
-
-        height = bottom - top
-        width = right - left
-        m_label = (labels == label).astype('uint8')
-        m = m_label[top:bottom, left:right]
-        top = top + node.top - 1
-        left = left + node.left - 1
-        node_id = next_node_id
-        inlinks = copy.deepcopy(node.inlinks)
-        outlinks = copy.deepcopy(node.outlinks)
-        data = copy.deepcopy(node.data)
-        dataset = node.dataset
-        document = node.document
-
-        new_node = Node(node_id, node.class_name, top, left, width, height,
-                        inlinks=inlinks, outlinks=outlinks,
-                        mask=m, data=data, dataset=dataset, document=document)
-        output.append(new_node)
-
-        next_node_id += 1
-
-    return output
-
-
-def merge_nodes(first_node: Node, second_node: Node, class_name: str, id_: int) -> Node:
-    """Merge the given Nodes with respect to the other.
-    Returns a new Node (without modifying any of the inputs)."""
-    return merge_multiple_nodes([first_node, second_node], class_name, id_)
-
-
-def merge_multiple_nodes(nodes: List[Node], class_name: str, id_: int) -> Node:
-    """Merge multiple nodes. Does not modify any of the inputs."""
-    if len(set([c.document for c in nodes])) > 1:
-        raise ValueError('Cannot merge Nodes from different documents!')
-    merged_top, merged_left, merged_bottom, merged_right = compute_unifying_bounding_box(nodes)
-    merged_height, merged_width = merged_bottom - merged_top, merged_right - merged_left
-    merged_mask = compute_unifying_mask(nodes)
-    merged_inlinks, merged_outlinks = merge_inlinks_and_outlinks_to_nodes_outside_of_this_list(
-        nodes)
-
-    dataset = nodes[0].dataset
-    document = nodes[0].document
-
-    output = Node(id_, class_name,
-                  top=merged_top, left=merged_left, height=merged_height, width=merged_width,
-                  mask=merged_mask,
-                  inlinks=merged_inlinks, outlinks=merged_outlinks,
-                  dataset=dataset, document=document)
-    return output
-
-
-def compute_unifying_bounding_box(nodes: List[Node]) -> (int, int, int, int):
-    """ Computes the union bounding box of multiple nodes """
-    top, left, bottom, right = numpy.inf, numpy.inf, -1, -1
-    for node in nodes:
-        top = min(top, node.top)
-        left = min(left, node.left)
-        bottom = max(bottom, node.bottom)
-        right = max(right, node.right)
-
-    it, il, ib, ir = int(top), int(left), int(bottom), int(right)
-    if (it != top) or (il != left) or (ib != bottom) or (ir != right):
-        logging.warning('Merged bounding box does not consist of integers!'
-                        ' {0}'.format((top, left, bottom, right)))
-
-    return it, il, ib, ir
-
-
-def compute_unifying_mask(nodes: List[Node], intersection=False) -> Optional[numpy.ndarray]:
-    """ Merges the masks of the given Nodes into one. Masks are combined by an OR operation.
-
-    >>> c1 = Node(0, 'name', 10, 10, 4, 1, mask=numpy.ones((1, 4), dtype='uint8'))
-    >>> c2 = Node(1, 'name', 11, 10, 6, 1, mask=numpy.ones((1, 6), dtype='uint8'))
-    >>> c3 = Node(2, 'name', 9, 14,  2, 4, mask=numpy.ones((4, 2), dtype='uint8'))
-    >>> nodes = [c1, c2, c3]
-    >>> m1 = compute_unifying_mask(nodes)
-    >>> m1.shape
-    (4, 6)
-    >>> print(m1)
-    [[0 0 0 0 1 1]
-     [1 1 1 1 1 1]
-     [1 1 1 1 1 1]
-     [0 0 0 0 1 1]]
-
-    Mask behavior: if at least one of the Nodes has a mask, then
-    masking behavior is activated. The masks are combined using OR: any
-    pixel of the resulting merged Node that corresponds to a True
-    mask pixel in one of the input Nodes will get a True mask value,
-    all others (ie. including all intermediate areas) will get a False.
-
-    If no input Node has a mask, then the resulting Node also will not have a mask.
-
-    If some Nodes have masks and some don't, this call with throw an error.
-
-    :param nodes: The list of nodes whose masks will be merged
-
-    :param intersection: Instead of a union, return the mask
-        intersection: only those pixels which are common to all
-        the Nodes.
-    """
-    no_node_has_a_mask = len([c for c in nodes if c.mask is not None]) == 0
-    if no_node_has_a_mask:
-        return None
-
-    for node in nodes:
-        if node.mask is None:
-            # Some nodes have masks and some don't
-            raise ValueError('Cannot deal with a mix of masked and non-masked Nodes.')
-
-    top, left, bottom, right = compute_unifying_bounding_box(nodes)
-    height = bottom - top
-    width = right - left
-    output_mask = numpy.zeros((height, width), dtype=nodes[0].mask.dtype)
-    for node in nodes:
-        ct, cl, cb, cr = node.top - top, node.left - left, height - (
-                bottom - node.bottom), width - (right - node.right)
-        output_mask[ct:cb, cl:cr] += node.mask
-
-    if intersection:
-        output_mask[output_mask < len(nodes)] = 0
-        output_mask[output_mask != 0] = 1
-    else:
-        output_mask[output_mask > 0] = 1
-    return output_mask
-
-
-def merge_inlinks_and_outlinks_to_nodes_outside_of_this_list(nodes: List[Node]) \
-        -> Tuple[List[int], List[int]]:
-    """Collect all inlinks and outlinks of the given set of Nodes
-    to Nodes outside of this set. The rationale for this is that
-    these given ``nodes`` will be merged into one, so relationships
-    within the set would become loops and disappear.
-
-    (Note that this is not sufficient to update the relationships upon
-    a merge, because the affected Nodess *outside* the given set
-    will need to have their inlinks/outlinks redirected to the new object.)
-
-    :returns: A tuple of lists: ``(inlinks, outlinks)``
-    """
-    all_node_ids = frozenset([node.id for node in nodes])
-    outlinks = []
-    inlinks = []
-    for c in nodes:
-        # No duplicates
-        outlinks.extend([o for o in c.outlinks
-                         if (o not in all_node_ids) and (o not in outlinks)])
-        inlinks.extend([i for i in c.inlinks
-                        if (i not in all_node_ids) and (i not in inlinks)])
-    return inlinks, outlinks
-
-
-def merge_node_lists_from_multiple_documents(node_lists: List[List[Node]]) -> List[Node]:
-    """Combines the Node lists from different documents
-    into one list, so that inlink/outlink references still work.
-    This is useful only if you want to merge two documents
-    into one (e.g., if your annotators worked on different "layers"
-    of data, and you want to merge these annotations).
-
-    This just means shifting the ``id`` (and thus inlinks
-    and outlinks). It is assumed the lists pertain to the same
-    image. Uses deepcopy to avoid exposing the original lists
-    to modification through the merged list.
-
-    Currently cannot handle precedence edges.
-
-    """
-    max_node_ids = [max([node.id for node in c_list]) for c_list in node_lists]
-    min_node_ids = [min([node.id for node in c_list]) for c_list in node_lists]
-    shift_by = [0] + [sum(max_node_ids[:i]) - min_node_ids[i] + 1 for i in
-                      range(1, len(max_node_ids))]
-
-    new_lists = []
-    for nodes, s in zip(node_lists, shift_by):
-        new_list = []
-        for node in nodes:
-            new_node = copy.deepcopy(node)
-            new_id = node.id + s
-            new_node.set_id(new_id)
-
-            # Graph handling
-            new_node.inlinks = [i + s for i in node.inlinks]
-            new_node.outlinks = [o + s for o in node.outlinks]
-
-            new_list.append(new_node)
-        new_lists.append(new_list)
-
-    output = list(itertools.chain(*new_lists))
-
-    return output
-
-
-def link_nodes(from_node: Node, to_node: Node, check_that_nodes_have_the_same_document: bool = True):
-    """Add a relationship from one node to the other. Updates the nodes in-place.
-
-    If the objects are already linked, does nothing.
-    """
-    if from_node.document != to_node.document:
-        if check_that_nodes_have_the_same_document:
-            raise ValueError('Cannot link two Nodes that are')
-        else:
-            logging.warning('Attempting to link Nodes from two different'
-                            ' docments. From: {0}, to: {1}'
-                            ''.format(from_node.document, to_node.document))
-
-    if (to_node.id not in from_node.outlinks) and (from_node.id in to_node.inlinks):
-        logging.warning('Malformed object graph in document {0}:'
-                        ' Relationship {1} --> {2} already exists as inlink,'
-                        ' but not as outlink!.'
-                        ''.format(from_node.document, from_node.id, to_node.id))
-    from_node.outlinks.append(to_node.id)
-    to_node.inlinks.append(from_node.id)
-
-
-def bounding_box_intersection(first_bounding_box: Tuple[int, int, int, int],
-                              second_bounding_box: Tuple[int, int, int, int]) -> Optional[
-    Tuple[int, int, int, int]]:
-    """Returns the t, l, b, r coordinates of the sub-bounding box
-    of bbox_this that is also inside bbox_other.
-    If the bounding boxes do not overlap, returns None."""
-    t, l, b, r = second_bounding_box
-    tt, tl, tb, tr = first_bounding_box
-
-    out_top = max(t, tt)
-    out_bottom = min(b, tb)
-    out_left = max(l, tl)
-    out_right = min(r, tr)
-
-    if (out_top < out_bottom) and (out_left < out_right):
-        return out_top - tt, \
-               out_left - tl, \
-               out_bottom - tt, \
-               out_right - tl
-    else:
-        return None
-
-
-def bounding_box_dice_coefficient(first_bounding_box: Tuple[int, int, int, int],
-                                  second_bounding_box: Tuple[int, int, int, int],
-                                  vertical: bool = False,
-                                  horizontal: bool = False) -> float:
-    """Compute the Dice coefficient (intersection over union)
-    for the given two bounding boxes.
-
-    :param vertical: If set, will only return vertical IoU.
-
-    :param horizontal: If set, will only return horizontal IoU.
-        If both vertical and horizontal are set, will return
-        normal IoU, as if they were both false.
-    """
-    t_t, t_l, t_b, t_r = first_bounding_box
-    o_t, o_l, o_b, o_r = second_bounding_box
-
-    u_t, i_t = min(t_t, o_t), max(t_t, o_t)
-    u_l, i_l = min(t_l, o_l), max(t_l, o_l)
-    u_b, i_b = max(t_b, o_b), min(t_b, o_b)
-    u_r, i_r = max(t_r, o_r), min(t_r, o_r)
-
-    u_vertical = max(0, u_b - u_t)
-    u_horizontal = max(0, u_r - u_l)
-
-    i_vertical = max(0, i_b - i_t)
-    i_horizontal = max(0, i_r - i_l)
-
-    if vertical and not horizontal:
-        if u_vertical == 0:
-            return 0.0
-        else:
-            return i_vertical / u_vertical
-    elif horizontal and not vertical:
-        if u_horizontal == 0:
-            return 0.0
-        else:
-            return i_horizontal / u_horizontal
-    else:
-        if (u_horizontal == 0) or (u_vertical == 0):
-            return 0.0
-        else:
-            return (i_horizontal * i_vertical) / (u_horizontal * u_vertical)
-
-
-def draw_nodes_on_empty_canvas(nodes: List[Node], margin: int = 10) -> Tuple[
-    numpy.ndarray, Tuple[int, int]]:
-    """Draws all the given Nodes onto a zero background.
-    The size of the canvas adapts to the Nodes, with the    given margin.
-
-    Also returns the top left corner coordinates w.r.t. Nodes' bounding boxes.
-    """
-
-    # margin is used to avoid the stafflines touching the edges,
-    # which could perhaps break some assumptions down the line.
-    top, left, bottom, right = compute_unifying_bounding_box(nodes)
-    top_with_margin, left_with_margin, bottom_with_margin, right_with_margin = \
-        max(0, top - margin), max(0, left - margin), bottom + margin, right + margin
-
-    canvas = numpy.zeros(
-        (bottom_with_margin - top_with_margin, right_with_margin - left_with_margin))
-
-    for node in nodes:
-        canvas[node.top - top_with_margin:node.bottom - top_with_margin,
-        node.left - left_with_margin:node.right - left_with_margin] = node.mask * 1
-
-    canvas[canvas != 0] = 1
-
-    return canvas, (top_with_margin, left_with_margin)
+import copy
+import itertools
+import logging
+from typing import List, Union, Tuple, Optional, Any
+
+import numpy
+from math import ceil
+
+from mung.utils import compute_connected_components
+
+
+class Node(object):
+    """One annotated object.
+
+    The Node represents one instance of an annotation. It implements
+    the following attributes:
+
+    * ``node_id``: the unique number of the given annotation instance in the set
+      of annotations encoded in the containing `NodeList`.
+    * ``dataset``: the name of the dataset this Node belongs to, e.g., MUSCIMA++_2.0
+    * ``document``: the name of the document this Node belongs to, e.g., CVC-MUSCIMA_W-05_N-19_D-ideal
+    * ``class_name``: the name of the label that was given to the annotation
+      (this is the human-readable string such as ``notehead-full``).
+    * ``top``: the vertical dimension (row) of the upper left corner pixel.
+    * ``left``: the horizontal dimension (column) of the upper left corner pixel.
+    * ``bottom``: the vertical dimension (row) of the lower right corner pixel + 1,
+      so that you can index the corresponding image rows using
+      ``img[c.top:c.bottom]``.
+    * ``right``: the horizontal dimension (row) of the lower right corner pixel + 1,
+      so that you can index the corresponding image columns using
+      ``img[:, c.left:c.right]``.
+    * ``width``: the amount of rows that the Node spans.
+    * ``height``: the amount of columns that the Node spans.
+    * ``mask``: a binary (0/1) numpy array that denotes the area within the
+      Node's bounding box (specified by ``top``, ``left``, ``height``
+      and ``width``) that the Node actually occupies. If the mask is
+      ``None``, the object is understood to occupy the entire bounding box.
+    * ``data``: a dictionary that can be empty, or can contain anything. It is
+      generated from the optional ``<Data>`` element of a Node.
+
+    Constructing a simple Node that consists of the "b"-like flat music
+    notation symbol (never mind the ``unique_id`` for now):
+
+    >>> top = 10
+    >>> left = 15
+    >>> height = 10
+    >>> width = 4
+    >>> mask = numpy.array([[1, 1, 0, 0],
+    ...                     [1, 0, 0, 0],
+    ...                     [1, 0, 0, 0],
+    ...                     [1, 0, 0, 0],
+    ...                     [1, 0, 1, 1],
+    ...                     [1, 1, 1, 1],
+    ...                     [1, 0, 0, 1],
+    ...                     [1, 0, 1, 1],
+    ...                     [1, 1, 1, 0],
+    ...                     [0, 1, 0, 0]])
+    >>> class_name = 'flat'
+    >>> dataset = 'MUSCIMA-pp_2.0'
+    >>> document = 'CVC-MUSCIMA_W-35_N-08_D-ideal'
+    >>> node = Node(611, class_name=class_name,
+    ...                top=top, left=left, height=height, width=width,
+    ...                inlinks=[], outlinks=[],
+    ...                mask=mask,
+    ...                dataset=dataset, document=document)
+
+    Nodes can also form graphs, using the following attributes:
+
+    * ``outlinks``: Outgoing edges. A list of integers; it is assumed they are
+      valid ``node_id`` within the same global/doc namespace.
+    * ``inlinks``: Incoming edges. A list of integers; it is assumed they are
+      valid ``node_id`` within the same global/doc namespace.
+
+    So far, Node graphs do not support multiple relationship types.
+
+    **Unique identification**
+
+    The ``unique_id`` serves to identify the Node uniquely,
+    at least within the MUSCIMA dataset system. (We anticipate further
+    versions of the dataset, and need to plan for that.)
+
+    To uniquely identify a Node, there are three "levels":
+
+    * The "global", **dataset-level identification**: which dataset is this
+      Node coming from? (For this dataset: ``MUSCIMA++_1.0``)
+    * The "local", **document-level identification**: which document
+      (within the given dataset) is this Node coming from?
+      For MUSCIMA++ 1.0, this will usually be a string like
+      ``CVC-MUSCIMA_W-35_N-08_D-ideal``, derived from the filename
+      under which the Nodes containing the given Node
+      is stored.
+    * The **within-document identification**, which is the ``node_id``.
+
+    These three components are joined together into one string by
+    a delimiter: ``___``
+
+    The full ``unique_id`` of a Node then might look like this::
+    >>> node.unique_id
+    'MUSCIMA-pp_2.0___CVC-MUSCIMA_W-35_N-08_D-ideal___611'
+
+    And it consists of these three parts:
+
+    >>> node.document
+    'CVC-MUSCIMA_W-35_N-08_D-ideal'
+    >>> node.dataset
+    'MUSCIMA-pp_2.0'
+    >>> node.id
+    611
+
+    **Nodes and images**
+
+    Nodes and images are not tightly bound. This is because the same
+    object can apply to multiple images: in the case of the CVC-MUSCIMA dataset,
+    for example, the same Nodes are present both in the full image
+    and in the staff-less image. The limitation here is that Nodes
+    are based on exact pixels, so in order to retain validity, the images
+    must correspond to each other exactly, as "layers".
+
+    Because Nodes do not correspond to any given image, there is
+    no facility in the data format to link them to a specific one. You have to
+    take care of matching Node annotations to the right images by yourself.
+
+    The ``Node`` class implements some interactions with images.
+
+    To recover the area corresponding to a Node `c`, use:
+
+    >>> image = numpy.array([]) #doctest: +SKIP
+    >>> if node.mask is not None: crop = image[node.top:node.bottom, node.left:node.right] * node.mask  #doctest: +SKIP
+    >>> if node.mask is None: crop = image[node.top:node.bottom, node.left:node.right]               #doctest: +SKIP
+
+    Because this is clunky, we have implemented the following to get the crop:
+
+    >>> crop = node.project_to(image)    #doctest: +SKIP
+
+    And to get the Node projected onto the entire image:
+
+    >>> crop = node.project_on(image)    #doctest: +SKIP
+
+    Above, note the multiplicative role of the mask: while we typically would
+    expect the mask to be binary, in principle, this is not strictly necessary.
+    You could supply a different mask interpration, such as probabilistic.
+    However, we strongly advise not to misuse this feature unless you have
+    a really good reason; remember that the Node is supposed to represent
+    an annotation of a given image. (One possible use for a non-binary mask
+    that we can envision is aggregating multiple annotations of the same
+    image.)
+
+    For visualization, there is a more sophisticated method that renders
+    the Node as a transparent colored transparent rectangle over
+    an RGB image. (NOTE: this really changes the input image!)
+
+    >>> import matplotlib.pyplot as plt #doctest: +SKIP
+    >>> node.render(image)           #doctest: +SKIP
+    >>> plt.imshow(image); plt.show() #doctest: +SKIP
+
+    However, `Node.render()` currently does not support rendering
+    the mask.
+
+    **Disambiguating class names**
+
+    Since the class names are present
+    through the ``class_name`` attribute (``<ClassName>`` element),
+    matching the list is no longer necessary for general understanding
+    of the file. The NodeClasses file serves as a disambiguation tool:
+    there may be multiple annotation projects that use the same names
+    but maybe define them differently and use different guidelines,
+    and their respective NodeClasses allow you to interpret the symbol
+    names correctly, in light of the corresponding set of definitions.
+
+    .. note::
+
+        In MUSCIMarker, the NodeClasses is currently necessary to define
+        how Nodes are displayed: their color. (All noteheads are red,
+        all barlines are green, etc.) The other function, matching names
+        to ``clsid``, has been superseeded by the ``class_name`` Node
+        attribute.
+
+    **Merging Nodes**
+
+    To merge a list of Nodes into a new one, you need to:
+
+    * Compute the new object's bounding box: ``compute_unifying_bounding_box()``
+    * Compute the new object's mask: ``compute_unifying_mask()``
+    * Determine the class_name and node_id of the new object.
+
+    Since node_id and class_name of merges may depend on external settings
+    and generally cannot be reliably determined from the merged
+    objects themselves (e.g. the merge of a notehead and a stem
+    should be a new note symbol), you need to supply them externally.
+    However, the bounding box and mask can be determined. The bounding
+    box is computed simply as the smallest bounding box that
+    encompasses all the Nodes, and the mask is an OR operation
+    over the individual masks (or None, if the Nodes don't
+    have masks). Note that the merge cannot deal with a situation
+    where only some of the objects have a mask.
+
+    **Implementation notes on the mask**
+
+    The mask is a numpy array that will be saved using run-length encoding.
+    The numpy array is first flattened, then runs of successive 0's and 1's
+    are encoded as e.g. ``0:10`` for a run of 10 zeros.
+
+    How much space does this take?
+
+    Objects tend to be relatively convex, so after flattening, we can expect
+    more or less two runs per row (flattening is done in ``C`` order). Because
+    each run takes (approximately) 5 characters, each mask takes roughly ``5 * n_rows``
+    bytes to encode. This makes it efficient for objects wider than 5 pixels, with
+    a compression ratio approximately ``n_cols / 5``.
+    (Also, the numpy array needs to be made C-contiguous for that, which
+    explains the ``order='C'`` hack in ``set_mask()``.)
+    """
+
+    # Delimits the Node UID fields (global, document namespaces, id)
+    UID_DELIMITER = '___'
+    DEFAULT_DATASET = 'MUSCIMA_DEFAULT_DATASET_PLACEHOLDER'
+    DEFAULT_DOCUMENT = 'default-document'
+
+    def __init__(self, id_: int,
+                 class_name: str,
+                 top: int,
+                 left: int,
+                 width: int,
+                 height: int,
+                 outlinks: List[int] = None,
+                 inlinks: List[int] = None,
+                 mask: numpy.ndarray = None,
+                 dataset: str = None,
+                 document: str = None,
+                 data=None):
+        self.__id = id_
+        self.__class_name = class_name
+        self.__top = top
+        self.__left = left
+        self.__width = width
+        self.__height = height
+
+        # The mask presupposes integer bounds.
+        # Applied relative to Node bounds, not the whole image.
+        self.__to_integer_bounds()
+        self.__mask = None
+        self.set_mask(mask)
+
+        if inlinks is None:
+            inlinks = []
+        self.inlinks = inlinks  # type: List[int]
+
+        if outlinks is None:
+            outlinks = []
+        self.outlinks = outlinks  # type: List[int]
+
+        if dataset is None:
+            dataset = self.DEFAULT_DATASET
+        self.__dataset = dataset
+
+        if document is None:
+            document = self.DEFAULT_DOCUMENT
+        self.__document = document
+
+        self.is_selected = False
+
+        if data is None:
+            data = dict()
+        self.data = data
+
+    @property
+    def unique_id(self) -> str:
+        """Returns the ``unique_id`` of this Node
+
+        >>> node = Node(0, "", 0, 0, 0, 0)
+        >>> node.unique_id
+        'MUSCIMA_DEFAULT_DATASET_PLACEHOLDER___default-document___0'
+        """
+        return self.UID_DELIMITER.join([self.dataset,
+                                        self.document,
+                                        str(self.id)])
+
+    @staticmethod
+    def parse_unique_id(uid: str) -> (str, str, int):
+        """Parse a unique identifier. This breaks down the UID into the dataset name,
+        document name, and id
+
+        The delimiter is expected to be ``___``
+        (kept as ``Node.UID_DELIMITER``)
+
+        >>> Node.parse_unique_id('MUSCIMA++_2.0___CVC-MUSCIMA_W-05_N-19_D-ideal___424')
+        ('MUSCIMA++_2.0', 'CVC-MUSCIMA_W-05_N-19_D-ideal', 424)
+
+        :returns: ``global_namespace, document_namespace, id`` triplet.
+            The namespaces are strings, ``id`` is an integer. If ``unique_id``
+            is ``None``, returns ``None`` as ``id`` and expects it
+            to be filled in from the caller Node instance.
+        """
+        if uid is None:
+            global_namespace = Node.DEFAULT_DATASET
+            document_namespace = Node.DEFAULT_DOCUMENT
+            node_id = None
+        else:
+            global_namespace, document_namespace, node_id_string = uid.split(Node.UID_DELIMITER)
+            node_id = int(node_id_string)
+        return global_namespace, document_namespace, node_id
+
+    @property
+    def id(self) -> int:
+        return self.__id
+
+    def set_id(self, id_):
+        self.__id = id_
+
+    @property
+    def class_name(self) -> str:
+        return self.__class_name
+    
+    def set_class_name(self, class_name_):
+        self.__class_name = class_name_
+
+    @property
+    def dataset(self) -> str:
+        return self.__dataset
+
+    @property
+    def document(self) -> str:
+        return self.__document
+
+    @property
+    def top(self) -> int:
+        """Row coordinate of upper left corner."""
+        return self.__top
+
+    @property
+    def bottom(self) -> int:
+        """Row coordinate 1 beyond bottom right corner, so that indexing
+        in the form ``img[node.top:node.bottom]`` is possible."""
+        return self.__top + self.__height
+
+    @property
+    def left(self) -> int:
+        """Column coordinate of upper left corner."""
+        return self.__left
+
+    @property
+    def right(self) -> int:
+        """Column coordinate 1 beyond bottom right corner, so that indexing
+        in the form ``img[:, node.left:node.right]`` is possible."""
+        return self.__left + self.__width
+
+    @property
+    def width(self) -> int:
+        return self.__width
+
+    @property
+    def height(self) -> int:
+        return self.__height
+
+    @property
+    def bounding_box(self) -> Tuple[int, int, int, int]:
+        """The ``top, left, bottom, right`` tuple of the Node's coordinates."""
+        return self.top, self.left, self.bottom, self.right
+
+    @property
+    def middle(self) -> Tuple[int, int]:
+        """Returns the integer representation of where the middle
+        of the Node lies, as a ``(m_vert, m_horz)`` tuple.
+
+        The integers just get rounded down.
+
+        >>> node = Node(0,'', 10, 20, 30, 40)
+        >>> node.middle
+        (30, 35)
+        """
+        vertical_center = self.top + self.height // 2
+        horizontal_center = self.left + self.width // 2
+        return int(vertical_center), int(horizontal_center)
+
+    @property
+    def mask(self) -> numpy.ndarray:
+        return self.__mask
+
+    def set_mask(self, mask: numpy.ndarray):
+        """Sets the Node's mask to the given array. Performs
+        some compatibility checks: size, dtype (converts to ``uint8``)."""
+        if mask is None:
+            self.__mask = None
+        else:
+            # Check dimension
+            t, l, b, r = self.round_bounding_box_to_integer(self.top,
+                                                            self.left,
+                                                            self.bottom,
+                                                            self.right)
+            if mask.shape != (b - t, r - l):
+                raise ValueError('Mask shape {0} does not correspond'
+                                 ' to integer shape {1} of Node.'
+                                 ''.format(mask.shape, (b - t, r - l)))
+            if str(mask.dtype) != 'uint8':
+                logging.debug('Node.set_mask(): Supplied non-integer mask'
+                              ' with dtype={0}'.format(mask.dtype))
+
+            self.__mask = mask.astype('uint8')
+
+    @staticmethod
+    def round_bounding_box_to_integer(top: float, left: float, bottom: float, right: float) \
+            -> (int, int, int, int):
+        """Rounds off the Node bounds to the nearest integer
+        so that no area is lost (e.g. bottom and right bounds are
+        rounded up, top and left bounds are rounded down).
+
+        Returns the rounded-off integers (top, left, bottom, right)
+        as integers.
+
+        >>> Node.round_bounding_box_to_integer(44.2, 18.9, 55.1, 92.99)
+        (44, 18, 56, 93)
+        >>> Node.round_bounding_box_to_integer(44, 18, 56, 92.99)
+        (44, 18, 56, 93)
+
+        """
+        return int(top), int(left), int(ceil(bottom)), int(ceil(right))
+
+    def project_to(self, image: numpy.ndarray):
+        """This function returns the *crop* of the input image
+        corresponding to the Node (incl. masking).
+        Assumes zeros are background."""
+        # Make a copy! We don't want to modify the original image by the mask.
+        # Copy forced by the "* 1" part.
+        crop = image[self.top:self.bottom, self.left:self.right] * 1
+        if self.__mask is not None:
+            crop *= self.__mask
+        return crop
+
+    def project_on(self, image: numpy.ndarray):
+        """This function returns only those parts of the input image
+        that correspond to the Node and masks out everything else
+        with zeros. The dimension of the returned array is the same
+        as of the input image. This function basically reconstructs
+        the symbol as an indicator function over the pixels of
+        the annotated image."""
+        output = numpy.zeros(image.shape, image.dtype)
+        crop = self.project_to(image)
+        output[self.top:self.bottom, self.left:self.right] = crop
+        return output
+
+    def render(self, image: numpy.ndarray, alpha: float = 0.3,
+               rgb: Tuple[float, float, float] = (1.0, 0.0, 0.0)) -> numpy.ndarray:
+        """Renders itself upon the given image as a rectangle
+        of the given color and transparency. Might help visualization.
+        """
+        color = numpy.array(rgb)
+        logging.debug('Rendering object {0}, class_name {1}, t/b/l/r: {2}'
+                      ''.format(self.id, self.class_name,
+                                (self.top, self.bottom, self.left, self.right)))
+        # logging.debug('Shape: {0}'.format((self.height, self.width, 3)))
+        mask = numpy.ones((self.__height, self.__width, 3)) * color
+        crop = image[self.top:self.bottom, self.left:self.right]
+        # logging.debug('Mask done, creating crop')
+        logging.debug('Shape: {0}. Got crop. Crop shape: {1}, img shape: {2}'
+                      ''.format((self.__height, self.__width, 3), crop.shape, image.shape))
+        mix = (crop + alpha * mask) / (1 + alpha)
+
+        image[self.top:self.bottom, self.left:self.right] = mix
+        return image
+
+    def overlaps(self, bounding_box_or_node):
+        # type: (Union[Tuple[int, int, int, int], Node]) -> bool
+        """Check whether this Node overlaps the given bounding box or Node.
+
+        >>> node = Node(0, 'test', 10, 100, height=20, width=10)
+        >>> node.bounding_box
+        (10, 100, 30, 110)
+        >>> node.overlaps((10, 100, 30, 110))  # Exact match
+        True
+        >>> node.overlaps((0, 100, 8, 110))    # Row mismatch
+        False
+        >>> node.overlaps((10, 0, 30, 89))     # Column mismatch
+        False
+        >>> node.overlaps((0, 0, 8, 89))       # Total mismatch
+        False
+        >>> node.overlaps((9, 99, 31, 111))    # Encompasses Node
+        True
+        >>> node.overlaps((11, 101, 29, 109))  # Within Node
+        True
+        >>> node.overlaps((9, 101, 31, 109))   # Encompass horz., within vert.
+        True
+        >>> node.overlaps((11, 99, 29, 111))   # Encompasses vert., within horz.
+        True
+        >>> node.overlaps((11, 101, 31, 111))  # Corner within: top left
+        True
+        >>> node.overlaps((11, 99, 31, 109))   # Corner within: top right
+        True
+        >>> node.overlaps((9, 101, 29, 111))   # Corner within: bottom left
+        True
+        >>> node.overlaps((9, 99, 29, 109))    # Corner within: bottom right
+        True
+
+        """
+        if isinstance(bounding_box_or_node, Node):
+            t, l, b, r = bounding_box_or_node.bounding_box
+        else:
+            t, l, b, r = bounding_box_or_node
+        # Does it overlap vertically? Includes situations where the Node is inside the bounding box.
+        # Note that the bottom is +1 (fencepost), so the checks bottom vs. top need to be "less than",
+        # not leq. If one object's top would be equal to the other's bottom, they would be touching,
+        # not overlapping.
+        if max(t, self.top) < min(b, self.bottom):
+            if max(l, self.left) < min(r, self.right):
+                return True
+        return False
+
+    def contains(self, bounding_box_or_node):
+        # type: (Union[Tuple[int, int, int, int], Node]) -> bool
+        """Check if this Node entirely contains the other bounding
+        box (or, the other node's bounding box)."""
+        if isinstance(bounding_box_or_node, Node):
+            top, left, bottom, right = bounding_box_or_node.bounding_box
+        else:
+            top, left, bottom, right = bounding_box_or_node
+
+        if self.top <= top <= bottom <= self.bottom:
+            if self.left <= left <= right <= self.right:
+                return True
+        return False
+
+    def bounding_box_intersection(self, bounding_box: Tuple[int, int, int, int]) \
+            -> Optional[Tuple[int, int, int, int]]:
+        """Returns the sub-bounding box of this Node intersecting with the given bounding box.
+        If the intersection is empty, returns None.
+
+        >>> node = Node(0, 'test', 10, 100, height=20, width=10)
+        >>> node.bounding_box
+        (10, 100, 30, 110)
+        >>> other_bbox = 20, 100, 40, 105
+        >>> node.bounding_box_intersection(other_bbox)
+        (10, 0, 20, 5)
+        >>> containing_bbox = 4, 55, 44, 115
+        >>> node.bounding_box_intersection(containing_bbox)
+        (0, 0, 20, 10)
+        >>> contained_bbox = 12, 102, 22, 108
+        >>> node.bounding_box_intersection(contained_bbox)
+        (2, 2, 12, 8)
+        >>> non_overlapping_bbox = 0, 0, 3, 3
+        >>> node.bounding_box_intersection(non_overlapping_bbox) is None
+        True
+
+        """
+        t, l, b, r = bounding_box
+
+        out_top = max(t, self.top)
+        out_bottom = min(b, self.bottom)
+        out_left = max(l, self.left)
+        out_right = min(r, self.right)
+
+        if (out_top < out_bottom) and (out_left < out_right):
+            return out_top - self.top, \
+                   out_left - self.left, \
+                   out_bottom - self.top, \
+                   out_right - self.left
+        else:
+            return None
+
+    def crop_to_mask(self):
+        """Crops itself to the minimum bounding box that contains all
+        its pixels, as determined by its mask.
+
+        If the mask is all zeros, does not do anything, because
+        at this point, the is_empty check should be invoked anyway
+        in any situation where you care whether the object is empty
+        or not (e.g. delete it after trimming).
+
+        >>> mask = numpy.zeros((20, 10))
+        >>> mask[5:15, 3:8] = 1
+        >>> node = Node(0, 'test', 10, 100, width=10, height=20, mask=mask)
+        >>> node.bounding_box
+        (10, 100, 30, 110)
+        >>> node.crop_to_mask()
+        >>> node.bounding_box
+        (15, 103, 25, 108)
+        >>> node.height, node.width
+        (10, 5)
+
+        Assumes integer bounds, which is ensured during Node initialization.
+        """
+        if self.__mask is None:
+            return
+
+        mask_is_empty = self.__mask.sum() == 0
+        if mask_is_empty:
+            return
+
+        # We know the object is not empty.
+
+        # How many rows/columns to trim from top, bottom, etc.
+        trim_top = -1
+        for i in range(self.__mask.shape[0]):
+            if self.__mask[i, :].sum() != 0:
+                trim_top = i
+                break
+
+        trim_left = -1
+        for j in range(self.__mask.shape[1]):
+            if self.__mask[:, j].sum() != 0:
+                trim_left = j
+                break
+
+        trim_bottom = -1
+        for k in range(self.__mask.shape[0]):
+            if self.__mask[-(k + 1), :].sum() != 0:
+                trim_bottom = k
+                break
+
+        trim_right = -1
+        for l in range(self.__mask.shape[1]):
+            if self.__mask[:, -(l + 1)].sum() != 0:
+                trim_right = l
+                break
+
+        logging.debug('Node.crop: Trimming top={0}, left={1},'
+                      'bottom={2}, right={3}'
+                      ''.format(trim_top, trim_left, trim_bottom, trim_right))
+
+        # new bounding box relative to the current bounding box -- used to trim
+        # the mask
+        rel_t = trim_top
+        rel_l = trim_left
+        rel_b = self.__height - trim_bottom
+        rel_r = self.__width - trim_right
+
+        new_mask = self.__mask[rel_t:rel_b, rel_l:rel_r] * 1
+
+        logging.debug('Node.crop: Old mask shape {0}, new mask shape {1}'
+                      ''.format(self.__mask.shape, new_mask.shape))
+
+        # new bounding box, relative to image -- used to compute the Node's position and size
+        abs_t = self.top + trim_top
+        abs_l = self.left + trim_left
+        abs_b = self.bottom - trim_bottom
+        abs_r = self.right - trim_right
+
+        self.__top = abs_t
+        self.__left = abs_l
+        self.__height = abs_b - abs_t
+        self.__width = abs_r - abs_l
+
+        self.set_mask(new_mask)
+
+    def __str__(self):
+        """Format the Node as string representation. See the documentation
+        of :module:`mung.io` for details."""
+        lines = []
+        lines.append('<Node>')
+        lines.append('\t<Id>{0}</Id>'.format(self.id))
+        lines.append('\t<ClassName>{0}</ClassName>'.format(self.class_name)) # TODO change this if relevant for final XML notation 
+        lines.append('\t<Top>{0}</Top>'.format(self.top))
+        lines.append('\t<Left>{0}</Left>'.format(self.left))
+        lines.append('\t<Width>{0}</Width>'.format(self.__width))
+        lines.append('\t<Height>{0}</Height>'.format(self.__height))
+
+        mask_string = self.encode_mask()
+        lines.append('\t<Mask>{0}</Mask>'.format(mask_string))
+
+        if len(self.inlinks) > 0:
+            inlinks_string = ' '.join(list(map(str, self.inlinks)))
+            lines.append('\t<Inlinks>{0}</Inlinks>'.format(inlinks_string))
+        if len(self.outlinks) > 0:
+            outlinks_string = ' '.join(list(map(str, self.outlinks)))
+            lines.append('\t<Outlinks>{0}</Outlinks>'.format(outlinks_string))
+
+        data_string = self.encode_data()
+        if data_string is not None:
+            lines.append('\t<Data>\n{0}\n\t</Data>'.format(data_string))
+
+        lines.append('</Node>')
+        return '\n'.join(lines)
+
+    def encode_mask(self, mode: str = 'rle') -> str:
+        """Encode a binary array ``mask`` as a string, compliant
+        with the Node format specification in :mod:`mung.io`.
+        """
+        if mode == 'rle':
+            return self.encode_mask_rle(self.mask)
+        elif mode == 'bitmap':
+            return self.encode_mask_bitmap(self.mask)
+
+    def encode_data(self) -> Optional[str]:
+        if self.data is None:
+            return None
+        if len(self.data) == 0:
+            return None
+
+        lines = []
+        for k, v in list(self.data.items()):
+            vtype = 'str'
+            vval = v
+            if isinstance(v, int):
+                vtype = 'int'
+                vval = str(v)
+            elif isinstance(v, float):
+                vtype = 'float'
+                vval = str(v)
+            elif isinstance(v, list):
+                vtype = 'list[str]'
+                if len(v) > 0:
+                    if isinstance(v[0], int):
+                        vtype = 'list[int]'
+                    elif isinstance(v[0], float):
+                        vtype = 'list[float]'
+                vval = ' '.join([str(vv) for vv in v])
+
+            line = '\t\t<DataItem key="{0}" type="{1}">{2}</DataItem>' \
+                   ''.format(k, vtype, vval)
+            lines.append(line)
+
+        return '\n'.join(lines)
+
+    def data_display_text(self) -> str:
+        if self.data is None:
+            return '[No data]'
+        if len(self.data) == 0:
+            return '[No data]'
+
+        lines = []
+        for k, v in list(self.data.items()):
+            lines.append('{0}:      {1}'.format(k, v))
+        return '\n'.join(lines)
+
+    @staticmethod
+    def encode_mask_bitmap(mask: numpy.ndarray) -> str:
+        """Encodes the mask array in a compact form. Returns 'None' if mask
+        is None. If the mask is not None, uses the following algorithm:
+
+        * Flatten the mask (then use width and height of Node for reshaping).
+        * Record as string, with whitespace separator
+        * Return resulting string
+        """
+        if mask is None:
+            return 'None'
+        # By default works in row-major order.
+        # So we can just prescribe 'C' without losing data.
+        mask_flat = mask.flatten(order='C')
+        output = ' '.join(list(map(str, mask_flat)))
+        return output
+
+    @staticmethod
+    def encode_mask_rle(mask: numpy.ndarray) -> str:
+        """Encodes the mask array in Run-Length Encoding. Instead of
+        having the bitmap ``0 0 1 1 1 0 0 0 1 1``, the RLE encodes
+        the mask as ``0:2 1:3 0:3 1:2``. This is much more compact.
+
+        Currently, the rows of the mask are not treated in any special
+        way. The mask just gets flattened and then encoded.
+
+        """
+        if mask is None:
+            return 'None'
+        mask_flat = mask.flatten(order='C')
+
+        output_strings = []
+        current_run_type = 0
+        current_run_length = 0
+        for i in mask_flat:
+            if i == current_run_type:
+                current_run_length += 1
+            else:
+                s = '{0}:{1}'.format(current_run_type, current_run_length)
+                output_strings.append(s)
+                current_run_type = i
+                current_run_length = 1
+        s = '{0}:{1}'.format(current_run_type, current_run_length)
+        output_strings.append(s)
+        output = ' '.join(output_strings)
+        return output
+
+    @staticmethod
+    def decode_mask(mask_string: str, shape) -> Optional[numpy.ndarray]:
+        """Decodes a Node mask string into a binary
+        numpy array of the given shape."""
+        mode = Node.__determine_mask_mode(mask_string)
+        if mode == 'rle':
+            return Node.decode_mask_rle(mask_string, shape=shape)
+        elif mode == 'bitmap':
+            return Node.decode_mask_bitmap(mask_string, shape=shape)
+
+    @staticmethod
+    def __determine_mask_mode(mask_string: str):
+        """If the mask string starts with '0:' or '1:', or generally
+        if it contains a non-0 or 1 symbol, assume it is RLE."""
+        mode = 'bitmap'
+        if len(mask_string) < 3:
+            mode = 'bitmap'
+        elif ':' in mask_string[:3]:
+            mode = 'rle'
+        return mode
+
+    @staticmethod
+    def decode_mask_bitmap(mask_string: str, shape) -> Optional[numpy.ndarray]:
+        """Decodes the mask array from the encoded form to the 2D numpy array."""
+        if mask_string == 'None':
+            return None
+        try:
+            values = list(map(float, mask_string.split()))
+        except ValueError:
+            logging.info(
+                'Node.decode_mask_bitmap() Cannot decode mask values:\n{0}'.format(mask_string))
+            raise
+        mask = numpy.array(values).reshape(shape)
+        return mask
+
+    @staticmethod
+    def decode_mask_rle(mask_string: str, shape) -> Optional[numpy.ndarray]:
+        """Decodes the mask array from the RLE-encoded form
+        to the 2D numpy array.
+        """
+        if mask_string == 'None':
+            return None
+
+        mask_flat = numpy.zeros(shape[0]*shape[1], numpy.uint8)
+        index = 0
+        for kv in mask_string.split(' '):
+            k_string, v_string = kv.split(':')
+            k, v = int(k_string), int(v_string)
+            if k == 1:
+                mask_flat[index:index+v] = 1
+            index += v
+
+        mask = mask_flat.reshape(shape)
+        return mask
+
+    def join(self, other):
+        """Node "addition": performs an OR on this
+        and the ``other`` Nodes' masks and bounding boxes,
+        and assigns to this Node the result. Merges
+        also the inlinks and outlinks.
+
+        Works only if the document spaces for both Nodes
+        are the same. (Otherwise changes nothing.)
+
+        The ``class_name`` of the ``other`` is ignored.
+        """
+        if self.document != other.document:
+            logging.warning(
+                "Trying to join Node from different documents, which is forbidden. Skipping join.")
+            return
+
+        # Get combined bounding box
+        new_top = min(self.top, other.top)
+        new_left = min(self.left, other.left)
+        new_bottom = max(self.bottom, other.bottom)
+        new_right = max(self.right, other.right)
+
+        new_height = new_bottom - new_top
+        new_width = new_right - new_left
+
+        # Create mask of corresponding size
+        new_mask = numpy.zeros((new_height, new_width), dtype=self.__mask.dtype)
+
+        # Find coordinates where to paste the masks
+        spt = self.top - new_top
+        spl = self.left - new_left
+        opt = other.top - new_top
+        opl = other.left - new_left
+
+        # Paste the masks into these places
+        new_mask[spt:spt + self.__height, spl:spl + self.__width] += self.__mask
+        new_mask[opt:opt + other.height, opl:opl + other.width] += other.mask
+
+        # Normalize mask value
+        new_mask[new_mask != 0] = 1
+
+        # Assign the new variables to this Node
+        self.__top = new_top
+        self.__left = new_left
+        self.__height = new_height
+        self.__width = new_width
+        self.__mask = new_mask
+
+        # Add inlinks and outlinks (check for multiple and self-reference)
+        for o in other.outlinks:
+            if (o not in self.outlinks) and (o != self.id):
+                self.outlinks.append(o)
+        for i in other.inlinks:
+            if (i not in self.inlinks) and (i != self.id):
+                self.inlinks.append(i)
+
+    def get_outlink_objects(self, nodes):
+        # type: (List[Node]) -> List[Node]
+        """Out of the given ``nodes`` list, return a list
+        of those to which this Node has outlinks.
+        Can deal with Nodes from multiple documents.
+        """
+        return self.__check_nodes_that_have_links(self.outlinks, nodes)
+
+    def get_inlink_objects(self, nodes):
+        # type: (List[Node]) -> List[Node]
+        """Out of the given ``nodes`` list, return a list
+        of those from which this node has inlinks
+        Can deal with Nodes from multiple documents.
+        """
+        return self.__check_nodes_that_have_links(self.inlinks, nodes)
+
+    def __check_nodes_that_have_links(self, links, nodes):
+        # type: (List[int], List[Node]) -> List[Node]
+        output = []
+        if len(links) == 0:
+            return output
+
+        link_set = frozenset(links)
+
+        for node in nodes:
+            if node.document != self.document:
+                continue
+            if node.id in link_set:
+                output.append(node)
+            if len(output) == len(self.inlinks):
+                break
+        return output
+
+    def translate(self, down: int = 0, right: int = 0):
+        """Move the Node down and right by the given amount of pixels."""
+        self.__top += down
+        self.__left += right
+
+    def scale(self, zoom: float = 1.0):
+        """Re-compute the Node with the given scaling factor."""
+        mask = self.__mask * 1.0
+        import skimage.transform
+        new_mask_shape = max(int(self.__height * zoom), 1), max(int(self.__width * zoom), 1)
+        new_mask = skimage.transform.resize(mask,
+                                            output_shape=new_mask_shape)
+        new_mask[new_mask >= 0.5] = 1
+        new_mask[new_mask < 0.5] = 0
+        new_mask = new_mask.astype('uint8')
+
+        new_height, new_width = new_mask.shape
+        new_top = int(self.top * zoom)
+        new_left = int(self.left * zoom)
+
+        self.__top = new_top
+        self.__left = new_left
+        self.__height = new_height
+        self.__width = new_width
+        self.__mask = new_mask
+
+    def __to_integer_bounds(self):
+        """Ensures that the Node has an integer position and size.
+        (This is important whenever you want to use a mask, and reasonable
+        whenever you do not need sub-pixel resolution...)
+        """
+        bounding_box = self.bounding_box
+        top, left, bottom, right = self.round_bounding_box_to_integer(*bounding_box)
+        height = bottom - top
+        width = right - left
+
+        self.__top = top
+        self.__left = left
+        self.__height = height
+        self.__width = width
+
+    def distance_to(self, node) -> Any:
+        """Computes the distance between this node and another node.
+        Their minimum vertical and horizontal distances are each taken
+        separately, and the euclidean norm is computed from them."""
+        if self.document != node.document:
+            logging.warning('Cannot compute distances between Nodes'
+                            ' from different documents! ({0} vs. {1})'
+                            ''.format(self.document, node.document))
+
+        if (self.top <= node.top <= self.bottom) or (node.top <= self.top <= node.bottom):
+            delta_vert = 0
+        elif self.top < node.top:
+            delta_vert = node.top - self.bottom
+        else:
+            delta_vert = self.top - node.bottom
+
+        if (self.left <= node.left <= self.right) or (node.left <= self.left <= node.right):
+            delta_horz = 0
+        elif self.left < node.left:
+            delta_horz = node.left - self.right
+        else:
+            delta_horz = self.left - node.right
+
+        return numpy.sqrt(delta_vert ** 2 + delta_horz ** 2)
+
+    def compute_recall_precision_fscore_on_mask(self, other_node):
+        # type: (Node) -> Tuple[float, float, float]
+        """Compute the recall, precision and f-score of the predicted
+        Node's mask against another node's mask."""
+
+        if bounding_box_intersection(self.bounding_box, other_node.bounding_box) is None:
+            return 0.0, 0.0, 0.0
+
+        mask_intersection = compute_unifying_mask([(self), (other_node)], intersection=False)
+
+        gt_pasted_mask = mask_intersection * 1
+        t, l, b, r = compute_unifying_bounding_box([self, other_node])
+        h, w = b - t, r - l
+        ct, cl, cb, cr = self.top - t, \
+                         self.left - l, \
+                         h - (b - self.bottom), \
+                         w - (r - self.right)
+        gt_pasted_mask[ct:cb, cl:cr] += self.mask
+        gt_pasted_mask[gt_pasted_mask != 0] = 1
+
+        pred_pasted_mask = mask_intersection * 1
+        t, l, b, r = other_node.bounding_box
+        h, w = b - t, r - l
+        ct, cl, cb, cr = other_node.top - t, \
+                         other_node.left - l, \
+                         h - (b - other_node.bottom), \
+                         w - (r - other_node.right)
+        pred_pasted_mask[ct:cb, cl:cr] += other_node.mask
+        pred_pasted_mask[pred_pasted_mask != 0] = 1
+
+        true_positives = float(mask_intersection.sum())
+        false_positives = pred_pasted_mask.sum() - true_positives
+        false_negatives = gt_pasted_mask.sum() - true_positives
+        recall = true_positives / (true_positives + false_negatives)
+        precision = true_positives / (true_positives + false_positives)
+        f_score = (2 * recall * precision) / (recall + precision)
+
+        return recall, precision, f_score
+
+
+##############################################################################
+
+
+def split_node_by_its_connected_components(node: Node, next_node_id: int) -> List[Node]:
+    """Split the Node into one object per connected component
+    of the mask. All inlinks/outlinks are retained in all the newly
+    created Nodes, and the old object is not changed.
+    If there is only one connected component, the object is returned unchanged
+    in a list with one entry.
+
+    A ``id`` must be provided at which to start numbering the newly
+    created Nodes.
+
+    The ``data`` attribute is also retained.
+    """
+    # "Safety margin"
+    canvas = numpy.zeros((node.mask.shape[0] + 2, node.mask.shape[1] + 2))
+    canvas[1:-1, 1:-1] = node.mask
+    number_of_connected_components, labels, bounding_boxes = compute_connected_components(canvas)
+
+    logging.info('Node.split(): {0} connected components, bounding boxes: {1}'
+                 .format(number_of_connected_components, bounding_boxes))
+
+    if len(bounding_boxes) == 1:
+        return [node]
+
+    output = []
+
+    for label, (top, left, bottom, right) in list(bounding_boxes.items()):
+        # Background in compute_connected_components() doesn't work?
+        if label == 0:
+            continue
+
+        height = bottom - top
+        width = right - left
+        m_label = (labels == label).astype('uint8')
+        m = m_label[top:bottom, left:right]
+        top = top + node.top - 1
+        left = left + node.left - 1
+        node_id = next_node_id
+        inlinks = copy.deepcopy(node.inlinks)
+        outlinks = copy.deepcopy(node.outlinks)
+        data = copy.deepcopy(node.data)
+        dataset = node.dataset
+        document = node.document
+
+        new_node = Node(node_id, node.class_name, top, left, width, height,
+                        inlinks=inlinks, outlinks=outlinks,
+                        mask=m, data=data, dataset=dataset, document=document)
+        output.append(new_node)
+
+        next_node_id += 1
+
+    return output
+
+
+def merge_nodes(first_node: Node, second_node: Node, class_name: str, id_: int) -> Node:
+    """Merge the given Nodes with respect to the other.
+    Returns a new Node (without modifying any of the inputs)."""
+    return merge_multiple_nodes([first_node, second_node], class_name, id_)
+
+
+def merge_multiple_nodes(nodes: List[Node], class_name: str, id_: int) -> Node:
+    """Merge multiple nodes. Does not modify any of the inputs."""
+    if len(set([c.document for c in nodes])) > 1:
+        raise ValueError('Cannot merge Nodes from different documents!')
+    merged_top, merged_left, merged_bottom, merged_right = compute_unifying_bounding_box(nodes)
+    merged_height, merged_width = merged_bottom - merged_top, merged_right - merged_left
+    merged_mask = compute_unifying_mask(nodes)
+    merged_inlinks, merged_outlinks = merge_inlinks_and_outlinks_to_nodes_outside_of_this_list(
+        nodes)
+
+    dataset = nodes[0].dataset
+    document = nodes[0].document
+
+    output = Node(id_, class_name,
+                  top=merged_top, left=merged_left, height=merged_height, width=merged_width,
+                  mask=merged_mask,
+                  inlinks=merged_inlinks, outlinks=merged_outlinks,
+                  dataset=dataset, document=document)
+    return output
+
+
+def compute_unifying_bounding_box(nodes: List[Node]) -> (int, int, int, int):
+    """ Computes the union bounding box of multiple nodes """
+    top, left, bottom, right = numpy.inf, numpy.inf, -1, -1
+    for node in nodes:
+        top = min(top, node.top)
+        left = min(left, node.left)
+        bottom = max(bottom, node.bottom)
+        right = max(right, node.right)
+
+    it, il, ib, ir = int(top), int(left), int(bottom), int(right)
+    if (it != top) or (il != left) or (ib != bottom) or (ir != right):
+        logging.warning('Merged bounding box does not consist of integers!'
+                        ' {0}'.format((top, left, bottom, right)))
+
+    return it, il, ib, ir
+
+
+def compute_unifying_mask(nodes: List[Node], intersection=False) -> Optional[numpy.ndarray]:
+    """ Merges the masks of the given Nodes into one. Masks are combined by an OR operation.
+
+    >>> c1 = Node(0, 'name', 10, 10, 4, 1, mask=numpy.ones((1, 4), dtype='uint8'))
+    >>> c2 = Node(1, 'name', 11, 10, 6, 1, mask=numpy.ones((1, 6), dtype='uint8'))
+    >>> c3 = Node(2, 'name', 9, 14,  2, 4, mask=numpy.ones((4, 2), dtype='uint8'))
+    >>> nodes = [c1, c2, c3]
+    >>> m1 = compute_unifying_mask(nodes)
+    >>> m1.shape
+    (4, 6)
+    >>> print(m1)
+    [[0 0 0 0 1 1]
+     [1 1 1 1 1 1]
+     [1 1 1 1 1 1]
+     [0 0 0 0 1 1]]
+
+    Mask behavior: if at least one of the Nodes has a mask, then
+    masking behavior is activated. The masks are combined using OR: any
+    pixel of the resulting merged Node that corresponds to a True
+    mask pixel in one of the input Nodes will get a True mask value,
+    all others (ie. including all intermediate areas) will get a False.
+
+    If no input Node has a mask, then the resulting Node also will not have a mask.
+
+    If some Nodes have masks and some don't, this call with throw an error.
+
+    :param nodes: The list of nodes whose masks will be merged
+
+    :param intersection: Instead of a union, return the mask
+        intersection: only those pixels which are common to all
+        the Nodes.
+    """
+    no_node_has_a_mask = len([c for c in nodes if c.mask is not None]) == 0
+    if no_node_has_a_mask:
+        return None
+
+    for node in nodes:
+        if node.mask is None:
+            # Some nodes have masks and some don't
+            raise ValueError('Cannot deal with a mix of masked and non-masked Nodes.')
+
+    top, left, bottom, right = compute_unifying_bounding_box(nodes)
+    height = bottom - top
+    width = right - left
+    output_mask = numpy.zeros((height, width), dtype=nodes[0].mask.dtype)
+    for node in nodes:
+        ct, cl, cb, cr = node.top - top, node.left - left, height - (
+                bottom - node.bottom), width - (right - node.right)
+        output_mask[ct:cb, cl:cr] += node.mask
+
+    if intersection:
+        output_mask[output_mask < len(nodes)] = 0
+        output_mask[output_mask != 0] = 1
+    else:
+        output_mask[output_mask > 0] = 1
+    return output_mask
+
+
+def merge_inlinks_and_outlinks_to_nodes_outside_of_this_list(nodes: List[Node]) \
+        -> Tuple[List[int], List[int]]:
+    """Collect all inlinks and outlinks of the given set of Nodes
+    to Nodes outside of this set. The rationale for this is that
+    these given ``nodes`` will be merged into one, so relationships
+    within the set would become loops and disappear.
+
+    (Note that this is not sufficient to update the relationships upon
+    a merge, because the affected Nodess *outside* the given set
+    will need to have their inlinks/outlinks redirected to the new object.)
+
+    :returns: A tuple of lists: ``(inlinks, outlinks)``
+    """
+    all_node_ids = frozenset([node.id for node in nodes])
+    outlinks = []
+    inlinks = []
+    for c in nodes:
+        # No duplicates
+        outlinks.extend([o for o in c.outlinks
+                         if (o not in all_node_ids) and (o not in outlinks)])
+        inlinks.extend([i for i in c.inlinks
+                        if (i not in all_node_ids) and (i not in inlinks)])
+    return inlinks, outlinks
+
+
+def merge_node_lists_from_multiple_documents(node_lists: List[List[Node]]) -> List[Node]:
+    """Combines the Node lists from different documents
+    into one list, so that inlink/outlink references still work.
+    This is useful only if you want to merge two documents
+    into one (e.g., if your annotators worked on different "layers"
+    of data, and you want to merge these annotations).
+
+    This just means shifting the ``id`` (and thus inlinks
+    and outlinks). It is assumed the lists pertain to the same
+    image. Uses deepcopy to avoid exposing the original lists
+    to modification through the merged list.
+
+    Currently cannot handle precedence edges.
+
+    """
+    max_node_ids = [max([node.id for node in c_list]) for c_list in node_lists]
+    min_node_ids = [min([node.id for node in c_list]) for c_list in node_lists]
+    shift_by = [0] + [sum(max_node_ids[:i]) - min_node_ids[i] + 1 for i in
+                      range(1, len(max_node_ids))]
+
+    new_lists = []
+    for nodes, s in zip(node_lists, shift_by):
+        new_list = []
+        for node in nodes:
+            new_node = copy.deepcopy(node)
+            new_id = node.id + s
+            new_node.set_id(new_id)
+
+            # Graph handling
+            new_node.inlinks = [i + s for i in node.inlinks]
+            new_node.outlinks = [o + s for o in node.outlinks]
+
+            new_list.append(new_node)
+        new_lists.append(new_list)
+
+    output = list(itertools.chain(*new_lists))
+
+    return output
+
+
+def link_nodes(from_node: Node, to_node: Node, check_that_nodes_have_the_same_document: bool = True):
+    """Add a relationship from one node to the other. Updates the nodes in-place.
+
+    If the objects are already linked, does nothing.
+    """
+    if from_node.document != to_node.document:
+        if check_that_nodes_have_the_same_document:
+            raise ValueError('Cannot link two Nodes that are')
+        else:
+            logging.warning('Attempting to link Nodes from two different'
+                            ' docments. From: {0}, to: {1}'
+                            ''.format(from_node.document, to_node.document))
+
+    if (to_node.id not in from_node.outlinks) and (from_node.id in to_node.inlinks):
+        logging.warning('Malformed object graph in document {0}:'
+                        ' Relationship {1} --> {2} already exists as inlink,'
+                        ' but not as outlink!.'
+                        ''.format(from_node.document, from_node.id, to_node.id))
+    from_node.outlinks.append(to_node.id)
+    to_node.inlinks.append(from_node.id)
+
+
+def bounding_box_intersection(first_bounding_box: Tuple[int, int, int, int],
+                              second_bounding_box: Tuple[int, int, int, int]) -> Optional[
+    Tuple[int, int, int, int]]:
+    """Returns the t, l, b, r coordinates of the sub-bounding box
+    of bbox_this that is also inside bbox_other.
+    If the bounding boxes do not overlap, returns None."""
+    t, l, b, r = second_bounding_box
+    tt, tl, tb, tr = first_bounding_box
+
+    out_top = max(t, tt)
+    out_bottom = min(b, tb)
+    out_left = max(l, tl)
+    out_right = min(r, tr)
+
+    if (out_top < out_bottom) and (out_left < out_right):
+        return out_top - tt, \
+               out_left - tl, \
+               out_bottom - tt, \
+               out_right - tl
+    else:
+        return None
+
+
+def bounding_box_dice_coefficient(first_bounding_box: Tuple[int, int, int, int],
+                                  second_bounding_box: Tuple[int, int, int, int],
+                                  vertical: bool = False,
+                                  horizontal: bool = False) -> float:
+    """Compute the Dice coefficient (intersection over union)
+    for the given two bounding boxes.
+
+    :param vertical: If set, will only return vertical IoU.
+
+    :param horizontal: If set, will only return horizontal IoU.
+        If both vertical and horizontal are set, will return
+        normal IoU, as if they were both false.
+    """
+    t_t, t_l, t_b, t_r = first_bounding_box
+    o_t, o_l, o_b, o_r = second_bounding_box
+
+    u_t, i_t = min(t_t, o_t), max(t_t, o_t)
+    u_l, i_l = min(t_l, o_l), max(t_l, o_l)
+    u_b, i_b = max(t_b, o_b), min(t_b, o_b)
+    u_r, i_r = max(t_r, o_r), min(t_r, o_r)
+
+    u_vertical = max(0, u_b - u_t)
+    u_horizontal = max(0, u_r - u_l)
+
+    i_vertical = max(0, i_b - i_t)
+    i_horizontal = max(0, i_r - i_l)
+
+    if vertical and not horizontal:
+        if u_vertical == 0:
+            return 0.0
+        else:
+            return i_vertical / u_vertical
+    elif horizontal and not vertical:
+        if u_horizontal == 0:
+            return 0.0
+        else:
+            return i_horizontal / u_horizontal
+    else:
+        if (u_horizontal == 0) or (u_vertical == 0):
+            return 0.0
+        else:
+            return (i_horizontal * i_vertical) / (u_horizontal * u_vertical)
+
+
+def draw_nodes_on_empty_canvas(nodes: List[Node], margin: int = 10) -> Tuple[
+    numpy.ndarray, Tuple[int, int]]:
+    """Draws all the given Nodes onto a zero background.
+    The size of the canvas adapts to the Nodes, with the    given margin.
+
+    Also returns the top left corner coordinates w.r.t. Nodes' bounding boxes.
+    """
+
+    # margin is used to avoid the stafflines touching the edges,
+    # which could perhaps break some assumptions down the line.
+    top, left, bottom, right = compute_unifying_bounding_box(nodes)
+    top_with_margin, left_with_margin, bottom_with_margin, right_with_margin = \
+        max(0, top - margin), max(0, left - margin), bottom + margin, right + margin
+
+    canvas = numpy.zeros(
+        (bottom_with_margin - top_with_margin, right_with_margin - left_with_margin))
+
+    for node in nodes:
+        canvas[node.top - top_with_margin:node.bottom - top_with_margin,
+        node.left - left_with_margin:node.right - left_with_margin] = node.mask * 1
+
+    canvas[canvas != 0] = 1
+
+    return canvas, (top_with_margin, left_with_margin)
```

### Comparing `mung-1.1/mung/node_class.py` & `mung-1.2/mung/node_class.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-"""
-
-**NOTE: This file should become obsolete. The list of classes will be
-implemented as a sub-JSON from SMuFL.**
-
-This module implements the :class:`NodeClass`, which
-represents one possible :class:`Node` class, such as
-a notehead or a time signature. Aside from defining the "vocabulary"
-of available object classes for annotation, it also contains
-some information about how objects of the given class should
-be displayed in the MUSCIMarker annotation software (ordering
-related object classes together in menus, implementing a sensible
-color scheme, etc.). There is nothing interesting about this class,
-we pulled it into the ``mung`` package because the object
-grammar (i.e. which relationships are allowed and which are not)
-depends on having NodeClass object as its "vocabulary",
-and you will probably want to manipulate the data somehow based
-on the objects' relationships (like reassembling notes from notation
-primitives: notehead plus stem plus flags...), and the grammar
-file is a reference for doing that.
-
-NodeClass is a plain old data class, nothing interesting
-about it. The only catch is that colors for rendering
-in MUSCIMarker are kept as a ``#RRGGBB`` string in the XML
-file, but represented in the ``NodeClass.color`` attribute
-as a triplet of floats between 0 (``00``) and 255 (``ff``).
-
-
-The ``___str__()`` method of the class will output the correct
-XML representation.
-
-**XML example**
-
-This is what a single NodeClass element might look like::
-
-    <NodeClass>
-        <Id>1</Id>
-        <Name>notehead-empty</Name>
-        <GroupName>note-primitive/notehead-empty</GroupName>
-        <Color>#FF7566</Color>
-    </NodeClass>
-
-See e.g. ``test/test_data/mff-muscima-classes-annot.xml``,
-which is incidentally the real NodeClass list used
-for annotating MUSCIMA++.
-
-"""
-import logging
-
-
-class NodeClass(object):
-    """Information about the annotation class. We're using it
-    mostly to get the color of rendered Node.
-
-    NodeClass is a Plain Old Data class, there is no other
-    functionality beyond simply existing and writing itself
-    out in the appropriate XML format.
-    """
-
-    def __init__(self, class_id, name, group_name, color):
-        self.class_id = class_id
-        self.name = name
-        self.group_name = group_name
-        # Parse the string into a RGB spec.
-        r, g, b = hex2rgb(color)
-        logging.debug('NodeClass {0}: color {1}'.format(name, (r, g, b)))
-        self.color = (r, g, b)
-
-    def __str__(self):
-        lines = []
-        lines.append('<NodeClass>')
-        lines.append('    <Id>{0}</Id>'.format(self.class_id))
-        lines.append('    <Name>{0}</Name>'.format(self.name))
-        lines.append('    <GroupName>{0}</GroupName>'.format(self.group_name))
-        lines.append('    <Color>{0}</Color>'.format(rgb2hex(self.color)))
-        lines.append('</NodeClass>')
-        return '\n'.join(lines)
-
-
-#######################################################################
-# Utility functions for name/writer conversions
-_hex_tr = {
-    '0': 0,
-    '1': 1, '2': 2, '3': 3, '4': 4, '5': 5, '6': 6, '7': 7,
-    '8': 8, '9': 9,
-    'a': 10, 'b': 11, 'c': 12, 'd': 13, 'e': 14, 'f': 15,
-    'A': 10, 'B': 11, 'C': 12, 'D': 13, 'E': 14, 'F': 15,
-}
-_hex_itr = {v: k for k, v in list(_hex_tr.items())}
-
-
-def parse_hex(hstr):
-    """Convert a hexadecimal number string to integer.
-
-    >>> parse_hex('33')
-    51
-    >>> parse_hex('abe8')
-    44008
-
-    """
-    out = 0
-    for i, l in enumerate(reversed(hstr)):
-        out += (16 ** i) * _hex_tr[l]
-    return out
-
-
-def hex2rgb(hstr):
-    """Parse a hex-coded color like '#AA0202' into a floating-point representation.
-
-    >>> hex2rgb('#abe822')
-    (0.6705882352941176, 0.9098039215686274, 0.13333333333333333)
-
-    """
-    if hstr.startswith('#'):
-        hstr = hstr[1:]
-    rs, gs, bs = hstr[:2], hstr[2:4], hstr[4:]
-    r, g, b = parse_hex(rs), parse_hex(gs), parse_hex(bs)
-    return r / 255.0, g / 255.0, b / 255.0
-
-
-def rgb2hex(rgb):
-    """Convert a floating-point representation of R, G, B values
-    between 0 and 1 (inclusive) to a hex string (strating with a
-    hashmark). Will use uppercase letters for 10 - 15.
-
-    >>> rgb = (0.6705882352941176, 0.9098039215686274, 0.13333333333333333)
-    >>> rgb2hex(rgb)
-    '#ABE822'
-
-    """
-    rgb_int = [int(ch * 255) for ch in rgb]
-    return '#' + ''.join(['{:02X}'.format(ch) for ch in rgb_int])
+"""
+
+**NOTE: This file should become obsolete. The list of classes will be
+implemented as a sub-JSON from SMuFL.**
+
+This module implements the :class:`NodeClass`, which
+represents one possible :class:`Node` class, such as
+a notehead or a time signature. Aside from defining the "vocabulary"
+of available object classes for annotation, it also contains
+some information about how objects of the given class should
+be displayed in the MUSCIMarker annotation software (ordering
+related object classes together in menus, implementing a sensible
+color scheme, etc.). There is nothing interesting about this class,
+we pulled it into the ``mung`` package because the object
+grammar (i.e. which relationships are allowed and which are not)
+depends on having NodeClass object as its "vocabulary",
+and you will probably want to manipulate the data somehow based
+on the objects' relationships (like reassembling notes from notation
+primitives: notehead plus stem plus flags...), and the grammar
+file is a reference for doing that.
+
+NodeClass is a plain old data class, nothing interesting
+about it. The only catch is that colors for rendering
+in MUSCIMarker are kept as a ``#RRGGBB`` string in the XML
+file, but represented in the ``NodeClass.color`` attribute
+as a triplet of floats between 0 (``00``) and 255 (``ff``).
+
+
+The ``___str__()`` method of the class will output the correct
+XML representation.
+
+**XML example**
+
+This is what a single NodeClass element might look like::
+
+    <NodeClass>
+        <Id>1</Id>
+        <Name>notehead-empty</Name>
+        <GroupName>note-primitive/notehead-empty</GroupName>
+        <Color>#FF7566</Color>
+    </NodeClass>
+
+See e.g. ``test/test_data/mff-muscima-classes-annot.xml``,
+which is incidentally the real NodeClass list used
+for annotating MUSCIMA++.
+
+"""
+import logging
+
+
+class NodeClass(object):
+    """Information about the annotation class. We're using it
+    mostly to get the color of rendered Node.
+
+    NodeClass is a Plain Old Data class, there is no other
+    functionality beyond simply existing and writing itself
+    out in the appropriate XML format.
+    """
+
+    def __init__(self, class_id, name, group_name, color):
+        self.class_id = class_id
+        self.name = name
+        self.group_name = group_name
+        # Parse the string into a RGB spec.
+        r, g, b = hex2rgb(color)
+        logging.debug('NodeClass {0}: color {1}'.format(name, (r, g, b)))
+        self.color = (r, g, b)
+
+    def __str__(self):
+        lines = []
+        lines.append('<NodeClass>')
+        lines.append('    <Id>{0}</Id>'.format(self.class_id))
+        lines.append('    <Name>{0}</Name>'.format(self.name))
+        lines.append('    <GroupName>{0}</GroupName>'.format(self.group_name))
+        lines.append('    <Color>{0}</Color>'.format(rgb2hex(self.color)))
+        lines.append('</NodeClass>')
+        return '\n'.join(lines)
+
+
+#######################################################################
+# Utility functions for name/writer conversions
+_hex_tr = {
+    '0': 0,
+    '1': 1, '2': 2, '3': 3, '4': 4, '5': 5, '6': 6, '7': 7,
+    '8': 8, '9': 9,
+    'a': 10, 'b': 11, 'c': 12, 'd': 13, 'e': 14, 'f': 15,
+    'A': 10, 'B': 11, 'C': 12, 'D': 13, 'E': 14, 'F': 15,
+}
+_hex_itr = {v: k for k, v in list(_hex_tr.items())}
+
+
+def parse_hex(hstr):
+    """Convert a hexadecimal number string to integer.
+
+    >>> parse_hex('33')
+    51
+    >>> parse_hex('abe8')
+    44008
+
+    """
+    out = 0
+    for i, l in enumerate(reversed(hstr)):
+        out += (16 ** i) * _hex_tr[l]
+    return out
+
+
+def hex2rgb(hstr):
+    """Parse a hex-coded color like '#AA0202' into a floating-point representation.
+
+    >>> hex2rgb('#abe822')
+    (0.6705882352941176, 0.9098039215686274, 0.13333333333333333)
+
+    """
+    if hstr.startswith('#'):
+        hstr = hstr[1:]
+    rs, gs, bs = hstr[:2], hstr[2:4], hstr[4:]
+    r, g, b = parse_hex(rs), parse_hex(gs), parse_hex(bs)
+    return r / 255.0, g / 255.0, b / 255.0
+
+
+def rgb2hex(rgb):
+    """Convert a floating-point representation of R, G, B values
+    between 0 and 1 (inclusive) to a hex string (strating with a
+    hashmark). Will use uppercase letters for 10 - 15.
+
+    >>> rgb = (0.6705882352941176, 0.9098039215686274, 0.13333333333333333)
+    >>> rgb2hex(rgb)
+    '#ABE822'
+
+    """
+    rgb_int = [int(ch * 255) for ch in rgb]
+    return '#' + ''.join(['{:02X}'.format(ch) for ch in rgb_int])
```

### Comparing `mung-1.1/mung/stafflines.py` & `mung-1.2/mung/stafflines.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,812 +1,814 @@
-"""This module implements functions for manipulating staffline symbols.
-Mostly it is support for going from detected staffline fragments
-to full staff objects and relationships; this machinery is called
-e.g. by pressing "shift+s" in MUSCIMarker."""
-import collections
-import logging
-import pprint
-
-import numpy
-from skimage.filters import gaussian
-from skimage.morphology import watershed
-from typing import List, Tuple
-
-from mung.graph import NotationGraph, find_noteheads_on_staff_linked_to_leger_line
-from mung.constants import InferenceEngineConstants as _CONST
-from mung.node import Node, draw_nodes_on_empty_canvas, link_nodes
-from mung.utils import compute_connected_components
-
-
-def __has_parent_staff(node: Node, nodes: List[Node]) -> bool:
-    id_to_node_mapping = {c.id: c for c in nodes}
-    staff_inlinks = [id_to_node_mapping[i] for i in node.inlinks
-                     if id_to_node_mapping[i].class_name == _CONST.STAFF_CLASS_NAME]
-    return len(staff_inlinks) > 0
-
-
-def __has_child_staffspace(staff: Node, nodes: List[Node]) -> bool:
-    id_to_node_mapping = {c.id: c for c in nodes}
-    staffline_outlinks = [id_to_node_mapping[i] for i in staff.outlinks
-                          if id_to_node_mapping[i].class_name == _CONST.STAFFSPACE_CLASS_NAME]
-    return len(staffline_outlinks) > 0
-
-
-def __has_neighbor_staffspace(staffline: Node, nodes: List[Node]) -> bool:
-    id_to_node_mapping = {c.id: c for c in nodes}
-    # Find parent staff
-    if not __has_parent_staff(staffline, nodes):
-        return False
-    parent_staffs = [id_to_node_mapping[i] for i in staffline.inlinks
-                     if id_to_node_mapping[i].class_name == _CONST.STAFF_CLASS_NAME]
-    if len(parent_staffs) > 1:
-        raise ValueError('More than one parent staff for staffline {0}!'
-                         ''.format(staffline.id))
-    staff = parent_staffs[0]
-    return __has_child_staffspace(staff, nodes)
-
-
-def merge_staffline_segments(nodes: List[Node], margin: int = 10) -> List[Node]:
-    """Given a list of Nodes that contain some staffline
-    objects, generates a new list where the stafflines
-    are merged based on their horizontal projections.
-    Basic step for going from the staffline detection masks to
-    the actual staffline objects.
-
-    Assumes that stafflines are straight: their bounding boxes
-    do not touch or overlap.
-
-    :return: A modified Node list: the original staffline-class
-        symbols are replaced by the merged ones. If the original stafflines
-        had any inlinks, they are preserved (mapped to the new staffline).
-    """
-    already_processed_stafflines = [node for node in nodes
-                                    if (node.class_name == _CONST.STAFFLINE_CLASS_NAME) and
-                                    __has_parent_staff(node, nodes)]
-    # margin is used to avoid the stafflines touching the edges,
-    # which could perhaps break some assumptions down the line.
-    old_staffline_nodes = [c for c in nodes
-                           if (c.class_name == _CONST.STAFFLINE_CLASS_NAME) and
-                           not __has_parent_staff(c, nodes)]
-    if len(old_staffline_nodes) == 0:
-        logging.info('merge_staffline_segments: nothing new to do!')
-        return nodes
-
-    canvas, (_t, _l) = draw_nodes_on_empty_canvas(old_staffline_nodes)
-
-    _staffline_bboxes, staffline_masks = staffline_bboxes_and_masks_from_horizontal_merge(canvas)
-    # Bounding boxes need to be adjusted back with respect to the original image!
-    staffline_bboxes = [(t + _t, l + _l, b + _t, r + _l) for t, l, b, r in _staffline_bboxes]
-
-    # Create the Nodes.
-    next_node_id = max([c.id for c in nodes]) + 1
-    dataset = nodes[0].dataset
-    document = nodes[0].document
-
-    #  - Create the staffline Nodes
-    staffline_nodes = []
-    for sl_bb, sl_m in zip(staffline_bboxes, staffline_masks):
-        t, l, b, r = sl_bb
-        c = Node(id_=next_node_id,
-                 class_name=_CONST.STAFFLINE_CLASS_NAME,
-                 top=t, left=l, height=b - t, width=r - l,
-                 mask=sl_m,
-                 dataset=dataset, document=document)
-        staffline_nodes.append(c)
-        next_node_id += 1
-
-    non_staffline_nodes = [c for c in nodes
-                           if c.class_name != _CONST.STAFFLINE_CLASS_NAME]
-    old_staffline_ids = set([c.id for c in old_staffline_nodes])
-    old2new_staffline_id_map = {}
-    for os in old_staffline_nodes:
-        for ns in staffline_nodes:
-            if os.overlaps(ns):
-                old2new_staffline_id_map[os.id] = ns
-
-    logging.info('Re-linking from the old staffline objects to new ones.')
-    for c in non_staffline_nodes:
-        new_outlinks = []
-        for o in c.outlinks:
-            if o in old_staffline_ids:
-                new_staffline = old2new_staffline_id_map[o]
-                new_outlinks.append(new_staffline.id)
-                new_staffline.inlinks.append(c.id)
-            else:
-                new_outlinks.append(o)
-
-    output = non_staffline_nodes + staffline_nodes + already_processed_stafflines
-    return output
-
-
-def staffline_bboxes_and_masks_from_horizontal_merge(mask: numpy.ndarray) -> \
-        Tuple[List[Tuple[int, int, int, int]], List[numpy.ndarray]]:
-    """Returns a list of staff_line bboxes and masks
-     computed from the input mask, with
-    each set of connected components in the mask that has at least
-    one pixel in a neighboring or overlapping row is assigned to
-    the same label. Intended for finding staffline masks from individual
-    components of the stafflines (for this purpose, you have to assume
-    that the stafflines are straight)."""
-    logging.info('Getting staffline connected components.')
-
-    cc, labels, bboxes = compute_connected_components(mask)
-
-    logging.info('Getting staffline component vertical projections')
-    #  - Use vertical dimension of CCs to determine which ones belong together
-    #    to form stafflines. (Criterion: row overlap.)
-    n_rows, n_cols = mask.shape
-    # For each row of the image: which CCs have pxs on that row?
-    intervals = [[] for _ in range(n_rows)]
-    for label, (t, l, b, r) in list(bboxes.items()):
-        if label == 0:
-            continue
-        # Ignore very short staffline segments that can easily be artifacts
-        # and should not affect the vertical range of the staffline anyway.
-        # The "8" is a magic number, no good reason for specifically 8.
-        # (It should be some proportion of the image width, like 0.01.)
-        if (r - l) < 8:
-            continue
-        for row in range(t, b):
-            intervals[row].append(label)
-
-    logging.warning('Grouping staffline connected components into stafflines.')
-    # For each staffline, we collect the CCs that it is made of. We assume stafflines
-    # are separated from each other by at least one empty row.
-    staffline_components = []
-    _in_staffline = False
-    _current_staffline_components = []
-    for r_labels in intervals:
-        if not _in_staffline:
-            # Last row did not contain staffline components.
-            if len(r_labels) == 0:
-                # No staffline component on current row
-                continue
-            else:
-                _in_staffline = True
-                _current_staffline_components += r_labels
-        else:
-            # Last row contained staffline components.
-            if len(r_labels) == 0:
-                # Current staffline has no more rows.
-                staffline_components.append(set(_current_staffline_components))
-                _current_staffline_components = []
-                _in_staffline = False
-                continue
-            else:
-                # Current row contains staffline components: the current
-                # staffline continues.
-                _current_staffline_components += r_labels
-
-    logging.info('No. of stafflines, with component groups: {0}'
-                 ''.format(len(staffline_components)))
-
-    # Now: merge the staffline components into one bbox/mask.
-    logging.info('Merging staffline components into staffline bboxes and masks.')
-    staffline_bboxes = []
-    staffline_masks = []
-    for sc in sorted(staffline_components,
-                     key=lambda c: min([bboxes[cc][0]
-                                        for cc in c])):  # Sorted top-down
-        st, sl, sb, sr = n_rows, n_cols, 0, 0
-        for component in sc:
-            t, l, b, r = bboxes[component]
-            st, sl, sb, sr = min(t, st), min(l, sl), max(b, sb), max(r, sr)
-        # Here, again, we assume that no two "real" stafflines have overlapping
-        # bounding boxes.
-        _sm = mask[st:sb, sl:sr]
-        staffline_bboxes.append((st, sl, sb, sr))
-        staffline_masks.append(_sm)
-
-    # Check if n. of stafflines is divisible by 5
-    n_stafflines = len(staffline_bboxes)
-    logging.warning('\tTotal stafflines: {0}'.format(n_stafflines))
-    if n_stafflines % 5 != 0:
-        raise ValueError('Number of stafflines is not divisible by 5!')
-
-    return staffline_bboxes, staffline_masks
-
-
-def staff_bboxes_and_masks_from_staffline_bboxes_and_image(staffline_bboxes, mask) -> \
-        Tuple[List[Tuple[int, int, int, int]], List[numpy.ndarray]]:
-    logging.warning('Creating staff bboxes and masks.')
-
-    #  - Go top-down and group the stafflines by five to get staves.
-    #    (The staffline bboxes are already sorted top-down.)
-    staff_bboxes = []
-    staff_masks = []
-
-    n_stafflines = len(staffline_bboxes)
-    for i in range(n_stafflines // 5):
-        _sbb = staffline_bboxes[5 * i:5 * (i + 1)]
-        _st = min([bb[0] for bb in _sbb])
-        _sl = min([bb[1] for bb in _sbb])
-        _sb = max([bb[2] for bb in _sbb])
-        _sr = max([bb[3] for bb in _sbb])
-        staff_bboxes.append((_st, _sl, _sb, _sr))
-        staff_masks.append(mask[_st:_sb, _sl:_sr])
-
-    logging.warning('Total staffs: {0}'.format(len(staff_bboxes)))
-
-    return staff_bboxes, staff_masks
-
-
-def staffline_surroundings_mask(staffline_node: Node) -> Tuple[numpy.ndarray, numpy.ndarray]:
-    """Find the parts of the staffline's bounding box which lie
-    above or below the actual staffline.
-
-    These areas will be very small for straight stafflines,
-    but might be considerable when staffline curvature grows.
-    """
-    # We segment both masks into "above staffline" and "below staffline"
-    # areas.
-    elevation = staffline_node.mask * 255
-    # Blur, to plug small holes somewhat:
-    elevation = gaussian(elevation, sigma=1.0)
-    # Prepare the segmentation markers: 1 is ABOVE, 2 is BELOW
-    markers = numpy.zeros(staffline_node.mask.shape)
-    markers[0, :] = 1
-    markers[-1, :] = 2
-    markers[staffline_node.mask != 0] = 0
-    seg = watershed(elevation, markers)
-
-    bmask = numpy.ones(seg.shape)
-    bmask[seg != 2] = 0
-    tmask = numpy.ones(seg.shape)
-    tmask[seg != 1] = 0
-
-    return bmask, tmask
-
-
-def build_staff_nodes(nodes: List[Node]) -> List[Node]:
-    """Derives staff objects from staffline objects.
-
-    Assumes each staff has 5 stafflines.
-
-    Assumes the stafflines have already been merged."""
-    stafflines = [c for c in nodes
-                  if c.class_name == _CONST.STAFFLINE_CLASS_NAME and
-                  not __has_parent_staff(c, nodes)]
-    if len(stafflines) == 0:
-        return []
-
-    staffline_bboxes = [c.bounding_box for c in stafflines]
-    canvas, (_t, _l) = draw_nodes_on_empty_canvas(stafflines)
-
-    logging.warning('Creating staff bboxes and masks.')
-
-    #  - Go top-down and group the stafflines by five to get staves.
-    #    (The staffline bboxes are already sorted top-down.)
-    staff_bboxes = []
-    staff_masks = []
-
-    n_stafflines = len(stafflines)
-    for i in range(n_stafflines // 5):
-        _sbb = staffline_bboxes[5 * i:5 * (i + 1)]
-        _st = min([bb[0] for bb in _sbb])
-        _sl = min([bb[1] for bb in _sbb])
-        _sb = max([bb[2] for bb in _sbb])
-        _sr = max([bb[3] for bb in _sbb])
-        staff_bboxes.append((_st, _sl, _sb, _sr))
-        staff_masks.append(canvas[_st - _t:_sb - _t, _sl - _l:_sr - _l])
-
-    logging.info('Creating staff Nodes')
-    next_node_id = max([c.id for c in nodes]) + 1
-    dataset = nodes[0].dataset
-    document = nodes[0].document
-
-    staffs = []
-    for s_bb, s_m in zip(staff_bboxes, staff_masks):
-        t, l, b, r = s_bb
-        staff = Node(id_=next_node_id,
-                     class_name=_CONST.STAFF_CLASS_NAME,
-                     top=t, left=l, height=b - t, width=r - l,
-                     mask=s_m,
-                     dataset=dataset, document=document)
-        staffs.append(staff)
-        next_node_id += 1
-
-    for i, sc in enumerate(staffs):
-        sl_from = 5 * i
-        sl_to = 5 * (i + 1)
-        for sl in stafflines[sl_from:sl_to]:
-            sl.inlinks.append(sc.id)
-            sc.outlinks.append(sl.id)
-
-    return staffs
-
-
-def build_staffspace_nodes(nodes: List[Node]) -> List[Node]:
-    """Creates the staffspace objects based on stafflines
-    and staffs. There is a staffspace between each two stafflines,
-    one on the top side of each staff, and one on the bottom
-    side for each staff (corresponding e.g. to positions of g5 and d4
-    with the standard G-clef).
-
-    Note that staffspaces do not assume anything about the number
-    of stafflines per staff. However, single-staffline staffs will
-    not have the outer staffspaces generated (there is nothing to derive
-    their size from), for now.
-
-    :param nodes: A list of Nodes that must contain
-        all the relevant stafflines and staffs.
-
-    :return: A list of staffspace Nodes.
-    """
-    next_node_id = max([c.id for c in nodes]) + 1
-    dataset = nodes[0].dataset
-    document = nodes[0].document
-
-    staff_nodes = [node for node in nodes
-                   if node.class_name == _CONST.STAFF_CLASS_NAME
-                   and not __has_child_staffspace(node, nodes)]
-    staffline_nodes = [node for node in nodes
-                       if node.class_name == _CONST.STAFFLINE_CLASS_NAME
-                       and not __has_neighbor_staffspace(node, nodes)]
-
-    staff_spaces = []
-
-    for i, staff in enumerate(staff_nodes):
-        current_stafflines = [sc for sc in staffline_nodes
-                              if sc.id in staff.outlinks]
-        sorted_stafflines = sorted(current_stafflines, key=lambda x: x.top)
-
-        current_staffspace_nodes = []
-
-        # Percussion single-line staves do not have staffspaces.
-        if len(sorted_stafflines) == 1:
-            continue
-
-        #################
-        # Internal staffspace
-        for s1, s2 in zip(sorted_stafflines[:-1], sorted_stafflines[1:]):
-            # s1 is the UPPER staffline, s2 is the LOWER staffline
-            # Left and right limits: to simplify things, we take the column
-            # *intersection* of (s1, s2). This gives the invariant that
-            # the staffspace is limited from top and bottom in each of its columns.
-            l = max(s1.left, s2.left)
-            r = min(s1.right, s2.right)
-
-            # Shift s1, s2 to the right by this much to have the cols. align
-            # All of these are non-negative.
-            dl1, dl2 = l - s1.left, l - s2.left
-            dr1, dr2 = s1.right - r, s2.right - r
-
-            # The stafflines are not necessarily straight,
-            # so top is given for the *topmost bottom edge* of the top staffline + 1
-
-            # First create mask
-            canvas = numpy.zeros((s2.bottom - s1.top, r - l), dtype='uint8')
-
-            # Paste masks into canvas.
-            # This assumes that the top of the bottom staffline is below
-            # the top of the top staffline... and that the bottom
-            # of the top staffline is above the bottom of the bottom
-            # staffline. This may not hold in very weird situations,
-            # but it's good for now.
-            logging.debug(s1.bounding_box, s1.mask.shape)
-            logging.debug(s2.bounding_box, s2.mask.shape)
-            logging.debug(canvas.shape)
-            logging.debug('l={0}, dl1={1}, dl2={2}, r={3}, dr1={4}, dr2={5}'
-                          ''.format(l, dl1, dl2, r, dr1, dr2))
-            # canvas[:s1.height, :] += s1.mask[:, dl1:s1.width-dr1]
-            # canvas[-s2.height:, :] += s2.mask[:, dl2:s2.width-dr2]
-
-            # We have to deal with staffline interruptions.
-            # One way to do this
-            # is watershed fill: put markers along the bottom and top
-            # edge, use mask * 10000 as elevation
-
-            s1_above, s1_below = staffline_surroundings_mask(s1)
-            s2_above, s2_below = staffline_surroundings_mask(s2)
-
-            # Get bounding boxes of the individual stafflines' masks
-            # that intersect with the staffspace bounding box, in terms
-            # of the staffline bounding box.
-            s1_t, s1_l, s1_b, s1_r = 0, dl1, \
-                                     s1.height, s1.width - dr1
-            s1_h, s1_w = s1_b - s1_t, s1_r - s1_l
-            s2_t, s2_l, s2_b, s2_r = canvas.shape[0] - s2.height, dl2, \
-                                     canvas.shape[0], s2.width - dr2
-            s2_h, s2_w = s2_b - s2_t, s2_r - s2_l
-
-            logging.debug(s1_t, s1_l, s1_b, s1_r, (s1_h, s1_w))
-
-            # We now take the intersection of s1_below and s2_above.
-            # If there is empty space in the middle, we fill it in.
-            staffspace_mask = numpy.ones(canvas.shape)
-            staffspace_mask[s1_t:s1_b, :] -= (1 - s1_below[:, dl1:s1.width - dr1])
-            staffspace_mask[s2_t:s2_b, :] -= (1 - s2_above[:, dl2:s2.width - dr2])
-
-            ss_top = s1.top
-            ss_bottom = s2.bottom
-            ss_left = l
-            ss_right = r
-
-            staff_space = Node(next_node_id, _CONST.STAFFSPACE_CLASS_NAME,
-                               top=ss_top, left=ss_left,
-                               height=ss_bottom - ss_top,
-                               width=ss_right - ss_left,
-                               mask=staffspace_mask,
-                               dataset=dataset, document=document)
-
-            staff_space.inlinks.append(staff.id)
-            staff.outlinks.append(staff_space.id)
-
-            current_staffspace_nodes.append(staff_space)
-
-            next_node_id += 1
-
-        ##########
-        # Add top and bottom staffspace.
-        # These outer staffspaces will have the width
-        # of their bottom neighbor, and height derived
-        # from its mask columns.
-        # This is quite approximate, but it should do.
-
-        # Upper staffspace
-        tsl = sorted_stafflines[0]
-        tsl_heights = tsl.mask.sum(axis=0)
-        tss = current_staffspace_nodes[0]
-        tss_heights = tss.mask.sum(axis=0)
-
-        uss_top = max(0, tss.top - max(tss_heights))
-        uss_left = tss.left
-        uss_width = tss.width
-        # We use 1.5, so that large noteheads
-        # do not "hang out" of the staffspace.
-        uss_height = int(tss.height / 1.2)
-        # Shift because of height downscaling:
-        uss_top += tss.height - uss_height
-        uss_mask = tss.mask[:uss_height, :] * 1
-
-        staff_space = Node(next_node_id, _CONST.STAFFSPACE_CLASS_NAME,
-                           top=uss_top, left=uss_left,
-                           height=uss_height,
-                           width=uss_width,
-                           mask=uss_mask,
-                           dataset=dataset, document=document)
-        current_staffspace_nodes.append(staff_space)
-        staff.outlinks.append(staff_space.id)
-        staff_space.inlinks.append(staff.id)
-        next_node_id += 1
-
-        # Lower staffspace
-        bss = current_staffspace_nodes[-2]
-        bss_heights = bss.mask.sum(axis=0)
-        bsl = sorted_stafflines[-1]
-        bsl_heights = bsl.mask.sum(axis=0)
-
-        lss_top = bss.bottom  # + max(bsl_heights)
-        lss_left = bss.left
-        lss_width = bss.width
-        lss_height = int(bss.height / 1.2)
-        lss_mask = bss.mask[:lss_height, :] * 1
-
-        staff_space = Node(next_node_id, _CONST.STAFFSPACE_CLASS_NAME,
-                           top=lss_top, left=lss_left,
-                           height=lss_height,
-                           width=lss_width,
-                           mask=lss_mask,
-                           dataset=dataset, document=document)
-        current_staffspace_nodes.append(staff_space)
-        staff.outlinks.append(staff_space.id)
-        staff_space.inlinks.append(staff.id)
-        next_node_id += 1
-
-        staff_spaces += current_staffspace_nodes
-
-    return staff_spaces
-
-
-def add_staff_relationships(nodes: List[Node],
-                            notehead_staffspace_threshold: float = 0.2,
-                            reprocess_noteheads_inside_staff_with_lls: bool = True):
-    """Adds the relationships from various symbols to staff objects:
-    stafflines, staffspaces, and staffs.
-
-    :param nodes: The list of Nodes in the document. Must
-        include the staff objects.
-
-    :param notehead_staffspace_threshold: A notehead is considered to be
-        on a staffline if it intersects a staffline, and the ratio between
-        how far above the staffline and how far below the staffline it reaches
-        is at least this (default: 0.2). The ratio is computed both ways:
-        d_top / d_bottom and d_bottom / d_top, and the minimum is taken,
-        so the default in effect restricts d_top / d_bottom between 0.2 and 0.8:
-        in other words, the imbalance of the notehead's bounding box around
-        the staffline should be less than 1:4.
-
-    :param reprocess_noteheads_inside_staff_with_lls: If set to True, will check against noteheads
-        that are connected to leger lines, but intersect a staffline. If found,
-        will remove their edges before further processing, so that the noteheads
-        will seem properly unprocessed.
-
-        Note that this handling is a bit ad-hoc for now. However, we currently
-        do not have a better place to fit this in, since the Best Practices
-        currently call for first applying the syntactic parser and then
-        adding staff relationships.
-
-    :return: The list of Nodes corresponding to the new graph.
-    """
-    graph = NotationGraph(nodes)
-    id_to_node_mapping = {node.id: node for node in nodes}
-
-    ON_STAFFLINE_RATIO_TRHESHOLD = notehead_staffspace_threshold
-
-    ##########################################################################
-    if reprocess_noteheads_inside_staff_with_lls:
-        ll_noteheads_on_staff = find_noteheads_on_staff_linked_to_leger_line(nodes)
-        logging.info('Reprocessing noteheads that are inside a staff, but have links'
-                     ' to leger lines. Found {0} such noteheads.'
-                     ''.format(len(ll_noteheads_on_staff)))
-        for n in ll_noteheads_on_staff:
-            # Remove all links to leger lines.
-            leger_lines = graph.children(n, class_filter=[_CONST.LEGER_LINE_CLASS_NAME])
-            for ll in leger_lines:
-                graph.remove_edge(n.id, ll.id)
-
-    ##########################################################################
-    logging.info('Find the staff-related symbols')
-    staffs = [c for c in nodes if c.class_name == _CONST.STAFF_CLASS_NAME]
-
-    staff_related_symbols = collections.defaultdict(list)
-    notehead_symbols = collections.defaultdict(list)
-    rest_symbols = collections.defaultdict(list)
-    for node in nodes:
-        if node.class_name in _CONST.STAFF_RELATED_CLASS_NAMES:
-            # Check if it already has a staff link
-            if not graph.has_children(node, [_CONST.STAFF_CLASS_NAME]):
-                staff_related_symbols[node.class_name].append(node)
-        if node.class_name in _CONST.NOTEHEAD_CLASS_NAMES:
-            if not graph.has_children(node, [_CONST.STAFF_CLASS_NAME]):
-                notehead_symbols[node.class_name].append(node)
-        if node.class_name in _CONST.REST_CLASS_NAMES:
-            if not graph.has_children(node, [_CONST.STAFF_CLASS_NAME]):
-                rest_symbols[node.class_name].append(node)
-
-    ##########################################################################
-    logging.info('Adding staff relationships')
-    #  - Which direction do the relationships lead in?
-    #    Need to define this.
-    #
-    # Staff -> symbol?
-    # Symbol -> staff?
-    # It does not really matter, but it's more intuitive to attach symbols
-    # onto a pre-existing staff. So, symbol -> staff.
-    for class_name, cs in list(staff_related_symbols.items()):
-        for node in cs:
-            # Find the related staff. Relatedness is measured by row overlap.
-            # That means we have to modify the staff bounding box to lead
-            # from the leftmost to the rightmost column. This holds
-            # especially for the staff_grouping symbols.
-            for s in staffs:
-                st, sl, sb, sr = s.bounding_box
-                sl = 0
-                sr = max(sr, node.right)
-                if node.overlaps((st, sl, sb, sr)):
-                    link_nodes(node, s, check_that_nodes_have_the_same_document=False)
-
-    ##########################################################################
-    logging.info('Adding rest --> staff relationships.')
-    for class_name, cs in list(rest_symbols.items()):
-        for node in cs:
-            closest_staff = min([s for s in staffs],
-                                key=lambda x: ((x.bottom + x.top) / 2. - (
-                                        node.bottom + node.top) / 2.) ** 2)
-            link_nodes(node, closest_staff, check_that_nodes_have_the_same_document=False)
-
-    ##########################################################################
-    logging.info('Adding notehead relationships.')
-
-    # NOTE:
-    # This part should NOT rely on staffspace masks in any way!
-    # They are highly unreliable.
-
-    # Sort the staff objects top-down. Assumes stafflines do not cross,
-    # and that there are no crazy curves at the end that would make the lower
-    # stafflines stick out over the ones above them...
-    stafflines = [c for c in nodes if c.class_name == _CONST.STAFFLINE_CLASS_NAME]
-    stafflines = sorted(stafflines, key=lambda c: c.top)
-    staffspaces = [c for c in nodes if c.class_name == _CONST.STAFFSPACE_CLASS_NAME]
-    staffspaces = sorted(staffspaces, key=lambda c: c.top)
-    staves = [c for c in nodes if c.class_name == _CONST.STAFF_CLASS_NAME]
-    staves = sorted(staves, key=lambda c: c.top)
-
-    logging.info('Stafflines: {0}'.format(len(stafflines)))
-    logging.info('Staffspaces: {0}'.format(len(staffspaces)))
-    logging.info('Staves: {0}'.format(len(staves)))
-
-    # Indexing data structures.
-    #
-    # We need to know:
-    #  - per staffline and staffspace: its containing staff
-    _staff_per_ss_sl = {}
-    #  - per staffline and staffspace: its index (top to bottom) within the staff
-    _ss_sl_idx_wrt_staff = {}
-    # Reverse indexes:
-    # If I know which staff (by id) and which index of staffline/staffspace,
-    # I want to retrieve the given staffline/staffspace Node:
-    _staff_and_idx2ss = collections.defaultdict(dict)
-    _staff_and_idx2sl = collections.defaultdict(dict)
-
-    # Build the indexes
-    for _staff in staves:
-        # Keep the top-down ordering from above:
-        _s_stafflines = [_staffline for _staffline in stafflines
-                         if _staff.id in _staffline.inlinks]
-        _s_staffspaces = [_staffspace for _staffspace in staffspaces
-                          if _staff.id in _staffspace.inlinks]
-        for i, _sl in enumerate(_s_stafflines):
-            _staff_per_ss_sl[_sl.id] = _staff
-            _ss_sl_idx_wrt_staff[_sl.id] = i
-            _staff_and_idx2sl[_staff.id][i] = _sl
-            logging.debug('Staff {0}: stafflines {1}'.format(_staff.id,
-                                                             _staff_and_idx2sl[_staff.id]))
-        for i, _ss in enumerate(_s_staffspaces):
-            _staff_per_ss_sl[_ss.id] = _staff
-            _ss_sl_idx_wrt_staff[_ss.id] = i
-            _staff_and_idx2ss[_staff.id][i] = _ss
-
-    logging.debug(pprint.pformat(dict(_staff_and_idx2ss)))
-
-    for class_name, cs in list(notehead_symbols.items()):
-        for node in cs:
-
-            ct, cl, cb, cr = node.bounding_box
-
-            ################
-            # Add relationship to given staffline or staffspace.
-
-            # If notehead has leger lines, skip it for now.
-            has_leger_line = False
-            for outlink in node.outlinks:
-                if id_to_node_mapping[outlink].class_name == _CONST.LEGER_LINE_CLASS_NAME:
-                    has_leger_line = True
-                    break
-
-            if has_leger_line:
-                # Attach to the appropriate staff:
-                # meaning, staff closest to the innermost leger line.
-                leger_lines = [id_to_node_mapping[o] for o in node.outlinks
-                               if id_to_node_mapping[o].class_name == _CONST.LEGER_LINE_CLASS_NAME]
-                # Furthest from notehead's top is innermost.
-                # (If notehead is below staff and crosses a ll., one
-                #  of these numbers will be negative. But that doesn't matter.)
-                ll_max_dist = max(leger_lines, key=lambda leger_line: leger_line.top - node.top)
-                # Find closest staff to max-dist leger ine
-                staff_min_dist = min(staves,
-                                     key=lambda ss: min((ll_max_dist.bottom - ss.top) ** 2,
-                                                        (ll_max_dist.top - ss.bottom) ** 2))
-                distance_of_closest_staff = (ll_max_dist.top + ll_max_dist.bottom) / 2 \
-                                            - (staff_min_dist.top + staff_min_dist.bottom) / 2
-                if numpy.abs(distance_of_closest_staff) > (50 + 0.5 * staff_min_dist.height):
-                    logging.debug('Trying to join notehead with leger line to staff,'
-                                  ' but the distance is larger than 50. Notehead: {0},'
-                                  ' leger line: {1}, staff: {2}, distance: {3}'
-                                  ''.format(node.uid, ll_max_dist.uid, staff_min_dist.id,
-                                            distance_of_closest_staff))
-                else:
-                    link_nodes(node, staff_min_dist, check_that_nodes_have_the_same_document=False)
-                continue
-
-            # - Find the related staffline.
-            # - Because of curved stafflines, this has to be done w.r.t.
-            #   the horizontal position of the notehead.
-            # - Also, because stafflines are NOT filled in (they do not have
-            #   intersections annotated), it is necessary to use a wider
-            #   window than just the notehead.
-            # - We will assume that STAFFLINES DO NOT CROSS.
-            #   (That is a reasonable assumption.)
-            #
-            # - For now, we only work with more or less straight stafflines.
-
-            overlapped_stafflines = []
-            overlapped_staffline_idxs = []
-            for i, s in enumerate(stafflines):
-                # This is the assumption of straight stafflines!
-                if (ct <= s.top <= cb) or (ct <= s.bottom <= cb):
-                    overlapped_stafflines.append(s)
-                    overlapped_staffline_idxs.append(i)
-
-            if node.id < 10:
-                logging.info('Notehead {0} ({1}): overlaps {2} stafflines'.format(node.uid, node.bounding_box,
-                                                                                  len(overlapped_stafflines)))
-
-            if len(overlapped_stafflines) == 1:
-                s = overlapped_stafflines[0]
-                dtop = s.top - ct
-                dbottom = cb - s.bottom
-
-                logging.info('Notehead {0}, staffline {1}: ratio {2:.2f}'
-                             ''.format(node.id, s.id, min(dtop, dbottom) / max(dtop, dbottom)))
-                if min(dtop, dbottom) / max(dtop, dbottom) < ON_STAFFLINE_RATIO_TRHESHOLD:
-                    # Staffspace?
-                    #
-                    # To get staffspace:
-                    #  - Get orientation (below? above?)
-                    _is_staffspace_above = False
-                    if dtop > dbottom:
-                        _is_staffspace_above = True
-
-                    #  - Find staffspaces adjacent to the overlapped staffline.
-                    # NOTE: this will fail with single-staffline staves, because
-                    #       they do NOT have the surrounding staffspaces defined...
-                    _staffline_idx_wrt_staff = _ss_sl_idx_wrt_staff[s.id]
-                    if _is_staffspace_above:
-                        _staffspace_idx_wrt_staff = _staffline_idx_wrt_staff
-                    else:
-                        _staffspace_idx_wrt_staff = _staffline_idx_wrt_staff + 1
-
-                    # Retrieve the given staffsapce
-                    _staff = _staff_per_ss_sl[s.id]
-                    tgt_staffspace = _staff_and_idx2ss[_staff.id][_staffspace_idx_wrt_staff]
-                    # Link to staffspace
-                    link_nodes(node, tgt_staffspace, check_that_nodes_have_the_same_document=False)
-                    # And link to staff
-                    _c_staff = _staff_per_ss_sl[tgt_staffspace.id]
-                    link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
-
-                else:
-                    # Staffline!
-                    link_nodes(node, s, check_that_nodes_have_the_same_document=False)
-                    # And staff:
-                    _c_staff = _staff_per_ss_sl[s.id]
-                    link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
-            elif len(overlapped_stafflines) == 0:
-                # Staffspace!
-                # Link to the staffspace with which the notehead has
-                # greatest vertical overlap.
-                #
-                # Interesting corner case:
-                # Sometimes noteheads "hang out" of the upper/lower
-                # staffspace, so they are not entirely covered.
-                overlapped_staffspaces = {}
-                for _ss_i, s in enumerate(staffspaces):
-                    if s.top <= node.top <= s.bottom:
-                        overlapped_staffspaces[_ss_i] = min(s.bottom, node.bottom) - node.top
-                    elif node.top <= s.top <= node.bottom:
-                        overlapped_staffspaces[_ss_i] = s.bottom - max(node.top, s.top)
-
-                if len(overlapped_staffspaces) == 0:
-                    logging.warning('Notehead {0}: no overlapped staffline object, no leger line!'
-                                    ' Expecting it will be attached to leger line and staff later on.'
-                                    ''.format(node.uid))
-                    continue
-
-                _ss_i_max = max(list(overlapped_staffspaces.keys()),
-                                key=lambda x: overlapped_staffspaces[x])
-                max_overlap_staffspace = staffspaces[_ss_i_max]
-                link_nodes(node, max_overlap_staffspace, check_that_nodes_have_the_same_document=False)
-                _c_staff = _staff_per_ss_sl[max_overlap_staffspace.id]
-                link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
-
-            elif len(overlapped_stafflines) == 2:
-                # Staffspace between those two lines.
-                s1 = overlapped_stafflines[0]
-                s2 = overlapped_stafflines[1]
-
-                _staff1 = _staff_per_ss_sl[s1.id]
-                _staff2 = _staff_per_ss_sl[s2.id]
-                if _staff1.id != _staff2.id:
-                    raise ValueError('Really weird notehead overlapping two stafflines'
-                                     ' from two different staves: {0}'.format(node.uid))
-
-                _staffspace_idx = _ss_sl_idx_wrt_staff[s2.id]
-                s = _staff_and_idx2ss[_staff2.id][_staffspace_idx]
-                link_nodes(node, s, check_that_nodes_have_the_same_document=False)
-                # And link to staff:
-                _c_staff = _staff_per_ss_sl[s.id]
-                link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
-
-            elif len(overlapped_stafflines) > 2:
-                logging.warning('Really weird notehead overlapping more than 2 stafflines:'
-                                ' {0} (permissive: linking to middle staffline)'.format(node.uid))
-                # use the middle staffline -- this will be an error anyway,
-                # but we want to export some MIDI more or less no matter what
-                s_middle = overlapped_stafflines[len(overlapped_stafflines) // 2]
-                link_nodes(node, s_middle, check_that_nodes_have_the_same_document=False)
-                # And staff:
-                _c_staff = _staff_per_ss_sl[s_middle.id]
-                link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
-
-    return nodes
+"""This module implements functions for manipulating staffline symbols.
+Mostly it is support for going from detected staffline fragments
+to full staff objects and relationships; this machinery is called
+e.g. by pressing "shift+s" in MUSCIMarker."""
+import collections
+import logging
+import pprint
+
+import numpy
+from skimage.filters import gaussian
+from skimage.morphology import watershed
+from typing import List, Tuple
+
+from mung.graph import NotationGraph, find_noteheads_on_staff_linked_to_leger_line
+from mung.constants import InferenceEngineConstants
+from mung.node import Node, draw_nodes_on_empty_canvas, link_nodes
+from mung.utils import compute_connected_components
+
+_CONST = InferenceEngineConstants()
+
+
+def __has_parent_staff(node: Node, nodes: List[Node]) -> bool:
+    id_to_node_mapping = {c.id: c for c in nodes}
+    staff_inlinks = [id_to_node_mapping[i] for i in node.inlinks
+                     if id_to_node_mapping[i].class_name == _CONST.STAFF]
+    return len(staff_inlinks) > 0
+
+
+def __has_child_staffspace(staff: Node, nodes: List[Node]) -> bool:
+    id_to_node_mapping = {c.id: c for c in nodes}
+    staffline_outlinks = [id_to_node_mapping[i] for i in staff.outlinks
+                          if id_to_node_mapping[i].class_name == _CONST.STAFFSPACE]
+    return len(staffline_outlinks) > 0
+
+
+def __has_neighbor_staffspace(staffline: Node, nodes: List[Node]) -> bool:
+    id_to_node_mapping = {c.id: c for c in nodes}
+    # Find parent staff
+    if not __has_parent_staff(staffline, nodes):
+        return False
+    parent_staffs = [id_to_node_mapping[i] for i in staffline.inlinks
+                     if id_to_node_mapping[i].class_name == _CONST.STAFF]
+    if len(parent_staffs) > 1:
+        raise ValueError('More than one parent staff for staffline {0}!'
+                         ''.format(staffline.id))
+    staff = parent_staffs[0]
+    return __has_child_staffspace(staff, nodes)
+
+
+def merge_staffline_segments(nodes: List[Node], margin: int = 10) -> List[Node]:
+    """Given a list of Nodes that contain some staffline
+    objects, generates a new list where the stafflines
+    are merged based on their horizontal projections.
+    Basic step for going from the staffline detection masks to
+    the actual staffline objects.
+
+    Assumes that stafflines are straight: their bounding boxes
+    do not touch or overlap.
+
+    :return: A modified Node list: the original staffline-class
+        symbols are replaced by the merged ones. If the original stafflines
+        had any inlinks, they are preserved (mapped to the new staffline).
+    """
+    already_processed_stafflines = [node for node in nodes
+                                    if (node.class_name == _CONST.STAFFLINE) and
+                                    __has_parent_staff(node, nodes)]
+    # margin is used to avoid the stafflines touching the edges,
+    # which could perhaps break some assumptions down the line.
+    old_staffline_nodes = [c for c in nodes
+                           if (c.class_name == _CONST.STAFFLINE) and
+                           not __has_parent_staff(c, nodes)]
+    if len(old_staffline_nodes) == 0:
+        logging.info('merge_staffline_segments: nothing new to do!')
+        return nodes
+
+    canvas, (_t, _l) = draw_nodes_on_empty_canvas(old_staffline_nodes)
+
+    _staffline_bboxes, staffline_masks = staffline_bboxes_and_masks_from_horizontal_merge(canvas)
+    # Bounding boxes need to be adjusted back with respect to the original image!
+    staffline_bboxes = [(t + _t, l + _l, b + _t, r + _l) for t, l, b, r in _staffline_bboxes]
+
+    # Create the Nodes.
+    next_node_id = max([c.id for c in nodes]) + 1
+    dataset = nodes[0].dataset
+    document = nodes[0].document
+
+    #  - Create the staffline Nodes
+    staffline_nodes = []
+    for sl_bb, sl_m in zip(staffline_bboxes, staffline_masks):
+        t, l, b, r = sl_bb
+        c = Node(id_=next_node_id,
+                 class_name=_CONST.STAFFLINE,
+                 top=t, left=l, height=b - t, width=r - l,
+                 mask=sl_m,
+                 dataset=dataset, document=document)
+        staffline_nodes.append(c)
+        next_node_id += 1
+
+    non_staffline_nodes = [c for c in nodes
+                           if c.class_name != _CONST.STAFFLINE]
+    old_staffline_ids = set([c.id for c in old_staffline_nodes])
+    old2new_staffline_id_map = {}
+    for os in old_staffline_nodes:
+        for ns in staffline_nodes:
+            if os.overlaps(ns):
+                old2new_staffline_id_map[os.id] = ns
+
+    logging.info('Re-linking from the old staffline objects to new ones.')
+    for c in non_staffline_nodes:
+        new_outlinks = []
+        for o in c.outlinks:
+            if o in old_staffline_ids:
+                new_staffline = old2new_staffline_id_map[o]
+                new_outlinks.append(new_staffline.id)
+                new_staffline.inlinks.append(c.id)
+            else:
+                new_outlinks.append(o)
+
+    output = non_staffline_nodes + staffline_nodes + already_processed_stafflines
+    return output
+
+
+def staffline_bboxes_and_masks_from_horizontal_merge(mask: numpy.ndarray) -> \
+        Tuple[List[Tuple[int, int, int, int]], List[numpy.ndarray]]:
+    """Returns a list of staff_line bboxes and masks
+     computed from the input mask, with
+    each set of connected components in the mask that has at least
+    one pixel in a neighboring or overlapping row is assigned to
+    the same label. Intended for finding staffline masks from individual
+    components of the stafflines (for this purpose, you have to assume
+    that the stafflines are straight)."""
+    logging.info('Getting staffline connected components.')
+
+    cc, labels, bboxes = compute_connected_components(mask)
+
+    logging.info('Getting staffline component vertical projections')
+    #  - Use vertical dimension of CCs to determine which ones belong together
+    #    to form stafflines. (Criterion: row overlap.)
+    n_rows, n_cols = mask.shape
+    # For each row of the image: which CCs have pxs on that row?
+    intervals = [[] for _ in range(n_rows)]
+    for label, (t, l, b, r) in list(bboxes.items()):
+        if label == 0:
+            continue
+        # Ignore very short staffline segments that can easily be artifacts
+        # and should not affect the vertical range of the staffline anyway.
+        # The "8" is a magic number, no good reason for specifically 8.
+        # (It should be some proportion of the image width, like 0.01.)
+        if (r - l) < 8:
+            continue
+        for row in range(t, b):
+            intervals[row].append(label)
+
+    logging.warning('Grouping staffline connected components into stafflines.')
+    # For each staffline, we collect the CCs that it is made of. We assume stafflines
+    # are separated from each other by at least one empty row.
+    staffline_components = []
+    _in_staffline = False
+    _current_staffline_components = []
+    for r_labels in intervals:
+        if not _in_staffline:
+            # Last row did not contain staffline components.
+            if len(r_labels) == 0:
+                # No staffline component on current row
+                continue
+            else:
+                _in_staffline = True
+                _current_staffline_components += r_labels
+        else:
+            # Last row contained staffline components.
+            if len(r_labels) == 0:
+                # Current staffline has no more rows.
+                staffline_components.append(set(_current_staffline_components))
+                _current_staffline_components = []
+                _in_staffline = False
+                continue
+            else:
+                # Current row contains staffline components: the current
+                # staffline continues.
+                _current_staffline_components += r_labels
+
+    logging.info('No. of stafflines, with component groups: {0}'
+                 ''.format(len(staffline_components)))
+
+    # Now: merge the staffline components into one bbox/mask.
+    logging.info('Merging staffline components into staffline bboxes and masks.')
+    staffline_bboxes = []
+    staffline_masks = []
+    for sc in sorted(staffline_components,
+                     key=lambda c: min([bboxes[cc][0]
+                                        for cc in c])):  # Sorted top-down
+        st, sl, sb, sr = n_rows, n_cols, 0, 0
+        for component in sc:
+            t, l, b, r = bboxes[component]
+            st, sl, sb, sr = min(t, st), min(l, sl), max(b, sb), max(r, sr)
+        # Here, again, we assume that no two "real" stafflines have overlapping
+        # bounding boxes.
+        _sm = mask[st:sb, sl:sr]
+        staffline_bboxes.append((st, sl, sb, sr))
+        staffline_masks.append(_sm)
+
+    # Check if n. of stafflines is divisible by 5
+    n_stafflines = len(staffline_bboxes)
+    logging.warning('\tTotal stafflines: {0}'.format(n_stafflines))
+    if n_stafflines % 5 != 0:
+        raise ValueError('Number of stafflines is not divisible by 5!')
+
+    return staffline_bboxes, staffline_masks
+
+
+def staff_bboxes_and_masks_from_staffline_bboxes_and_image(staffline_bboxes, mask) -> \
+        Tuple[List[Tuple[int, int, int, int]], List[numpy.ndarray]]:
+    logging.warning('Creating staff bboxes and masks.')
+
+    #  - Go top-down and group the stafflines by five to get staves.
+    #    (The staffline bboxes are already sorted top-down.)
+    staff_bboxes = []
+    staff_masks = []
+
+    n_stafflines = len(staffline_bboxes)
+    for i in range(n_stafflines // 5):
+        _sbb = staffline_bboxes[5 * i:5 * (i + 1)]
+        _st = min([bb[0] for bb in _sbb])
+        _sl = min([bb[1] for bb in _sbb])
+        _sb = max([bb[2] for bb in _sbb])
+        _sr = max([bb[3] for bb in _sbb])
+        staff_bboxes.append((_st, _sl, _sb, _sr))
+        staff_masks.append(mask[_st:_sb, _sl:_sr])
+
+    logging.warning('Total staffs: {0}'.format(len(staff_bboxes)))
+
+    return staff_bboxes, staff_masks
+
+
+def staffline_surroundings_mask(staffline_node: Node) -> Tuple[numpy.ndarray, numpy.ndarray]:
+    """Find the parts of the staffline's bounding box which lie
+    above or below the actual staffline.
+
+    These areas will be very small for straight stafflines,
+    but might be considerable when staffline curvature grows.
+    """
+    # We segment both masks into "above staffline" and "below staffline"
+    # areas.
+    elevation = staffline_node.mask * 255
+    # Blur, to plug small holes somewhat:
+    elevation = gaussian(elevation, sigma=1.0)
+    # Prepare the segmentation markers: 1 is ABOVE, 2 is BELOW
+    markers = numpy.zeros(staffline_node.mask.shape)
+    markers[0, :] = 1
+    markers[-1, :] = 2
+    markers[staffline_node.mask != 0] = 0
+    seg = watershed(elevation, markers)
+
+    bmask = numpy.ones(seg.shape)
+    bmask[seg != 2] = 0
+    tmask = numpy.ones(seg.shape)
+    tmask[seg != 1] = 0
+
+    return bmask, tmask
+
+
+def build_staff_nodes(nodes: List[Node]) -> List[Node]:
+    """Derives staff objects from staffline objects.
+
+    Assumes each staff has 5 stafflines.
+
+    Assumes the stafflines have already been merged."""
+    stafflines = [c for c in nodes
+                  if c.class_name == _CONST.STAFFLINE and
+                  not __has_parent_staff(c, nodes)]
+    if len(stafflines) == 0:
+        return []
+
+    staffline_bboxes = [c.bounding_box for c in stafflines]
+    canvas, (_t, _l) = draw_nodes_on_empty_canvas(stafflines)
+
+    logging.warning('Creating staff bboxes and masks.')
+
+    #  - Go top-down and group the stafflines by five to get staves.
+    #    (The staffline bboxes are already sorted top-down.)
+    staff_bboxes = []
+    staff_masks = []
+
+    n_stafflines = len(stafflines)
+    for i in range(n_stafflines // 5):
+        _sbb = staffline_bboxes[5 * i:5 * (i + 1)]
+        _st = min([bb[0] for bb in _sbb])
+        _sl = min([bb[1] for bb in _sbb])
+        _sb = max([bb[2] for bb in _sbb])
+        _sr = max([bb[3] for bb in _sbb])
+        staff_bboxes.append((_st, _sl, _sb, _sr))
+        staff_masks.append(canvas[_st - _t:_sb - _t, _sl - _l:_sr - _l])
+
+    logging.info('Creating staff Nodes')
+    next_node_id = max([c.id for c in nodes]) + 1
+    dataset = nodes[0].dataset
+    document = nodes[0].document
+
+    staffs = []
+    for s_bb, s_m in zip(staff_bboxes, staff_masks):
+        t, l, b, r = s_bb
+        staff = Node(id_=next_node_id,
+                     class_name=_CONST.STAFF,
+                     top=t, left=l, height=b - t, width=r - l,
+                     mask=s_m,
+                     dataset=dataset, document=document)
+        staffs.append(staff)
+        next_node_id += 1
+
+    for i, sc in enumerate(staffs):
+        sl_from = 5 * i
+        sl_to = 5 * (i + 1)
+        for sl in stafflines[sl_from:sl_to]:
+            sl.inlinks.append(sc.id)
+            sc.outlinks.append(sl.id)
+
+    return staffs
+
+
+def build_staffspace_nodes(nodes: List[Node]) -> List[Node]:
+    """Creates the staffspace objects based on stafflines
+    and staffs. There is a staffspace between each two stafflines,
+    one on the top side of each staff, and one on the bottom
+    side for each staff (corresponding e.g. to positions of g5 and d4
+    with the standard G-clef).
+
+    Note that staffspaces do not assume anything about the number
+    of stafflines per staff. However, single-staffline staffs will
+    not have the outer staffspaces generated (there is nothing to derive
+    their size from), for now.
+
+    :param nodes: A list of Nodes that must contain
+        all the relevant stafflines and staffs.
+
+    :return: A list of staffspace Nodes.
+    """
+    next_node_id = max([c.id for c in nodes]) + 1
+    dataset = nodes[0].dataset
+    document = nodes[0].document
+
+    staff_nodes = [node for node in nodes
+                   if node.class_name == _CONST.STAFF
+                   and not __has_child_staffspace(node, nodes)]
+    staffline_nodes = [node for node in nodes
+                       if node.class_name == _CONST.STAFFLINE
+                       and not __has_neighbor_staffspace(node, nodes)]
+
+    staff_spaces = []
+
+    for i, staff in enumerate(staff_nodes):
+        current_stafflines = [sc for sc in staffline_nodes
+                              if sc.id in staff.outlinks]
+        sorted_stafflines = sorted(current_stafflines, key=lambda x: x.top)
+
+        current_staffspace_nodes = []
+
+        # Percussion single-line staves do not have staffspaces.
+        if len(sorted_stafflines) == 1:
+            continue
+
+        #################
+        # Internal staffspace
+        for s1, s2 in zip(sorted_stafflines[:-1], sorted_stafflines[1:]):
+            # s1 is the UPPER staffline, s2 is the LOWER staffline
+            # Left and right limits: to simplify things, we take the column
+            # *intersection* of (s1, s2). This gives the invariant that
+            # the staffspace is limited from top and bottom in each of its columns.
+            l = max(s1.left, s2.left)
+            r = min(s1.right, s2.right)
+
+            # Shift s1, s2 to the right by this much to have the cols. align
+            # All of these are non-negative.
+            dl1, dl2 = l - s1.left, l - s2.left
+            dr1, dr2 = s1.right - r, s2.right - r
+
+            # The stafflines are not necessarily straight,
+            # so top is given for the *topmost bottom edge* of the top staffline + 1
+
+            # First create mask
+            canvas = numpy.zeros((s2.bottom - s1.top, r - l), dtype='uint8')
+
+            # Paste masks into canvas.
+            # This assumes that the top of the bottom staffline is below
+            # the top of the top staffline... and that the bottom
+            # of the top staffline is above the bottom of the bottom
+            # staffline. This may not hold in very weird situations,
+            # but it's good for now.
+            logging.debug(s1.bounding_box, s1.mask.shape)
+            logging.debug(s2.bounding_box, s2.mask.shape)
+            logging.debug(canvas.shape)
+            logging.debug('l={0}, dl1={1}, dl2={2}, r={3}, dr1={4}, dr2={5}'
+                          ''.format(l, dl1, dl2, r, dr1, dr2))
+            # canvas[:s1.height, :] += s1.mask[:, dl1:s1.width-dr1]
+            # canvas[-s2.height:, :] += s2.mask[:, dl2:s2.width-dr2]
+
+            # We have to deal with staffline interruptions.
+            # One way to do this
+            # is watershed fill: put markers along the bottom and top
+            # edge, use mask * 10000 as elevation
+
+            s1_above, s1_below = staffline_surroundings_mask(s1)
+            s2_above, s2_below = staffline_surroundings_mask(s2)
+
+            # Get bounding boxes of the individual stafflines' masks
+            # that intersect with the staffspace bounding box, in terms
+            # of the staffline bounding box.
+            s1_t, s1_l, s1_b, s1_r = 0, dl1, \
+                                     s1.height, s1.width - dr1
+            s1_h, s1_w = s1_b - s1_t, s1_r - s1_l
+            s2_t, s2_l, s2_b, s2_r = canvas.shape[0] - s2.height, dl2, \
+                                     canvas.shape[0], s2.width - dr2
+            s2_h, s2_w = s2_b - s2_t, s2_r - s2_l
+
+            logging.debug(s1_t, s1_l, s1_b, s1_r, (s1_h, s1_w))
+
+            # We now take the intersection of s1_below and s2_above.
+            # If there is empty space in the middle, we fill it in.
+            staffspace_mask = numpy.ones(canvas.shape)
+            staffspace_mask[s1_t:s1_b, :] -= (1 - s1_below[:, dl1:s1.width - dr1])
+            staffspace_mask[s2_t:s2_b, :] -= (1 - s2_above[:, dl2:s2.width - dr2])
+
+            ss_top = s1.top
+            ss_bottom = s2.bottom
+            ss_left = l
+            ss_right = r
+
+            staff_space = Node(next_node_id, _CONST.STAFFSPACE,
+                               top=ss_top, left=ss_left,
+                               height=ss_bottom - ss_top,
+                               width=ss_right - ss_left,
+                               mask=staffspace_mask,
+                               dataset=dataset, document=document)
+
+            staff_space.inlinks.append(staff.id)
+            staff.outlinks.append(staff_space.id)
+
+            current_staffspace_nodes.append(staff_space)
+
+            next_node_id += 1
+
+        ##########
+        # Add top and bottom staffspace.
+        # These outer staffspaces will have the width
+        # of their bottom neighbor, and height derived
+        # from its mask columns.
+        # This is quite approximate, but it should do.
+
+        # Upper staffspace
+        tsl = sorted_stafflines[0]
+        tsl_heights = tsl.mask.sum(axis=0)
+        tss = current_staffspace_nodes[0]
+        tss_heights = tss.mask.sum(axis=0)
+
+        uss_top = max(0, tss.top - max(tss_heights))
+        uss_left = tss.left
+        uss_width = tss.width
+        # We use 1.5, so that large noteheads
+        # do not "hang out" of the staffspace.
+        uss_height = int(tss.height / 1.2)
+        # Shift because of height downscaling:
+        uss_top += tss.height - uss_height
+        uss_mask = tss.mask[:uss_height, :] * 1
+
+        staff_space = Node(next_node_id, _CONST.STAFFSPACE,
+                           top=uss_top, left=uss_left,
+                           height=uss_height,
+                           width=uss_width,
+                           mask=uss_mask,
+                           dataset=dataset, document=document)
+        current_staffspace_nodes.append(staff_space)
+        staff.outlinks.append(staff_space.id)
+        staff_space.inlinks.append(staff.id)
+        next_node_id += 1
+
+        # Lower staffspace
+        bss = current_staffspace_nodes[-2]
+        bss_heights = bss.mask.sum(axis=0)
+        bsl = sorted_stafflines[-1]
+        bsl_heights = bsl.mask.sum(axis=0)
+
+        lss_top = bss.bottom  # + max(bsl_heights)
+        lss_left = bss.left
+        lss_width = bss.width
+        lss_height = int(bss.height / 1.2)
+        lss_mask = bss.mask[:lss_height, :] * 1
+
+        staff_space = Node(next_node_id, _CONST.STAFFSPACE,
+                           top=lss_top, left=lss_left,
+                           height=lss_height,
+                           width=lss_width,
+                           mask=lss_mask,
+                           dataset=dataset, document=document)
+        current_staffspace_nodes.append(staff_space)
+        staff.outlinks.append(staff_space.id)
+        staff_space.inlinks.append(staff.id)
+        next_node_id += 1
+
+        staff_spaces += current_staffspace_nodes
+
+    return staff_spaces
+
+
+def add_staff_relationships(nodes: List[Node],
+                            notehead_staffspace_threshold: float = 0.2,
+                            reprocess_noteheads_inside_staff_with_lls: bool = True):
+    """Adds the relationships from various symbols to staff objects:
+    stafflines, staffspaces, and staffs.
+
+    :param nodes: The list of Nodes in the document. Must
+        include the staff objects.
+
+    :param notehead_staffspace_threshold: A notehead is considered to be
+        on a staffline if it intersects a staffline, and the ratio between
+        how far above the staffline and how far below the staffline it reaches
+        is at least this (default: 0.2). The ratio is computed both ways:
+        d_top / d_bottom and d_bottom / d_top, and the minimum is taken,
+        so the default in effect restricts d_top / d_bottom between 0.2 and 0.8:
+        in other words, the imbalance of the notehead's bounding box around
+        the staffline should be less than 1:4.
+
+    :param reprocess_noteheads_inside_staff_with_lls: If set to True, will check against noteheads
+        that are connected to leger lines, but intersect a staffline. If found,
+        will remove their edges before further processing, so that the noteheads
+        will seem properly unprocessed.
+
+        Note that this handling is a bit ad-hoc for now. However, we currently
+        do not have a better place to fit this in, since the Best Practices
+        currently call for first applying the syntactic parser and then
+        adding staff relationships.
+
+    :return: The list of Nodes corresponding to the new graph.
+    """
+    graph = NotationGraph(nodes)
+    id_to_node_mapping = {node.id: node for node in nodes}
+
+    ON_STAFFLINE_RATIO_TRHESHOLD = notehead_staffspace_threshold
+
+    ##########################################################################
+    if reprocess_noteheads_inside_staff_with_lls:
+        ll_noteheads_on_staff = find_noteheads_on_staff_linked_to_leger_line(nodes)
+        logging.info('Reprocessing noteheads that are inside a staff, but have links'
+                     ' to leger lines. Found {0} such noteheads.'
+                     ''.format(len(ll_noteheads_on_staff)))
+        for n in ll_noteheads_on_staff:
+            # Remove all links to leger lines.
+            leger_lines = graph.children(n, class_filter=[_CONST.LEGER_LINE])
+            for ll in leger_lines:
+                graph.remove_edge(n.id, ll.id)
+
+    ##########################################################################
+    logging.info('Find the staff-related symbols')
+    staffs = [c for c in nodes if c.class_name == _CONST.STAFF]
+
+    staff_related_symbols = collections.defaultdict(list)
+    notehead_symbols = collections.defaultdict(list)
+    rest_symbols = collections.defaultdict(list)
+    for node in nodes:
+        if node.class_name in _CONST.STAFF_RELATED_CLASS_NAMES:
+            # Check if it already has a staff link
+            if not graph.has_children(node, [_CONST.STAFF]):
+                staff_related_symbols[node.class_name].append(node)
+        if node.class_name in _CONST.NOTEHEAD_CLASS_NAMES:
+            if not graph.has_children(node, [_CONST.STAFF]):
+                notehead_symbols[node.class_name].append(node)
+        if node.class_name in _CONST.REST_CLASS_NAMES:
+            if not graph.has_children(node, [_CONST.STAFF]):
+                rest_symbols[node.class_name].append(node)
+
+    ##########################################################################
+    logging.info('Adding staff relationships')
+    #  - Which direction do the relationships lead in?
+    #    Need to define this.
+    #
+    # Staff -> symbol?
+    # Symbol -> staff?
+    # It does not really matter, but it's more intuitive to attach symbols
+    # onto a pre-existing staff. So, symbol -> staff.
+    for class_name, cs in list(staff_related_symbols.items()):
+        for node in cs:
+            # Find the related staff. Relatedness is measured by row overlap.
+            # That means we have to modify the staff bounding box to lead
+            # from the leftmost to the rightmost column. This holds
+            # especially for the staff_grouping symbols.
+            for s in staffs:
+                st, sl, sb, sr = s.bounding_box
+                sl = 0
+                sr = max(sr, node.right)
+                if node.overlaps((st, sl, sb, sr)):
+                    link_nodes(node, s, check_that_nodes_have_the_same_document=False)
+
+    ##########################################################################
+    logging.info('Adding rest --> staff relationships.')
+    for class_name, cs in list(rest_symbols.items()):
+        for node in cs:
+            closest_staff = min([s for s in staffs],
+                                key=lambda x: ((x.bottom + x.top) / 2. - (
+                                        node.bottom + node.top) / 2.) ** 2)
+            link_nodes(node, closest_staff, check_that_nodes_have_the_same_document=False)
+
+    ##########################################################################
+    logging.info('Adding notehead relationships.')
+
+    # NOTE:
+    # This part should NOT rely on staffspace masks in any way!
+    # They are highly unreliable.
+
+    # Sort the staff objects top-down. Assumes stafflines do not cross,
+    # and that there are no crazy curves at the end that would make the lower
+    # stafflines stick out over the ones above them...
+    stafflines = [c for c in nodes if c.class_name == _CONST.STAFFLINE]
+    stafflines = sorted(stafflines, key=lambda c: c.top)
+    staffspaces = [c for c in nodes if c.class_name == _CONST.STAFFSPACE]
+    staffspaces = sorted(staffspaces, key=lambda c: c.top)
+    staves = [c for c in nodes if c.class_name == _CONST.STAFF]
+    staves = sorted(staves, key=lambda c: c.top)
+
+    logging.info('Stafflines: {0}'.format(len(stafflines)))
+    logging.info('Staffspaces: {0}'.format(len(staffspaces)))
+    logging.info('Staves: {0}'.format(len(staves)))
+
+    # Indexing data structures.
+    #
+    # We need to know:
+    #  - per staffline and staffspace: its containing staff
+    _staff_per_ss_sl = {}
+    #  - per staffline and staffspace: its index (top to bottom) within the staff
+    _ss_sl_idx_wrt_staff = {}
+    # Reverse indexes:
+    # If I know which staff (by id) and which index of staffline/staffspace,
+    # I want to retrieve the given staffline/staffspace Node:
+    _staff_and_idx2ss = collections.defaultdict(dict)
+    _staff_and_idx2sl = collections.defaultdict(dict)
+
+    # Build the indexes
+    for _staff in staves:
+        # Keep the top-down ordering from above:
+        _s_stafflines = [_staffline for _staffline in stafflines
+                         if _staff.id in _staffline.inlinks]
+        _s_staffspaces = [_staffspace for _staffspace in staffspaces
+                          if _staff.id in _staffspace.inlinks]
+        for i, _sl in enumerate(_s_stafflines):
+            _staff_per_ss_sl[_sl.id] = _staff
+            _ss_sl_idx_wrt_staff[_sl.id] = i
+            _staff_and_idx2sl[_staff.id][i] = _sl
+            logging.debug('Staff {0}: stafflines {1}'.format(_staff.id,
+                                                             _staff_and_idx2sl[_staff.id]))
+        for i, _ss in enumerate(_s_staffspaces):
+            _staff_per_ss_sl[_ss.id] = _staff
+            _ss_sl_idx_wrt_staff[_ss.id] = i
+            _staff_and_idx2ss[_staff.id][i] = _ss
+
+    logging.debug(pprint.pformat(dict(_staff_and_idx2ss)))
+
+    for class_name, cs in list(notehead_symbols.items()):
+        for node in cs:
+
+            ct, cl, cb, cr = node.bounding_box
+
+            ################
+            # Add relationship to given staffline or staffspace.
+
+            # If notehead has leger lines, skip it for now.
+            has_leger_line = False
+            for outlink in node.outlinks:
+                if id_to_node_mapping[outlink].class_name == _CONST.LEGER_LINE:
+                    has_leger_line = True
+                    break
+
+            if has_leger_line:
+                # Attach to the appropriate staff:
+                # meaning, staff closest to the innermost leger line.
+                leger_lines = [id_to_node_mapping[o] for o in node.outlinks
+                               if id_to_node_mapping[o].class_name == _CONST.LEGER_LINE]
+                # Furthest from notehead's top is innermost.
+                # (If notehead is below staff and crosses a ll., one
+                #  of these numbers will be negative. But that doesn't matter.)
+                ll_max_dist = max(leger_lines, key=lambda leger_line: leger_line.top - node.top)
+                # Find closest staff to max-dist leger ine
+                staff_min_dist = min(staves,
+                                     key=lambda ss: min((ll_max_dist.bottom - ss.top) ** 2,
+                                                        (ll_max_dist.top - ss.bottom) ** 2))
+                distance_of_closest_staff = (ll_max_dist.top + ll_max_dist.bottom) / 2 \
+                                            - (staff_min_dist.top + staff_min_dist.bottom) / 2
+                if numpy.abs(distance_of_closest_staff) > (50 + 0.5 * staff_min_dist.height):
+                    logging.debug('Trying to join notehead with leger line to staff,'
+                                  ' but the distance is larger than 50. Notehead: {0},'
+                                  ' leger line: {1}, staff: {2}, distance: {3}'
+                                  ''.format(node.uid, ll_max_dist.uid, staff_min_dist.id,
+                                            distance_of_closest_staff))
+                else:
+                    link_nodes(node, staff_min_dist, check_that_nodes_have_the_same_document=False)
+                continue
+
+            # - Find the related staffline.
+            # - Because of curved stafflines, this has to be done w.r.t.
+            #   the horizontal position of the notehead.
+            # - Also, because stafflines are NOT filled in (they do not have
+            #   intersections annotated), it is necessary to use a wider
+            #   window than just the notehead.
+            # - We will assume that STAFFLINES DO NOT CROSS.
+            #   (That is a reasonable assumption.)
+            #
+            # - For now, we only work with more or less straight stafflines.
+
+            overlapped_stafflines = []
+            overlapped_staffline_idxs = []
+            for i, s in enumerate(stafflines):
+                # This is the assumption of straight stafflines!
+                if (ct <= s.top <= cb) or (ct <= s.bottom <= cb):
+                    overlapped_stafflines.append(s)
+                    overlapped_staffline_idxs.append(i)
+
+            if node.id < 10:
+                logging.info('Notehead {0} ({1}): overlaps {2} stafflines'.format(node.uid, node.bounding_box,
+                                                                                  len(overlapped_stafflines)))
+
+            if len(overlapped_stafflines) == 1:
+                s = overlapped_stafflines[0]
+                dtop = s.top - ct
+                dbottom = cb - s.bottom
+
+                logging.info('Notehead {0}, staffline {1}: ratio {2:.2f}'
+                             ''.format(node.id, s.id, min(dtop, dbottom) / max(dtop, dbottom)))
+                if min(dtop, dbottom) / max(dtop, dbottom) < ON_STAFFLINE_RATIO_TRHESHOLD:
+                    # Staffspace?
+                    #
+                    # To get staffspace:
+                    #  - Get orientation (below? above?)
+                    _is_staffspace_above = False
+                    if dtop > dbottom:
+                        _is_staffspace_above = True
+
+                    #  - Find staffspaces adjacent to the overlapped staffline.
+                    # NOTE: this will fail with single-staffline staves, because
+                    #       they do NOT have the surrounding staffspaces defined...
+                    _staffline_idx_wrt_staff = _ss_sl_idx_wrt_staff[s.id]
+                    if _is_staffspace_above:
+                        _staffspace_idx_wrt_staff = _staffline_idx_wrt_staff
+                    else:
+                        _staffspace_idx_wrt_staff = _staffline_idx_wrt_staff + 1
+
+                    # Retrieve the given staffsapce
+                    _staff = _staff_per_ss_sl[s.id]
+                    tgt_staffspace = _staff_and_idx2ss[_staff.id][_staffspace_idx_wrt_staff]
+                    # Link to staffspace
+                    link_nodes(node, tgt_staffspace, check_that_nodes_have_the_same_document=False)
+                    # And link to staff
+                    _c_staff = _staff_per_ss_sl[tgt_staffspace.id]
+                    link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
+
+                else:
+                    # Staffline!
+                    link_nodes(node, s, check_that_nodes_have_the_same_document=False)
+                    # And staff:
+                    _c_staff = _staff_per_ss_sl[s.id]
+                    link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
+            elif len(overlapped_stafflines) == 0:
+                # Staffspace!
+                # Link to the staffspace with which the notehead has
+                # greatest vertical overlap.
+                #
+                # Interesting corner case:
+                # Sometimes noteheads "hang out" of the upper/lower
+                # staffspace, so they are not entirely covered.
+                overlapped_staffspaces = {}
+                for _ss_i, s in enumerate(staffspaces):
+                    if s.top <= node.top <= s.bottom:
+                        overlapped_staffspaces[_ss_i] = min(s.bottom, node.bottom) - node.top
+                    elif node.top <= s.top <= node.bottom:
+                        overlapped_staffspaces[_ss_i] = s.bottom - max(node.top, s.top)
+
+                if len(overlapped_staffspaces) == 0:
+                    logging.warning('Notehead {0}: no overlapped staffline object, no leger line!'
+                                    ' Expecting it will be attached to leger line and staff later on.'
+                                    ''.format(node.uid))
+                    continue
+
+                _ss_i_max = max(list(overlapped_staffspaces.keys()),
+                                key=lambda x: overlapped_staffspaces[x])
+                max_overlap_staffspace = staffspaces[_ss_i_max]
+                link_nodes(node, max_overlap_staffspace, check_that_nodes_have_the_same_document=False)
+                _c_staff = _staff_per_ss_sl[max_overlap_staffspace.id]
+                link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
+
+            elif len(overlapped_stafflines) == 2:
+                # Staffspace between those two lines.
+                s1 = overlapped_stafflines[0]
+                s2 = overlapped_stafflines[1]
+
+                _staff1 = _staff_per_ss_sl[s1.id]
+                _staff2 = _staff_per_ss_sl[s2.id]
+                if _staff1.id != _staff2.id:
+                    raise ValueError('Really weird notehead overlapping two stafflines'
+                                     ' from two different staves: {0}'.format(node.uid))
+
+                _staffspace_idx = _ss_sl_idx_wrt_staff[s2.id]
+                s = _staff_and_idx2ss[_staff2.id][_staffspace_idx]
+                link_nodes(node, s, check_that_nodes_have_the_same_document=False)
+                # And link to staff:
+                _c_staff = _staff_per_ss_sl[s.id]
+                link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
+
+            elif len(overlapped_stafflines) > 2:
+                logging.warning('Really weird notehead overlapping more than 2 stafflines:'
+                                ' {0} (permissive: linking to middle staffline)'.format(node.uid))
+                # use the middle staffline -- this will be an error anyway,
+                # but we want to export some MIDI more or less no matter what
+                s_middle = overlapped_stafflines[len(overlapped_stafflines) // 2]
+                link_nodes(node, s_middle, check_that_nodes_have_the_same_document=False)
+                # And staff:
+                _c_staff = _staff_per_ss_sl[s_middle.id]
+                link_nodes(node, _c_staff, check_that_nodes_have_the_same_document=False)
+
+    return nodes
```

### Comparing `mung-1.1/mung/utils.py` & `mung-1.2/mung/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-import logging
-
-import numpy
-from skimage.measure import label
-from typing import Tuple, Dict, Any, List
-
-from mung.constants import InferenceEngineConstants as _CONST
-
-
-def connected_components2bboxes(labels: List[List[int]]) -> Dict[int, List[int]]:
-    """Returns a dictionary of bounding boxes (upper left c., lower right c.)
-    for each label.
-
-    >>> labels = [[0, 0, 1, 1], [2, 0, 0, 1], [2, 0, 0, 0], [0, 0, 3, 3]]
-    >>> bboxes = connected_components2bboxes(labels)
-    >>> bboxes[0]
-    [0, 0, 4, 4]
-    >>> bboxes[1]
-    [0, 2, 2, 4]
-    >>> bboxes[2]
-    [1, 0, 3, 1]
-    >>> bboxes[3]
-    [3, 2, 4, 4]
-
-
-    :param labels: The output of cv2.connectedComponents().
-
-    :returns: A dict indexed by labels. The values are quadruplets
-        (xmin, ymin, xmax, ymax) so that the component with the given label
-        lies exactly within labels[xmin:xmax, ymin:ymax].
-    """
-    bboxes = {}
-    for x, row in enumerate(labels):
-        for y, l in enumerate(row):
-            if l not in bboxes:
-                bboxes[l] = [x, y, x + 1, y + 1]
-            else:
-                box = bboxes[l]
-                if x < box[0]:
-                    box[0] = x
-                elif x + 1 > box[2]:
-                    box[2] = x + 1
-                if y < box[1]:
-                    box[1] = y
-                elif y + 1 > box[3]:
-                    box[3] = y + 1
-    return bboxes
-
-
-def compute_connected_components(image: numpy.ndarray) -> \
-        Tuple[int, numpy.ndarray, Dict[int, List[int]]]:
-    labels = label(image, background=0)
-    number_of_connected_components = int(labels.max())
-    bboxes = connected_components2bboxes(labels)
-    return number_of_connected_components, labels, bboxes
-
+import logging
+
+import numpy
+from skimage.measure import label
+from typing import Tuple, Dict, Any, List
+
+def connected_components2bboxes(labels: List[List[int]]) -> Dict[int, List[int]]:
+    """Returns a dictionary of bounding boxes (upper left c., lower right c.)
+    for each label.
+
+    >>> labels = [[0, 0, 1, 1], [2, 0, 0, 1], [2, 0, 0, 0], [0, 0, 3, 3]]
+    >>> bboxes = connected_components2bboxes(labels)
+    >>> bboxes[0]
+    [0, 0, 4, 4]
+    >>> bboxes[1]
+    [0, 2, 2, 4]
+    >>> bboxes[2]
+    [1, 0, 3, 1]
+    >>> bboxes[3]
+    [3, 2, 4, 4]
+
+
+    :param labels: The output of cv2.connectedComponents().
+
+    :returns: A dict indexed by labels. The values are quadruplets
+        (xmin, ymin, xmax, ymax) so that the component with the given label
+        lies exactly within labels[xmin:xmax, ymin:ymax].
+    """
+    bboxes = {}
+    for x, row in enumerate(labels):
+        for y, l in enumerate(row):
+            if l not in bboxes:
+                bboxes[l] = [x, y, x + 1, y + 1]
+            else:
+                box = bboxes[l]
+                if x < box[0]:
+                    box[0] = x
+                elif x + 1 > box[2]:
+                    box[2] = x + 1
+                if y < box[1]:
+                    box[1] = y
+                elif y + 1 > box[3]:
+                    box[3] = y + 1
+    return bboxes
+
+
+def compute_connected_components(image: numpy.ndarray) -> \
+        Tuple[int, numpy.ndarray, Dict[int, List[int]]]:
+    labels = label(image, background=0)
+    number_of_connected_components = int(labels.max())
+    bboxes = connected_components2bboxes(labels)
+    return number_of_connected_components, labels, bboxes
+
```

### Comparing `mung-1.1/mung.egg-info/SOURCES.txt` & `mung-1.2/mung.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.cfg
 setup.py
 mung/__init__.py
 mung/constants.py
 mung/dataset.py
 mung/grammar.py
@@ -15,14 +16,15 @@
 mung.egg-info/PKG-INFO
 mung.egg-info/SOURCES.txt
 mung.egg-info/dependency_links.txt
 mung.egg-info/requires.txt
 mung.egg-info/top_level.txt
 mung2midi/__init__.py
 mung2midi/inference.py
+mung2midi/run_inference.py
 scripts/add_staff_relationships.py
 scripts/add_staffline_symbols.py
 scripts/analyze_agreement.py
 scripts/analyze_annotations.py
 scripts/analyze_tracking_log.py
 scripts/baseline_process_symbols.py
 scripts/get_images_from_muscima.py
```

### Comparing `mung-1.1/mung2midi/inference.py` & `mung-1.2/mung2midi/inference.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,2407 +1,2263 @@
-import collections
-import copy
-import logging
-import operator
-import os
-
-from typing import List, Dict, Tuple
-
-from mung.graph import group_staffs_into_systems, NotationGraph, NotationGraphError
-from mung.constants import InferenceEngineConstants as _CONST
-from mung.node import bounding_box_dice_coefficient, Node
-
-
-class OnsetsInferenceStrategy(object):
-    def __init__(self):
-        self.permissive_desynchronization = True
-        self.precedence_only_for_objects_connected_to_staff = True
-        self.permissive = True
-
-
-class PitchInferenceStrategy(object):
-    def __init__(self):
-        self.permissive = True
-
-
-class PitchInferenceEngineState(object):
-    """This class represents the state of the MIDI pitch inference
-    engine during inference.
-
-    Reading pitch is a stateful operations. One needs to remember
-    how stafflines and staffspaces map to pitch codes. This is governed
-    by two things:
-
-    * The clef, which governs
-    * The accidentals: key signatures and inline accidentals.
-
-    Clef and key signature have unlimited scope which only changes when
-    a new key signature is introduced (or the piece ends). The key
-    signature affects all pitches in the given step class (F, C, G, ...)
-    regardless of octave. Inline accidentals have scope until the next
-    measure separator, and they are only valid within their own octave.
-
-    The pitch inference algorithm is run for each staff separately.
-
-    Base pitch representation
-    -------------------------
-
-    The base pitch corresponds to the pitch encoded by a notehead
-    simply sitting on the given staffline/staffspace, without any
-    regard to accidentals (key signature or inline). It is computed
-    by *distance from center staffline* of a staff, with positive
-    distance corresponding to going *up* and negative for going *down*
-    from the center staffline.
-
-    Accidentals representation
-    --------------------------
-
-    The accidentals are associated also with each staffline/staffspace,
-    as counted from the current center. (This means i.a. that
-    the octave periodicity is 7, not 12.)
-
-    There are two kinds of accidentals based on scope: key signature,
-    and inline. Inline accidentals are valid only up to the next
-    measure_separator, while key signature accidentals are valid
-    up until the key signature changes. Key signature accidentals
-    also apply across all octaves, while inline accidentals only apply
-    on the specific staffline.
-
-    Note that inline accidentals may *cancel* key signature
-    accidentals: they override the key signature when given.
-
-    Key accidentals are given **mod 7**.
-
-    Pitch inference procedure
-    -------------------------
-
-    Iterate through the relevant objects on a staff, sorted left-to-right
-    by left edge.
-    """
-
-    def __init__(self):
-
-        self.base_pitch = None  # type: int
-        '''The MIDI code corresponding to the middle staffline,
-        without modification by key or inline accidentals.'''
-
-        self.base_pitch_step = None  # type: int
-        '''The name of the base pitch: C, D, E, etc.'''
-
-        self.base_pitch_octave = None  # type: int
-        '''The octave where the pitch resides. C4 = c', the middle C.'''
-
-        self.current_clef = None  # type:Node
-        '''Holds the clef Node that is currently valid.'''
-
-        self.current_delta_steps = None  # type: List[int]
-        '''Holds for each staffline delta step (i.e. staffline delta mod 7)
-        the MIDI pitch codes.'''
-
-        self.current_clef_delta_shift = 0  # type: int
-        '''If the clef is in a non-standard position, this number is added
-        to the pitch computation delta.'''
-
-        self.key_accidentals = {}  # type: Dict[int,str]
-        self.inline_accidentals = {}  # type: Dict[int,str]
-
-    def reset(self):
-        self.base_pitch = None
-        self.current_clef = None
-        self.current_delta_steps = None
-        self.key_accidentals = {}
-        self.inline_accidentals = {}
-
-    def __str__(self):
-        lines = list()
-        lines.append('Current pitch inference state:')
-        lines.append('\tbase_pitch: {0}'.format(self.base_pitch))
-        lines.append('\tbase_pitch_step: {0}'.format(self.base_pitch_step))
-        lines.append('\tbase_pitch_octave: {0}'.format(self.base_pitch_octave))
-        if self.current_clef is not None:
-            lines.append('\t_current_clef: {0}'.format(self.current_clef.id))
-        else:
-            lines.append('\t_current_clef: None')
-        lines.append('\t_current_delta_steps: {0}'.format(self.current_delta_steps))
-        lines.append('\t_current_clef_delta_shift: {0}'.format(self.current_clef_delta_shift))
-        lines.append('\tkey_accidentals: {0}'.format(self.key_accidentals))
-        lines.append('\tinline_accidentals: {0}'.format(self.inline_accidentals))
-        return '\n'.join(lines)
-
-    def init_base_pitch(self, clef: Node = None, delta:int=0):
-        """Initializes the base pitch while taking into account
-        the displacement of the clef from its initial position."""
-        self.init_base_pitch_default_staffline(clef)
-        self.current_clef_delta_shift = -1 * delta
-
-    def init_base_pitch_default_staffline(self, clef: Node = None):
-        """Based solely on the clef class name and assuming
-        default stafflines, initialize the base pitch.
-        By default, initializes as though given a gClef."""
-
-        # There should be a mechanism for clefs that are connected
-        # directly to a staffline -- in non-standard positions
-        # (mostly cClefs, like page 03, but there is no reason
-        #  to limit this to cClefs).
-
-        if (clef is None) or (clef.class_name == _CONST.G_CLEF):
-            new_base_pitch = 71
-            new_delta_steps = [0, 1, 2, 2, 1, 2, 2, 2]
-            new_base_pitch_step = 6  # Index into pitch steps.
-            new_base_pitch_octave = 4
-        elif clef.class_name == _CONST.F_CLEF:
-            new_base_pitch = 50
-            new_delta_steps = [0, 2, 1, 2, 2, 2, 1, 2]
-            new_base_pitch_step = 1
-            new_base_pitch_octave = 3
-        elif clef.class_name == _CONST.C_CLEF:
-            new_base_pitch = 60
-            new_delta_steps = [0, 2, 2, 1, 2, 2, 2, 1]
-            new_base_pitch_step = 0
-            new_base_pitch_octave = 4
-        else:
-            raise ValueError('Unrecognized clef class_name: {0}'
-                             ''.format(clef.class_name))
-
-        # Shift the key and inline accidental deltas
-        # according to the change.
-        if self.current_clef is not None:
-            transposition_delta = _CONST.CLEF_CHANGE_DELTA[self.current_clef.class_name][clef.class_name]
-            if transposition_delta != 0:
-                new_key_accidentals = {
-                    (d + transposition_delta) % 7: v
-                    for d, v in list(self.key_accidentals.items())
-                }
-                new_inline_accidentals = {
-                    d + transposition_delta: v
-                    for d, v in list(self.inline_accidentals.items())
-                }
-                self.key_accidentals = new_key_accidentals
-                self.inline_accidentals = new_inline_accidentals
-
-        self.base_pitch = new_base_pitch
-        self.base_pitch_step = new_base_pitch_step
-        self.base_pitch_octave = new_base_pitch_octave
-        self.current_clef = clef
-        self.current_delta_steps = new_delta_steps
-
-    def set_key(self, number_of_sharps:int=0, number_of_flats:int=0):
-        """Initialize the staffline delta --> key accidental map.
-        Currently works only on standard key signatures, where
-        there are no repeating accidentals, no double sharps/flats,
-        and the order of accidentals is the standard major/minor system.
-
-        However, we can deal at least with key signatures that combine
-        sharps and flats (if not more than 7), as seen e.g. in harp music.
-
-        :param number_of_sharps: How many sharps are there in the key signature?
-
-        :param number_of_flats: How many flats are there in the key signature?
-        """
-        if number_of_flats + number_of_sharps > 7:
-            raise ValueError('Cannot deal with key signature that has'
-                             ' more than 7 sharps + flats!')
-
-        if self.base_pitch is None:
-            raise ValueError('Cannot initialize key if base pitch is not known.')
-
-        new_key_accidentals = {}
-
-        # The pitches (F, C, G, D, ...) have to be re-cast
-        # in terms of deltas, mod 7.
-        if (self.current_clef is None) or (self.current_clef.class_name == _CONST.G_CLEF):
-            deltas_sharp = [4, 1, 5, 2, 6, 3, 0]
-            deltas_flat = [0, 3, 6, 2, 5, 1, 4]
-        elif self.current_clef.class_name == _CONST.C_CLEF:
-            deltas_sharp = [3, 0, 4, 1, 5, 2, 6]
-            deltas_flat = [6, 2, 5, 1, 4, 0, 3]
-        elif self.current_clef.class_name == _CONST.F_CLEF:
-            deltas_sharp = [2, 6, 3, 0, 4, 1, 5]
-            deltas_flat = [5, 1, 4, 0, 3, 6, 2]
-        else:
-            raise ValueError("Incorrect clef node set as current_clef {0}.".format(self.current_clef))
-
-        for d in deltas_sharp[:number_of_sharps]:
-            new_key_accidentals[d] = 'sharp'
-        for d in deltas_flat[:number_of_flats]:
-            new_key_accidentals[d] = 'flat'
-
-        self.key_accidentals = new_key_accidentals
-
-    def set_inline_accidental(self, delta:int, accidental:Node):
-        self.inline_accidentals[delta] = accidental.class_name
-
-    def reset_inline_accidentals(self):
-        self.inline_accidentals = {}
-
-    def accidental(self, delta:int) -> int:
-        """Returns the modification, in MIDI code, corresponding
-        to the staffline given by the delta."""
-        pitch_mod = 0
-
-        step_delta = delta % 7
-        if step_delta in self.key_accidentals:
-            if self.key_accidentals[step_delta] == 'sharp':
-                pitch_mod = 1
-            elif self.key_accidentals[step_delta] == 'double_sharp':
-                pitch_mod = 2
-            elif self.key_accidentals[step_delta] == 'flat':
-                pitch_mod = -1
-            elif self.key_accidentals[step_delta] == 'double_flat':
-                pitch_mod = -2
-
-        # Inline accidentals override key accidentals.
-        if delta in self.inline_accidentals:
-            if self.inline_accidentals[delta] == 'natural':
-                logging.info('Natural at delta = {0}'.format(delta))
-                pitch_mod = 0
-            elif self.inline_accidentals[delta] == 'sharp':
-                pitch_mod = 1
-            elif self.inline_accidentals[delta] == 'double_sharp':
-                pitch_mod = 2
-            elif self.inline_accidentals[delta] == 'flat':
-                pitch_mod = -1
-            elif self.inline_accidentals[delta] == 'double_flat':
-                pitch_mod = -2
-        return pitch_mod
-
-    def pitch(self, delta:int) -> int:
-        """Given a staffline delta, returns the current MIDI pitch code.
-
-        (This method is the main interface of the PitchInferenceEngineState.)
-
-        :delta: Distance in stafflines + staffspaces from the middle staffline.
-            Negative delta means distance *below*, positive delta is *above*.
-
-        :returns: The MIDI pitch code for the given delta.
-        """
-        delta += self.current_clef_delta_shift
-
-        # Split this into octave and step components.
-        delta_step = delta % 7
-        delta_octave = delta // 7
-
-        # From the base pitch and clef:
-        step_pitch = self.base_pitch \
-                     + sum(self.current_delta_steps[:delta_step + 1]) \
-                     + (delta_octave * 12)
-        accidental_pitch = self.accidental(delta)
-
-        pitch = step_pitch + accidental_pitch
-
-        if self.current_clef_delta_shift != 0:
-            logging.info('PitchInferenceState: Applied clef-based delta {0},'
-                         ' resulting delta was {1}, pitch {2}'
-                         ''.format(self.current_clef_delta_shift,
-                                   delta, pitch))
-
-        return pitch
-
-    def pitch_name(self, delta:int) -> Tuple[str, int]:
-        """Given a staffline delta, returns the name of the corrensponding pitch."""
-        delta += self.current_clef_delta_shift
-
-        output_step = _CONST.PITCH_STEPS[(self.base_pitch_step + delta) % 7]
-        output_octave = self.base_pitch_octave + ((delta + self.base_pitch_step) // 7)
-
-        output_mod = ''
-        accidental = self.accidental(delta)
-        if accidental == 1:
-            output_mod = _CONST.ACCIDENTAL_CODES['sharp']
-        elif accidental == 2:
-            output_mod = _CONST.ACCIDENTAL_CODES['double_sharp']
-        elif accidental == -1:
-            output_mod = _CONST.ACCIDENTAL_CODES['flat']
-        elif accidental == 2:
-            output_mod = _CONST.ACCIDENTAL_CODES['double_flat']
-
-        return output_step + output_mod, output_octave
-
-
-class PitchInferenceEngine(object):
-    """The Pitch Inference Engine extracts MIDI from the notation
-    graph. To get the MIDI, there are two streams of information
-    that need to be combined: pitches and onsets, where the onsets
-    are necessary both for ON and OFF events.
-
-    Pitch inference is done through the ``infer_pitches()`` method.
-
-    Onsets inference is done in two stages. First, the durations
-    of individual notes (and rests) are computed, then precedence
-    relationships are found and based on the precedence graph
-    and durations, onset times are computed.
-
-    Onset inference
-    ---------------
-
-    Onsets are computed separately by measure, which enables time
-    signature constraint checking.
-
-    (This can be implemented in the precedence graph structure,
-    by (a) not allowing precedence edges to cross measure separators,
-    (b) chaining measure separators, or it can be implemented
-    directly in code. The first option is way more elegant.)
-
-    Creating the precedence graph
-    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-    * Get measure separators.
-    * Chain measure separators in precedence relationships.
-    * Group Nodes by bins between measure separators.
-    * For each staff participating in the current measure
-      (as defined by the relevant measure separator outlinks):
-
-        * Infer precedence between the participating notes & rests,
-        * Attach the sources of the resulting DAG to the leftward
-          measure_separator (if there is none, just leave them
-          as sources).
-
-    Invariants
-    ^^^^^^^^^^
-
-    * There is exactly one measure separator starting each measure,
-      except for the first measure, which has none. That implies:
-      when there are multiple disconnected barlines marking the interface
-      of the same two measures within a system, they are joined under
-      a single measure_separator anyway.
-    * Staff groupings are correct, and systems are read top-down.
-
-    """
-
-    def __init__(self, strategy=PitchInferenceStrategy()):
-        # Static temp data from which the pitches are inferred
-        self.id_to_node_mapping = {}
-
-        self.strategy = strategy
-
-        self.staves = None
-
-        self.clefs = None
-        self.clef_to_staff_map = None
-        self.staff_to_clef_map = None
-
-        self.key_signatures = None
-        self.key_to_staff_map = None
-        self.staff_to_key_map = None
-
-        self.measure_separators = None
-        self.staff_to_msep_map = None
-
-        self.noteheads = None
-        self.staff_to_noteheads_map = None
-
-        # Dynamic temp data: things that change as the pitches are inferred.
-        self.pitch_state = PitchInferenceEngineState()
-
-        # Results
-        self.pitches = None
-        self.pitches_per_staff = None
-
-        self.pitch_names = None
-        self.pitch_names_per_staff = None
-
-        # self.durations_beats = None
-        # self.durations_beats_per_staff = None
-
-    def reset(self):
-        self.__init__()
-
-    def infer_pitches(self, nodes: List[Node], with_names=False):
-        """The main workhorse for pitch inference.
-        Gets a list of Nodes and for each notehead-type
-        symbol, outputs a MIDI code corresponding to the pitch
-        encoded by that notehead.
-
-        Notehead
-        --------
-
-        * Check for ties; if there is an incoming tie, apply
-          the last pitch. (This is necessary because of ties
-          that go across barlines and maintain inline accidentals.)
-        * Determine its staffline delta from the middle staffline.
-        * Check for inline accidentals, apply them to inference state.
-        * Query pitch state with this staffline delta.
-
-        Ties are problematic, because they may reach across
-        staff breaks. This can only be resolved after all staves
-        are resolved and assigned to systems, because until then,
-        it is not clear which staff corresponds to which in the next
-        system. Theoretically, this is near-impossible to resolve,
-        because staves may not continue on the next system (e.g.,
-        instruments that do not play for some time in orchestral scores),
-        so simple staff counting is not foolproof. Some other matching
-        mechanism has to be found, e.g. matching outgoing and incoming
-        ties on the end and beginning of adjacent systems.
-
-        Measure separator
-        -----------------
-
-        * Reset all inline accidentals to empty.
-
-        Clef change
-        -----------
-
-        * Change base pitch
-        * Recompute the key and inline signature delta indexes
-
-        Key change
-        ----------
-
-        * Recompute key deltas
-
-        :param with_names: If set, will return also a dict of
-            id --> pitch names (e.g., {123: 'F#3'}).
-
-        :returns: A dict of ``id`` to MIDI pitch code, with
-            an entry for each (pitched) notehead. If ``with_names``
-            is given, returns a tuple with the id --> MIDI
-            and id --> pitch name dicts.
-
-        """
-        self.id_to_node_mapping = {c.id: c for c in nodes}
-
-        # Initialize pitch temp data.
-        self._collect_symbols_for_pitch_inference(nodes)
-
-        # Staff processing: this is where the inference actually
-        # happens.
-        self.pitches_per_staff = {}
-        self.pitches = {}
-        self.pitch_names_per_staff = {}
-        self.pitch_names = {}
-        # self.durations_beats = {}
-        # self.durations_beats_per_staff = {}
-
-        for staff in self.staves:
-            self.process_staff(staff)
-            self.pitches.update(self.pitches_per_staff[staff.id])
-
-        if with_names:
-            return copy.deepcopy(self.pitches), copy.deepcopy(self.pitch_names)
-        else:
-            return copy.deepcopy(self.pitches)
-
-    def process_staff(self, staff):
-
-        self.pitches_per_staff[staff.id] = {}
-        self.pitch_names_per_staff[staff.id] = {}
-
-        # self.durations_beats_per_staff[staff.id] = {}
-
-        self.pitch_state.reset()
-        self.pitch_state.init_base_pitch()
-
-        queue = sorted(
-            self.staff_to_clef_map[staff.id]
-            + self.staff_to_key_map[staff.id]
-            + self.staff_to_msep_map[staff.id]
-            + self.staff_to_noteheads_map[staff.id],
-            key=lambda x: x.left)
-
-        for q in queue:
-            logging.info('process_staff(): processing object {0}-{1}'
-                         ''.format(q.class_name, q.id))
-            if q.class_name in _CONST.CLEF_CLASS_NAMES:
-                self.process_clef(q)
-            elif q.class_name in _CONST.KEY_SIGNATURE_CLASS_NAMES:
-                self.process_key_signature(q)
-            elif q.class_name in _CONST.MEASURE_SEPARATOR_CLASS_NAMES:
-                self.process_measure_separator(q)
-            elif q.class_name in _CONST.NOTEHEAD_CLASS_NAMES:
-                p, pn = self.process_notehead(q, with_name=True)
-                self.pitches[q.id] = p
-                self.pitches_per_staff[staff.id][q.id] = p
-                self.pitch_names[q.id] = pn
-                self.pitch_names_per_staff[staff.id][q.id] = pn
-
-                ### DEBUG
-                if q.id in [131, 83, 89, 94]:
-                    logging.info('PitchInferenceEngine: Processing notehead {0}'
-                                 ''.format(q.id))
-                    logging.info('{0}'.format(self.pitch_state))
-
-                # b = self.beats(q)
-                # self.durations_beats[q.id] = b
-                # self.durations_beats_per_staff[staff.id][q.id] = b
-
-        return self.pitches_per_staff[staff.id]
-
-    def process_notehead(self, notehead, with_name=False):
-        """This is the main workhorse of the pitch inference engine.
-
-        :param notehead: The notehead-class Node for which we
-            want to infer pitch.
-
-        :param with_name: If set, will return not only the MIDI pitch
-            code, but the name of the encoded note (e.g., F#3) as well.
-        """
-        # Processing ties
-        # ---------------
-        ties = self.__children(notehead, [_CONST.TIE_CLASS_NAME])
-        for t in ties:
-            tied_noteheads = self.__parents(t, _CONST.NOTEHEAD_CLASS_NAMES)
-
-            # Corner cases: mistakes and staff breaks
-            if len(tied_noteheads) > 2:
-                raise ValueError('Tie {0}: joining together more than 2'
-                                 ' noteheads!'.format(t.id))
-            if len(tied_noteheads) < 2:
-                logging.warning('Tie {0}: only one notehead. Staff break?'
-                                ''.format(t.id))
-                break
-
-            left_tied_notehead = min(tied_noteheads, key=lambda x: x.left)
-            if left_tied_notehead.id != notehead.id:
-                try:
-                    p = self.pitches[left_tied_notehead.id]
-                    if with_name:
-                        pn = self.pitch_names[left_tied_notehead.id]
-                        return p, pn
-                    else:
-                        return p
-
-                except KeyError:
-                    raise KeyError('Processing tied notehead {0}:'
-                                   ' preceding notehead {1} has no pitch!'
-                                   ''.format(notehead.id, left_tied_notehead.id))
-
-            # If the condition doesn't hold, then this is the leftward
-            # note in the tie, and its pitch needs to be determined.
-
-        # Obtain notehead delta
-        # ---------------------
-        delta = self.staffline_delta(notehead)
-
-        # ### DEBUG
-        # if notehead.id == 200:
-        #     logging.info('Notehead {0}: delta {1}'.format(notehead.unique_id, delta))
-        #     logging.info('\tdelta_step: {0}'.format(delta % 7))
-        #     logging.info('\tdelta_step pitch sum: {0}'
-        #                  ''.format(sum(self.pitch_state._current_delta_steps[:(delta % 7)+1])))
-
-        # Processing inline accidentals
-        # -----------------------------
-        accidentals = self.__children(notehead, _CONST.ACCIDENTAL_CLASS_NAMES)
-
-        if len(accidentals) > 0:
-
-            # Sanity checks
-            if len(accidentals) > 2:
-                self.__warning_or_error('More than two accidentals attached to notehead'
-                                        ' {0}'.format(notehead.id))
-            elif len(accidentals) == 2:
-                naturals = [a for a in accidentals if a.class_name == 'natural']
-                non_naturals = [a for a in accidentals if a.class_name != 'natural']
-                if len(naturals) == 0:
-                    self.__warning_or_error('More than one non-natural accidental'
-                                            ' attached to notehead {0}'
-                                            ''.format(notehead.id))
-
-                if len(non_naturals) == 0:
-                    self.__warning_or_error('Two naturals attached to one notehead {0}'
-                                            ''.format(notehead.id))
-                    self.pitch_state.set_inline_accidental(delta, naturals[0])
-                else:
-                    self.pitch_state.set_inline_accidental(delta, non_naturals[0])
-
-            elif len(accidentals) == 1:
-                self.pitch_state.set_inline_accidental(delta, accidentals[0])
-
-        # Get the actual pitch
-        # --------------------
-        p = self.pitch_state.pitch(delta)
-
-        ### DEBUG
-        if notehead.id in [131, 83, 89, 94]:
-            logging.info('PitchInferenceEngine: results of pitch processing'
-                         ' for notehead {0}'.format(notehead.id))
-            logging.info('\tties: {0}'.format(ties))
-            logging.info('\taccidentals: {0}'.format(accidentals))
-            logging.info('\tdelta: {0}'.format(delta))
-            logging.info('\tpitch: {0}'.format(p))
-
-        if with_name is True:
-            pn = self.pitch_state.pitch_name(delta)
-            return p, pn
-        else:
-            return p
-
-    def staffline_delta(self, notehead: Node):
-        """Computes the staffline delta (distance from middle stafflines,
-        measured in stafflines and staffspaces) for the given notehead
-        (or any other symbol connected to a staffline/staffspace).
-        Accounts for leger lines.
-        """
-        current_staff = self.__children(notehead, ['staff'])[0]
-        staffline_objects = self.__children(notehead,
-                                            _CONST.STAFFLINE_CLASS_NAMES)
-
-        # Leger lines
-        # ------------
-        if len(staffline_objects) == 0:
-
-            # Processing leger lines:
-            #  - count leger lines
-            lls = self.__children(notehead, _CONST.LEGER_LINE_CLASS_NAME)
-            n_lls = len(lls)
-            if n_lls == 0:
-                raise ValueError('Notehead with no staffline or staffspace,'
-                                 ' but also no leger lines: {0}'
-                                 ''.format(notehead.id))
-
-            #  Determine: is notehead above or below staff?
-            is_above_staff = (notehead.top < current_staff.top)
-
-            #  Determine: is notehead on/next to (closest) leger line?
-            #    This needs to be done *after* we know whether the notehead
-            #    is above/below staff: if the notehead is e.g. above,
-            #    then it would be weird to find out it is in the
-            #    mini-staffspace *below* the closest leger line,
-            #    signalling a mistake in the data.
-            closest_ll = min(lls, key=lambda x: (x.top - notehead.top) ** 2 + (x.bottom - notehead.bottom) ** 2)
-
-            # Determining whether the notehead is on a leger
-            # line or in the adjacent temp staffspace.
-            # This uses a magic number, ON_STAFFLINE_RATIO_THRESHOLD.
-            on_leger_line = True
-
-            ### DEBUG!!!
-            dtop, dbottom = 1, 1
-
-            # Weird situation with notehead vertically *inside* bbox
-            # of leger line (could happen with slanted LLs and very small
-            # noteheads).
-            if closest_ll.top <= notehead.top <= notehead.bottom <= closest_ll.bottom:
-                on_leger_line = True
-
-            # No vertical overlap between LL and notehead
-            elif closest_ll.top > notehead.bottom:
-                on_leger_line = False
-            elif notehead.top > closest_ll.bottom:
-                on_leger_line = False
-
-            # Complicated situations: overlap
-            else:
-                # Notehead "around" leger line.
-                if notehead.top < closest_ll.top <= closest_ll.bottom < notehead.bottom:
-                    dtop = closest_ll.top - notehead.top
-                    dbottom = notehead.bottom - closest_ll.bottom
-
-                    if min(dtop, dbottom) / max(dtop, dbottom) \
-                            < _CONST.ON_STAFFLINE_RATIO_THRESHOLD:
-                        on_leger_line = False
-
-                        # Check orientation congruent with rel. to staff.
-                        # If it is wrong (e.g., notehead mostly under LL
-                        # but above staffline, and looks like off-LL),
-                        # change back to on-LL.
-                        if (dtop > dbottom) and not is_above_staff:
-                            on_leger_line = True
-                            logging.debug('Notehead in LL space with wrong orientation '
-                                          'w.r.t. staff:'
-                                          ' {0}'.format(notehead.id))
-                        if (dbottom > dtop) and is_above_staff:
-                            on_leger_line = True
-                            logging.debug('Notehead in LL space with wrong orientation '
-                                          'w.r.t. staff:'
-                                          ' {0}'.format(notehead.id))
-
-                # Notehead interlaced with leger line, notehead on top
-                elif notehead.top < closest_ll.top <= notehead.bottom <= closest_ll.bottom:
-                    # dtop = closest_ll.top - notehead.top
-                    # dbottom = max(notehead.bottom - closest_ll.top, 1)
-                    # if float(dbottom) / float(dtop) \
-                    #         < _CONST.ON_STAFFLINE_RATIO_TRHESHOLD:
-                    on_leger_line = False
-
-                # Notehead interlaced with leger line, leger line on top
-                elif closest_ll.top <= notehead.top <= closest_ll.bottom < notehead.bottom:
-                    # dtop = max(closest_ll.bottom - notehead.top, 1)
-                    # dbottom = notehead.bottom - closest_ll.bottom
-                    # if float(dtop) / float(dbottom) \
-                    #         < _CONST.ON_STAFFLINE_RATIO_TRHESHOLD:
-                    on_leger_line = False
-
-                else:
-                    raise ValueError('Strange notehead {0} vs. leger line {1}'
-                                     ' situation: bbox notehead {2}, LL {3}'
-                                     ''.format(notehead.id, closest_ll.id,
-                                               notehead.bounding_box,
-                                               closest_ll.bounding_box))
-
-            delta = (2 * n_lls - 1) + 5
-            if not on_leger_line:
-                delta += 1
-
-            if not is_above_staff:
-                delta *= -1
-
-            return delta
-
-        elif len(staffline_objects) == 1:
-            current_staffline = staffline_objects[0]
-
-            # Count how far from the current staffline we are.
-            #  - Collect staffline objects from the current staff
-            all_staffline_objects = self.__children(current_staff,
-                                                    _CONST.STAFFLINE_CLASS_NAMES)
-
-            #  - Determine their ordering, top to bottom
-            sorted_staffline_objects = sorted(all_staffline_objects,
-                                              key=lambda x: (x.top + x.bottom) / 2.)
-
-            delta = None
-            for i, s in enumerate(sorted_staffline_objects):
-                if s.id == current_staffline.id:
-                    delta = 5 - i
-
-            if delta is None:
-                raise ValueError('Notehead {0} attached to staffline {1},'
-                                 ' which is however not a child of'
-                                 ' the notehead\'s staff {2}!'
-                                 ''.format(notehead.id, current_staffline.id,
-                                           current_staff.id))
-
-            return delta
-
-        else:
-            raise ValueError('Notehead {0} attached to more than one'
-                             ' staffline/staffspace!'.format(notehead.id))
-
-    def process_measure_separator(self, measure_separator):
-        self.pitch_state.reset_inline_accidentals()
-
-    def process_key_signature(self, key_signature):
-        sharps = self.__children(key_signature, ['sharp'])
-        flats = self.__children(key_signature, ['flat'])
-        self.pitch_state.set_key(len(sharps), len(flats))
-
-    def process_clef(self, clef):
-        # Check for staffline children
-        stafflines = self.__children(clef, class_names=_CONST.STAFFLINE_CLASS_NAMES)
-        if len(stafflines) == 0:
-            logging.info('Clef not connected to any staffline, assuming default'
-                         ' position: {0}'.format(clef.id))
-            self.pitch_state.init_base_pitch(clef=clef)
-        else:
-            # Compute clef staffline delta from middle staffline.
-            delta = self.staffline_delta(clef)
-            logging.info('Clef {0}: computed staffline delta {1}'
-                         ''.format(clef.id, delta))
-            self.pitch_state.init_base_pitch(clef=clef, delta=delta)
-
-    def _collect_symbols_for_pitch_inference(self, nodes: List[Node],
-                                             ignore_nonstaff=True):
-        """Extract all symbols from the document relevant for pitch
-        inference and index them in the Engine's temp data structures."""
-        graph = NotationGraph(nodes)
-
-        # Collect staves.
-        self.staves = [c for c in nodes if c.class_name == 'staff']
-        logging.info('We have {0} staves.'.format(len(self.staves)))
-
-        # Collect clefs and key signatures per staff.
-        self.clefs = [c for c in nodes
-                      if c.class_name in _CONST.CLEF_CLASS_NAMES]
-        if ignore_nonstaff:
-            self.clefs = [c for c in self.clefs if graph.has_children(c, ['staff'])]
-
-        self.key_signatures = [c for c in nodes
-                               if c.class_name == 'key_signature']
-        if ignore_nonstaff:
-            self.key_signatures = [c for c in self.key_signatures
-                                   if graph.has_children(c, ['staff'])]
-
-        self.clef_to_staff_map = {}
-        # There may be more than one clef per staff.
-        self.staff_to_clef_map = collections.defaultdict(list)
-        for c in self.clefs:
-            # Assuming one staff per clef
-            try:
-                s = self.__children(c, ['staff'])[0]
-            except (KeyError, ValueError):
-                logging.warning('Clef {0} has no staff attached! Will not be'
-                                ' part of pitch inference.'.format(c.id))
-                continue
-            self.clef_to_staff_map[c.id] = s
-            self.staff_to_clef_map[s.id].append(c)
-
-        self.key_to_staff_map = {}
-        # There may be more than one key signature per staff.
-        self.staff_to_key_map = collections.defaultdict(list)
-        for k in self.key_signatures:
-            try:
-                s = self.__children(k, ['staff'])[0]
-            except KeyError:
-                logging.warning('Key signature {0} has no staff attached! Will not be'
-                                ' part of pitch inference.'.format(k.id))
-                continue
-            self.key_to_staff_map[k.id] = s
-            self.staff_to_key_map[s.id].append(k)
-
-        # Collect measure separators.
-        self.measure_separators = [c for c in nodes
-                                   if c.class_name == 'measure_separator']
-        if ignore_nonstaff:
-            self.measure_separators = [c for c in self.measure_separators
-                                       if graph.has_children(c, ['staff'])]
-
-        self.staff_to_msep_map = collections.defaultdict(list)
-        for m in self.measure_separators:
-            _m_staves = self.__children(m, ['staff'])
-            # (Measure separators might belong to multiple staves.)
-            for s in _m_staves:
-                self.staff_to_msep_map[s.id].append(m)
-                # Collect accidentals per notehead.
-
-        # Collect noteheads.
-        self.noteheads = [c for c in nodes
-                          if c.class_name in _CONST.NOTEHEAD_CLASS_NAMES]
-        if ignore_nonstaff:
-            self.noteheads = [c for c in self.noteheads
-                              if graph.has_children(c, ['staff'])]
-
-        self.staff_to_noteheads_map = collections.defaultdict(list)
-        for n in self.noteheads:
-            s = self.__children(n, ['staff'])[0]
-            self.staff_to_noteheads_map[s.id].append(n)
-
-    def __children(self, c: Node, class_names: List[str]) -> List[Node]:
-        """Retrieve the children of the given Node ``c``
-        that have class in ``clsnames``."""
-        return [self.id_to_node_mapping[o] for o in c.outlinks
-                if self.id_to_node_mapping[o].class_name in class_names]
-
-    def __parents(self, c: Node, class_names: List[str]) -> List[Node]:
-        """Retrieve the parents of the given Node ``c``
-        that have class in ``clsnames``."""
-        return [self.id_to_node_mapping[i] for i in c.inlinks
-                if self.id_to_node_mapping[i].class_name in class_names]
-
-    def __warning_or_error(self, message):
-        if self.strategy.permissive:
-            logging.warning(message)
-        else:
-            raise ValueError(message)
-
-
-class OnsetsInferenceEngine(object):
-
-    def __init__(self, nodes: List[Node], strategy=OnsetsInferenceStrategy()):
-        """Initialize the onset inference engine with the full Node
-        list in a document."""
-        self.id_to_node_mapping = {c.id: c for c in nodes}
-
-        self.strategy = strategy
-
-    def durations(self, nodes: List[Node], ignore_modifiers: bool = False) -> Dict[int, float]:
-        """Returns a dict that contains the durations (in beats)
-        of all Nodes that should be associated with a duration.
-        The dict keys are ``id``.
-
-        :param ignore_modifiers: If set, will ignore duration dots,
-            tuples, and other potential duration modifiers when computing
-            the durations. Effectively, this gives you classes that
-            correspond to note(head) type: whole (4.0), half (2.0),
-            quarter (1.0), eighth (0.5), etc.
-        """
-        # Generate & return the durations dictionary.
-        _relevant_clsnames = _CONST.classes_bearing_duration
-        duration_nodes = [c for c in nodes
-                          if c.class_name in _relevant_clsnames]
-
-        durations = {c.id: self.beats(c, ignore_modifiers=ignore_modifiers)
-                     for c in duration_nodes}
-        return durations
-
-    def beats(self, node: Node, ignore_modifiers=False):
-        if node.class_name in _CONST.NOTEHEAD_CLASS_NAMES:
-            return self.notehead_beats(node,
-                                       ignore_modifiers=ignore_modifiers)
-        elif node.class_name in _CONST.REST_CLASS_NAMES:
-            return self.rest_beats(node,
-                                   ignore_modifiers=ignore_modifiers)
-        else:
-            raise ValueError('Cannot compute beats for object {0} of class {1};'
-                             ' beats only available for notes and rests.'
-                             ''.format(node.id, node.class_name))
-
-    def notehead_beats(self, notehead, ignore_modifiers=False) -> float:
-        """Retrieves the duration for the given notehead, in beats.
-
-        It is possible that the notehead has two stems.
-        In that case, we return all the possible durations:
-        usually at most two, but if there is a duration dot, then
-        there can be up to 4 possibilities.
-
-        Grace notes currently return 0 beats.
-
-        :param ignore_modifiers: If given, will ignore all duration
-            modifiers: Duration dots, tuples, and other potential duration
-            modifiers when computing the durations. Effectively, this
-            gives you classes that correspond to note(head) type:
-            whole (4.0), half (2.0), quarter (1.0), eighth (0.5), etc.
-
-        :returns: A list of possible durations for the given notehead.
-            Mostly its length is just 1; for multi-stem noteheads,
-            you might get more.
-        """
-        beat = [0]
-
-        stems = self.__children(notehead, ['stem'])
-        flags_and_beams = self.__children(
-            notehead,
-            _CONST.FLAGS_AND_BEAMS)
-
-        if notehead.class_name.startswith('grace-notehead'):
-            logging.warning('Notehead {0}: Grace notes get zero duration!'
-                            ''.format(notehead.id))
-            beat = [0]
-
-        elif len(stems) > 1:
-            logging.warning('Inferring duration for multi-stem notehead: {0}'
-                            ''.format(notehead.id))
-            beat = self.process_multistem_notehead(notehead)
-            if len(beat) > 1:
-                self.__warning_or_error('Cannot deal with multi-stem notehead'
-                                        ' where multiple durations apply.')
-                beat = [max(beat)]
-
-        elif notehead.class_name == 'notehead-empty':
-            if len(flags_and_beams) != 0:
-                raise ValueError('Notehead {0} is empty, but has {1} flags and beams!'
-                                 ''.format(notehead.id))
-
-            if len(stems) == 0:
-                beat = [4]
-            else:
-                beat = [2]
-
-        elif notehead.class_name == 'noteheadFull':
-            if len(stems) == 0:
-                self.__warning_or_error('Full notehead {0} has no stem!'.format(notehead.id))
-
-            beat = [0.5 ** len(flags_and_beams)]
-
-        else:
-            raise ValueError('Notehead {0}: unknown class_name {1}'
-                             ''.format(notehead.id, notehead.class_name))
-
-        if not ignore_modifiers:
-            duration_modifier = self.compute_duration_modifier(notehead)
-            beat = [b * duration_modifier for b in beat]
-
-        if len(beat) > 1:
-            logging.warning('Notehead {0}: more than 1 duration: {1}, choosing first'
-                            ''.format(notehead.id, beat))
-        return beat[0]
-
-    def compute_duration_modifier(self, notehead: Node):
-        """Computes the duration modifier (multiplicative, in beats)
-        for the given notehead (or rest) from the tuples and duration dots.
-
-        Can handle duration dots within tuples.
-
-        Cannot handle nested/multiple tuples.
-        """
-        duration_modifier = 1
-        # Dealing with tuples:
-        tuples = self.__children(notehead, ['tuple'])
-        if len(tuples) > 1:
-            raise ValueError('Notehead {0}: Cannot deal with more than one tuple'
-                             ' simultaneously.'.format(notehead.id))
-        if len(tuples) == 1:
-            tuple = tuples[0]
-
-            # Find the number in the tuple.
-            numerals = sorted([self.id_to_node_mapping[o] for o in tuple.outlinks
-                               if self.id_to_node_mapping[o].class_name.startswith('numeral')],
-                              key=lambda x: x.left)
-            # Concatenate numerals left to right.
-            tuple_number = int(''.join([num.class_name[-1] for num in numerals]))
-
-            # Last note in tuple should get complementary duration
-            # to sum to a whole. Otherwise, playing brings slight trouble.
-
-            if tuple_number == 2:
-                # Duola makes notes *longer*
-                duration_modifier = 3 / 2
-            elif tuple_number == 3:
-                duration_modifier = 2 / 3
-            elif tuple_number == 4:
-                # This one also makes notes longer
-                duration_modifier = 4 / 3
-            elif tuple_number == 5:
-                duration_modifier = 4 / 5
-            elif tuple_number == 6:
-                # Most often done for two consecutive triolas,
-                # e.g. 16ths with a 6-tuple filling one beat
-                duration_modifier = 2 / 3
-            elif tuple_number == 7:
-                # Here we get into trouble, because this one
-                # can be both 4 / 7 (7 16th in a beat)
-                # or 8 / 7 (7 32nds in a beat).
-                # In the same vein, we cannot resolve higher
-                # tuples unless we establish precedence/simultaneity.
-                logging.warning('Cannot really deal with higher tuples than 6.')
-                # For MUSCIMA++ specifically, we can cheat: there is only one
-                # septuple, which consists of 7 x 32rd in 1 beat, so they
-                # get 8 / 7.
-                logging.warning('MUSCIMA++ cheat: we know there is only 7 x 32rd in 1 beat'
-                                ' in page 14.')
-                duration_modifier = 8 / 7
-            elif tuple_number == 10:
-                logging.warning('MUSCIMA++ cheat: we know there is only 10 x 32rd in 1 beat'
-                                ' in page 04.')
-                duration_modifier = 4 / 5
-            else:
-                raise NotImplementedError('Notehead {0}: Cannot deal with tuple '
-                                          'number {1}'.format(notehead.id,
-                                                              tuple_number))
-
-        # Duration dots
-        ddots = self.__children(notehead, ['duration-dot'])
-        dot_duration_modifier = 1
-        for i, d in enumerate(ddots):
-            dot_duration_modifier += 1 / (2 ** (i + 1))
-        duration_modifier *= dot_duration_modifier
-
-        return duration_modifier
-
-    def rest_beats(self, rest: Node, ignore_modifiers=False) -> float:
-        """Compute the duration of the given rest in beats.
-
-        :param ignore_modifiers: If given, will ignore all duration
-            modifiers: Duration dots, tuples, and other potential duration
-            modifiers when computing the durations. Effectively, this
-            gives you classes that correspond to note(head) type:
-            whole (4.0), half (2.0), quarter (1.0), eighth (0.5), etc.
-            Also ignores deriving duration from the time signature
-            for whole rests.
-
-        """
-        rest_beats_dict = {'whole_rest': 4,  # !!! We should find the Time Signature.
-                           'half_rest': 2,
-                           'quarter_rest': 1,
-                           '8th_rest': 0.5,
-                           '16th_rest': 0.25,
-                           '32th_rest': 0.125,
-                           '64th_and_higher_rest': 0.0625,
-                           # Technically, these two should just apply time sig.,
-                           # but the measure-factorized precedence graph
-                           # means these durations never have sounding
-                           # descendants anyway:
-                           'multi-measure_rest': 4,
-                           'repeat-measure': 4,
-                           }
-
-        try:
-            base_rest_duration = rest_beats_dict[rest.class_name]
-
-        except KeyError:
-            raise KeyError('Symbol {0}: Unknown rest type {1}!'
-                           ''.format(rest.id, rest.class_name))
-
-        # Process the whole rest:
-        #  - if it is the only symbol in the measure, it should take on
-        #    the duration of the current time signature.
-        #  - if it is not the only symbol in the measure, it takes 4 beats
-        #  - Theoretically, it could perhaps take e.g. 6 beats in weird situations
-        #    in a 6/2 time signature, but we don't care about this for now.
-        #
-        # If there is no leftward time signature, we need to infer the time
-        # sig from the other symbols. This necessitates two-pass processing:
-        # first get all available durations, then guess the time signatures
-        # (technically this might also be needed for each measure).
-        if (rest.class_name in _CONST.MEAUSURE_LASTING_CLASS_NAMES) and not ignore_modifiers:
-            base_rest_duration = self.measure_lasting_beats(rest)
-            beat = [base_rest_duration]  # Measure duration should never be ambiguous.
-
-        elif not ignore_modifiers:
-            duration_modifier = self.compute_duration_modifier(rest)
-            beat = [base_rest_duration * duration_modifier]
-
-        else:
-            beat = [base_rest_duration]
-
-        if len(beat) > 1:
-            logging.warning('Rest {0}: more than 1 duration: {1}, choosing first'
-                            ''.format(rest.id, beat))
-        return beat[0]
-
-    def measure_lasting_beats(self, node: Node):
-        """Find the duration of an object that lasts for an entire measure
-        by interpreting the time signature valid for the given point in
-        the score.
-
-        If any assumption is broken, will return the default measure duration:
-        4 beats."""
-        # Find rightmost preceding time signature on the staff.
-        graph = NotationGraph(list(self.id_to_node_mapping.values()))
-
-        # Find current time signature
-        staffs = graph.children(node, class_filter=[_CONST.STAFF_CLASS_NAME])
-
-        if len(staffs) == 0:
-            logging.warning('Interpreting object {0} as measure-lasting, but'
-                            ' it is not attached to any staff! Returning default: 4'
-                            ''.format(node.id))
-            return 4
-
-        if len(staffs) > 1:
-            logging.warning('Interpreting object {0} as measure-lasting, but'
-                            ' it is connected to more than 1 staff: {1}'
-                            ' Returning default: 4'
-                            ''.format(node.id, [s.id for s in staffs]))
-            return 4
-
-        logging.info('Found staffs: {0}'.format([s.id for s in staffs]))
-
-        staff = staffs[0]
-        time_signatures = graph.ancestors(staff, class_filter=_CONST.TIME_SIGNATURES)
-
-        logging.info('Time signatures: {0}'.format([t.id for t in time_signatures]))
-
-        applicable_time_signatures = sorted([t for t in time_signatures
-                                             if t.left < node.left],
-                                            key=operator.attrgetter('left'))
-        logging.info('Applicable time signatures: {0}'.format([t.id for t in time_signatures]))
-
-        if len(applicable_time_signatures) == 0:
-            logging.warning('Interpreting object {0} as measure-lasting, but'
-                            ' there is no applicable time signature. Returnig'
-                            ' default: 4'.format(node.id))
-            return 4
-
-        valid_time_signature = applicable_time_signatures[-1]
-        beats = self.interpret_time_signature(valid_time_signature)
-        return beats
-
-    def process_multistem_notehead(self, notehead):
-        """Attempts to recover the duration options of a multi-stem note."""
-        stems = self.__children(notehead, ['stem'])
-        flags_and_beams = self.__children(
-            notehead,
-            _CONST.FLAGS_AND_BEAMS)
-
-        if len(flags_and_beams) == 0:
-            if notehead.class_name == 'noteheadFull':
-                return [1]
-            elif notehead.class_name == 'notehead-empty':
-                return [2]
-
-        if notehead.class_name == 'notehead-empty':
-            raise NotationGraphError('Empty notehead with flags and beams: {0}'
-                                     ''.format(notehead.id))
-
-        n_avg_x = notehead.top + (notehead.bottom - notehead.top) / 2.0
-        print('Notehead {0}: avg_x = {1}'.format(notehead.id, n_avg_x))
-        f_and_b_above = []
-        f_and_b_below = []
-        for c in flags_and_beams:
-            c_avg_x = c.top + (c.bottom - c.top) / 2.0
-            print('Beam/flag {0}: avg_x = {1}'.format(c.id, c_avg_x))
-            if c_avg_x < n_avg_x:
-                f_and_b_above.append(c)
-                print('Appending above')
-            else:
-                f_and_b_below.append(c)
-                print('Appending below')
-
-        beat_above = 0.5 ** len(f_and_b_above)
-        beat_below = 0.5 ** len(f_and_b_below)
-
-        if beat_above != beat_below:
-            raise NotImplementedError('Cannot deal with multi-stem note'
-                                      ' that has different pre-modification'
-                                      ' durations: {0} vs {1}'
-                                      '{2}'.format(beat_above, beat_below, notehead.id))
-
-        beat = [beat_above]
-
-        tuples = self.__children(notehead, ['tuple'])
-        if len(tuples) % 2 != 0:
-            raise NotImplementedError('Cannot deal with multi-stem note'
-                                      ' that has an uneven number of tuples:'
-                                      ' {0}'.format(notehead.id))
-
-        duration_modifier = self.compute_duration_modifier(notehead)
-        beat = [b * duration_modifier for b in beat]
-
-        return beat
-
-    ##########################################################################
-    # Onsets inference
-    def infer_precedence_from_annotations(self, nodes: List[Node]):
-        """Infer precedence graph based solely on the "green lines"
-        in MUSCIMA++ annotation: precedence edges. These are encoded
-        in the data as inlink/outlink lists
-        in ``Node.data['precedence_inlinks']``,
-        and ``Node.data['precedence_outlinks']``.
-
-        :param nodes: A list of Nodes, not necessarily
-            only those that participate in the precedence graph.
-
-        :return: The list of source nodes of the precedence graph.
-        """
-        _relevant_clsnames = _CONST.classes_bearing_duration
-        precedence_nodes = [c for c in nodes
-                         if c.class_name in _relevant_clsnames]
-
-        if self.strategy.precedence_only_for_objects_connected_to_staff:
-            precedence_nodes = [c for c in precedence_nodes
-                             if len(self.__children(c, ['staff'])) > 0]
-
-        durations = {c.id: self.beats(c) for c in precedence_nodes}
-
-        precedence_nodes = {}
-        for c in precedence_nodes:
-            p_node = PrecedenceGraphNode(objid=c.id,
-                                         node=c,
-                                         inlinks=[],
-                                         outlinks=[],
-                                         duration=durations[c.id],
-                                         )
-            precedence_nodes[c.id] = p_node
-
-        for c in precedence_nodes:
-            inlinks = []
-            outlinks = []
-            if 'precedence_inlinks' in c.data:
-                inlinks = c.data['precedence_inlinks']
-            if 'precedence_outlinks' in c.data:
-                outlinks = c.data['precedence_outlinks']
-            p_node = precedence_nodes[c.id]
-            p_node.outlinks = [precedence_nodes[o] for o in outlinks]
-            p_node.inlinks = [precedence_nodes[i] for i in inlinks]
-
-        # Join staves/systems!
-
-        # ...systems:
-        systems = group_staffs_into_systems(nodes,
-                                            use_fallback_measure_separators=True)
-
-        if len(systems) == 1:
-            logging.info('Single-system score, no staff chaining needed.')
-            source_nodes = [n for n in list(precedence_nodes.values()) if len(n.inlinks) == 0]
-            return source_nodes
-
-        # Check all systems same no. of staffs
-        _system_lengths = [len(s) for s in systems]
-        if len(set(_system_lengths)) > 1:
-            raise ValueError('Cannot deal with variable number of staffs'
-                             ' w.r.t. systems! Systems: {0}'.format(systems))
-
-        staff_chains = [[] for _ in systems[0]]
-        for system in systems:
-            for i, staff in enumerate(system):
-                staff_chains[i].append(staff)
-
-        # Now, join the last --> first nodes within chains.
-        # - Assign objects to staffs
-        objid2staff = {}
-        for c in nodes:
-            staffs = self.__children(c, ['staff'])
-            if len(staffs) == 1:
-                objid2staff[c.id] = staffs[0].id
-
-        # - Assign staffs to sink nodes
-        sink_nodes2staff = {}
-        staff2sink_nodes = collections.defaultdict(list)
-        for node in list(precedence_nodes.values()):
-            if len(node.outlinks) == 0:
-                try:
-                    staff = self.__children(node.obj, ['staff'])[0]
-                except IndexError:
-                    logging.error('Object {0} is a sink node in the precedence graph, but has no staff!'
-                                  ''.format(node.obj.id))
-                    raise
-                sink_nodes2staff[node.obj.id] = staff.id
-                staff2sink_nodes[staff.id].append(node)
-
-        # Note that this means you should never have a sink node
-        # unless it's at the end of the staff. All notes have to lead
-        # somewhere. This is suboptimal; we should filter out non-maximal
-        # sink nodes. But since we do not know whether the sink nodes
-        # are maximal until we are done inferring onsets, we have to stick
-        # with this.
-        # The alternative is to only connect to the next staff the *rightmost*
-        # sink node. This risks *not* failing if the sink nodes of a staff
-        # are not synchronized properly.
-
-        # - Assign staffs to source nodes
-        source_nodes2staff = {}
-        staff2source_nodes = collections.defaultdict(list)
-        for node in list(precedence_nodes.values()):
-            if len(node.inlinks) == 0:
-                staff = self.__children(node.obj, ['staff'])[0]
-                source_nodes2staff[node.obj.id] = staff.id
-                staff2source_nodes[staff.id].append(node)
-
-        # - For each staff chain, link the sink nodes of the prev
-        #   to the source nodes of the next staff.
-        for staff_chain in staff_chains:
-            staffs = sorted(staff_chain, key=lambda x: x.top)
-            for (s1, s2) in zip(staffs[:-1], staffs[1:]):
-                sinks = staff2sink_nodes[s1.id]
-                sources = staff2source_nodes[s2.id]
-                for sink in sinks:
-                    for source in sources:
-                        sink.outlinks.append(source)
-                        source.inlinks.append(sink)
-
-        source_nodes = [n for n in list(precedence_nodes.values()) if len(n.inlinks) == 0]
-        return source_nodes
-
-    def infer_precedence(self, nodes: List[Node]):
-        """This is the most complex part of onset computation.
-
-        The output of this method is a **precedence graph**. The precedence
-        graph is a Directed Acyclic Graph (DAG) consisting of
-        :class:`PrecedenceGraphNode` objects. Each node represents some
-        musical concept that participates in establishing the onsets
-        by having a *duration*. The invariant of the graph is that
-        the onset of a node is the sum of the durations on each of its
-        predecessor paths to a root node (which has onset 0).
-
-        Not all nodes necessarily have nonzero duration (although these
-        nodes can technically be factored out).
-
-        Once the precedence graph is formed, then a breadth-first search
-        (rather than DFS, to more easily spot/resolve conflicts at multi-source
-        precedence graph nodes) simply accumulates durations.
-        Conflicts can be resolved through failing (currently implemented),
-        or looking up possible errors in assigning durations and attempting
-        to fix them.
-
-        Forming the precedence graph itself is difficult, because
-        of polyphonic (and especially pianoform) music. Practically the only
-        actual constraint followed throughout music is that *within a voice*
-        notes are read left-to-right. The practice of aligning e.g. whole
-        notes in an outer voice to the beginning of the bar rather than
-        to the middle took over only cca. 1800 or later.
-
-        An imperfect but overwhelmingly valid constraint is that notes taking
-        up a certain proportion of the measure are not written to the *right*
-        of the proportional horizontal span in the measure corresponding
-        to their duration in time. However, this is *not* uniform across
-        the measure: e.g., if the first voice is 2-8-8-8-8 and the second
-        is 2-2, then the first half can be very narrow and the second
-        quite wide, with the second lower-voice half-note in the middle
-        of that part. However, the *first* lower-voice half-note will
-        at least *not* be positioned in the horizontal span where
-        the 8th notes in the upper voice are.
-
-        Which Nodes participate in the precedence graph?
-        ------------------------------------------------------
-
-        We directly derive precedence graph nodes from the following
-        Nodes:
-
-        * Noteheads: empty, full, and grace noteheads of both kinds, which
-          are assigned duration based on their type (e.g., quarter, 16th, etc.)
-          and then may be further modified by duration dots and/or tuples.
-        * Rests of all kinds, which get duration via a simple table based
-          on the rest class and tuple/dot modification.
-        * Measure separators, which get a duration of 0.
-
-        The assumption of our symbol classes is that there are no rests
-        shorter than 64th.
-
-        Furthermore, we add synthetic nodes representing:
-
-        * Root measure separator, with duration 0 **and** onset 0,
-          which initializes the onset computations along the graph
-        * Measure nodes, with durations derived from time signatures
-          valid for the given measures.
-
-        Constructing the precedence graph
-        ---------------------------------
-
-        We factor the precedence graph into measures, and then infer precedence
-        for each measure separately, in order to keep the problem tractable
-        and in order for errors not to propagate too far. The inference
-        graph construction algorithm is therefore split into two steps:
-
-        * Construct the "spine" of the precedence graph from measure nodes,
-        * Construct the single-measure precedence subgraphs (further factored
-          by staff).
-
-        The difficulties lie primarily in step 2.
-
-        (Note that ties are currently disregarded: the second note
-        of the tie normally gets an onset. After all, conceptually,
-        it is a separate note with an onset, it just does not get played.)
-
-        Precedence graph spine
-        ^^^^^^^^^^^^^^^^^^^^^^
-
-        The **spine** of the precedence graph is a single path of alternating
-        ``measure_separator`` and ``measure`` nodes. ``measure_separator``
-        nodes are constructed from the Nodes, and ``measure`` nodes
-        are created artificially between consecutive ``measure_separator``
-        nodes. The measure separator nodes have a duration of 0, while
-        the duration of the measure nodes is inferred from the time signature
-        valid for that measure. An artificial root measure_separator node
-        is created to serve as the source of the entire precedence graph.
-
-        Thus, the first part of the algorithm is, at a high level:
-
-        * Order measure separators,
-        * Assign time signatures to measures and compute measure durations
-          from time signatures.
-
-        **Gory details:** In step 1, we assume that systems are ordered
-        top-down in time, that all systems are properly grouped using
-        ``staff_grouping`` symbols, that measure separators are strictly
-        monotonous (i.e., the same subset of possible onsets belongs to
-        the i-th measure on each staff, which is an assumption that does
-        *not* hold for isorhythmic motets and basically anything pre-16th
-        century).
-
-        In step 2, we assume that time signatures are always written within
-        the measure that *precedes* the first measure for which they are
-        valid, with the exception of the first time signature on the system.
-
-        We also currently assume that a given measure has the same number
-        of beats across all staves within a system (so: no polytempi for now).
-
-        Measure subgraphs
-        ^^^^^^^^^^^^^^^^^
-
-        There are again two high-level steps:
-
-        * Assign other onset-carrying objects (noteheads and rests)
-          to measures, to prepare the second phase that iterates over
-          these groups per measure (and staff).
-        * For each measure group, compute the subgraph and attach
-          its sources to the preceding measure separator node.
-
-        The first one can be resolved easily by looking at (a) staff
-        assignment, (b) horizontal position with respect to measure
-        separators. Noting that long measure separators might not
-        really be straight, we use the intersection of the separator
-        with the given staff.
-
-        The second step is the difficult one. We describe the algorithm
-        for inferring precedence, simultaneity span minimization,
-        in a separate section.
-
-
-        Simultaneity span minimization
-        ------------------------------
-
-        Inferring precedence in polyphonic music is non-trivial, especially
-        if one wants to handle handwritten music, and even more so when
-        extending the scope before the 1800s. We infer precedence using
-        the principle that notes which are supposed to be played together
-        should be as close to each other horizontally as possible: from
-        all the possible precedence assignments that fulfill notation
-        rule constraints, choose the one which minimizes the horizontal
-        span assigned to each unit of musical time in the bar.
-
-        The algorithm is initialized as follows:
-
-        * Determine the shortest subdivision of the measure (in beats)
-          which has to be treated independently. This generally corresponds
-          to the shortest note in the measure.
-        * Initialize the assignment table: for each onset-carrying object,
-          we will assign it to one of the time bins.
-
-        There are some rules of music notation that we use to prune the space
-        of possible precedence assignments by associating the notes (or rests)
-        into blocks:
-
-        * Beamed groups without intervening rests
-        * Tied note pairs
-        * Notes that share a stem
-        * Notes within a tuple
-
-        Rests within beamed groups (e.g., 8th - 8th_rest - 8th) are a problem.
-        A decision needs to be made whether the rest does belong to the group
-        or not.
-
-        """
-
-        if not self.measure_separators:
-            self._collect_symbols_for_pitch_inference(nodes)
-
-        measure_separators = [c for c in nodes
-                              if c.class_name in _CONST.MEASURE_SEPARATOR_CLASS_NAMES]
-
-        ######################################################################
-        # An important feature of measure-factorized onset inference
-        # instead of going left-to-right per part throughout is resistance
-        # to staves appearing & disappearing on line breaks (e.g. orchestral
-        # scores). Measures are (very, very often) points of synchronization
-        #  -- after all, that is their purpose.
-
-        # We currently DO NOT aim to process renaissance & medieval scores:
-        # especially motets may often have de-synchronized measure separators.
-
-        # Add the relationships between the measure separator nodes.
-        #  - Get staves to which the mseps are connected
-        msep_staffs = {m.id: self.__children(m, ['staff'])
-                       for m in measure_separators}
-        #  - Sort first by bottom-most staff to which the msep is connected
-        #    to get systems
-        #  - Sort left-to-right within systems to get final ordering of mseps
-        ordered_mseps = sorted(measure_separators,
-                               key=lambda m: (max([s.bottom
-                                                   for s in msep_staffs[m.id]]),
-                                              m.left))
-        ordered_msep_nodes = [PrecedenceGraphNode(node=m,
-                                                  inlinks=[],
-                                                  outlinks=[],
-                                                  onset=None,
-                                                  duration=0)
-                              for m in ordered_mseps]
-
-        # Add root node: like measure separator, but for the first measure.
-        # This one is the only one which is initialized with onset,
-        # with the value onset=0.
-        root_msep = PrecedenceGraphNode(objid=-1,
-                                        node=None,
-                                        inlinks=[], outlinks=[],
-                                        duration=0,
-                                        onset=0)
-
-        # Create measure bins. i-th measure ENDS at i-th ordered msep.
-        # We assume that every measure has a rightward separator.
-        measures = [(None, ordered_mseps[0])] + [(ordered_mseps[i], ordered_mseps[i + 1])
-                                                 for i in range(len(ordered_mseps) - 1)]
-        measure_nodes = [PrecedenceGraphNode(objid=None,
-                                             node=None,
-                                             inlinks=[root_msep],
-                                             outlinks=[ordered_msep_nodes[0]],
-                                             duration=0,  # Durations will be filled in
-                                             onset=None)] + \
-                        [PrecedenceGraphNode(objid=None,
-                                             node=None,
-                                             inlinks=[ordered_msep_nodes[i + 1]],
-                                             outlinks=[ordered_msep_nodes[i + 2]],
-                                             duration=0,  # Durations will be filled in
-                                             onset=None)
-                         for i in range(len(ordered_msep_nodes) - 2)]
-        #: A list of PrecedenceGraph nodes. These don't really need any Node
-        #  or id, they are just introducing through their duration the offsets
-        #  between measure separators (mseps have legit 0 duration, so that they
-        #  do not move the notes in their note descendants).
-        #  The list is already ordered.
-
-        # Add measure separator inlinks and outlinks.
-        for m_node in measure_nodes:
-            r_sep = m_node.outlinks[0]
-            r_sep.inliks.append(m_node)
-            if len(m_node.inlinks) > 0:
-                l_sep = m_node.inlinks[0]
-                l_sep.outlinks.append(m_node)
-
-        # Finally, hang the first measure on the root msep node.
-        root_msep.outlinks.append(measure_nodes[0])
-
-        ######################################################################
-        # Now, compute measure node durations from time signatures.
-        #  This is slightly non-trivial. Normally, a time signature is
-        #  (a) at the start of the staff, (b) right before the msep starting
-        #  the measure to which it should apply. However, sometimes the msep
-        #  comes up (c) at the *start* of the measure to which it should
-        #  apply. We IGNORE option (c) for now.
-        #
-        #  - Collect all time signatures
-        time_signatures = [c for c in nodes
-                           if c.class_name in _CONST.TIME_SIGNATURES]
-
-        #  - Assign time signatures to measure separators that *end*
-        #    the bars. (Because as opposed to the starting mseps,
-        #    the end mseps are (a) always there, (b) usually on the
-        #    same staff, (c) if not on the same staff, then they are
-        #    an anticipation at the end of a system, and will be repeated
-        #    at the beginning of the next one anyway.)
-        time_signatures_to_first_measure = {}
-        for t in time_signatures:
-            s = self.__children(t, ['staff'])[0]
-            # - Find the measure pairs
-            for i, (left_msep, right_msep) in enumerate(measures):
-                if s not in msep_staffs[right_msep.id]:
-                    continue
-                if (left_msep is None) or (s not in msep_staffs[left_msep.id]):
-                    # Beginning of system, valid already for the current bar.
-                    time_signatures_to_first_measure[t.id] = i
-                else:
-                    # Use i + 1, because the time signature is valid
-                    # for the *next* measure.
-                    time_signatures_to_first_measure[t.id] = i + 1
-
-        # - Interpret time signatures.
-        time_signature_durations = {t.id: self.interpret_time_signature(t)
-                                    for t in time_signatures}
-
-        # - Reverse map: for each measure, the time signature valid
-        #   for the measure.
-        measure_to_time_signature = [None for _ in measures]
-        time_signatures_sorted = sorted(time_signatures,
-                                        key=lambda x: time_signatures_to_first_measure[x.id])
-        for t1, t2 in zip(time_signatures_sorted[:-1], time_signatures_sorted[1:]):
-            affected_measures = list(range(time_signatures_to_first_measure[t1.id],
-                                           time_signatures_to_first_measure[t2.id]))
-            for i in affected_measures:
-                # Check for conflicting time signatures previously
-                # assigned to this measure.
-                if measure_to_time_signature[i] is not None:
-                    _competing_time_sig = measure_to_time_signature[i]
-                    if (time_signature_durations[t1.id] !=
-                            time_signature_durations[_competing_time_sig.id]):
-                        raise ValueError('Trying to overwrite time signature to measure'
-                                         ' assignment at measure {0}: new time sig'
-                                         ' {1} with value {2}, previous time sig {3}'
-                                         ' with value {4}'
-                                         ''.format(i, t1.id,
-                                                   time_signature_durations[t1.id],
-                                                   _competing_time_sig.id,
-                                                   time_signature_durations[_competing_time_sig.id]))
-
-                measure_to_time_signature[i] = t1
-
-        logging.debug('Checking that every measure has a time signature assigned.')
-        for i, (msep1, msep2) in enumerate(measures):
-            if measure_to_time_signature[i] is None:
-                raise ValueError('Measure without time signature: {0}, between'
-                                 'separators {1} and {2}'
-                                 ''.format(i, msep1.id, msep2.id))
-
-        # - Apply to each measure node the duration corresponding
-        #   to its time signature.
-        for i, m in enumerate(measure_nodes):
-            _tsig = measure_to_time_signature[i]
-            m.duration = time_signature_durations[_tsig.id]
-
-        # ...
-        # Now, the "skeleton" of the precedence graph consisting
-        # pf measure separator and measure nodes is complete.
-        ######################################################################
-
-        ######################################################################
-        # Collecting onset-carrying objects (at this point, noteheads
-        # and rests; the repeat-measure object that would normally
-        # affect duration is handled through measure node durations.
-        onset_objs = [c for c in nodes
-                      if c.class_name in _CONST.classes_bearing_duration]
-
-        # Assign onset-carrying objects to measures (their left msep).
-        # (This is *not* done by assigning outlinks to measure nodes,
-        # we are now just factorizing the space of possible precedence
-        # graphs.)
-        #  - This is done by iterating over staves.
-        staff_to_objs_map = collections.defaultdict(list)
-        for c in onset_objs:
-            ss = self.__children(c, ['staff'])
-            for s in ss:
-                staff_to_objs_map[s.id].append(c)
-
-        #  - Noteheads and rests are all connected to staves,
-        #    which immediately gives us for each staff the subset
-        #    of eligible symbols for each measure.
-        #  - We can just take the vertical projection of each onset
-        #    object and find out which measures it overlaps with.
-        #    To speed this up, we can just check whether the middles
-        #    of objects fall to the region delimited by the measure
-        #    separators. Note that sometimes the barlines making up
-        #    the measure separator are heavily bent, so it would
-        #    be prudent to perhaps use just the intersection of
-        #    the given barline and the current staff.
-
-        # Preparation: we need for each valid (staff, msep) combination
-        # the bounding box of their intersection, in order to deal with
-        # more curved measure separators.
-
-        msep_to_staff_projections = {}
-        #: For each measure separator, for each staff it connects to,
-        #  the bounding box of the measure separator's intersection with
-        #  that staff.
-        for msep in measure_separators:
-            msep_to_staff_projections[msep.id] = {}
-            for s in msep_staffs[msep.id]:
-                intersection_bbox = self.msep_staff_overlap_bbox(msep, s)
-                msep_to_staff_projections[msep.id][s.id] = intersection_bbox
-
-        staff_and_measure_to_objs_map = collections.defaultdict(
-            collections.defaultdict(list))
-        #: Per staff (indexed by id) and measure (by order no.), keeps a list of
-        #  Nodes from that staff that fall within that measure.
-
-        # Iterate over objects left to right, shift measure if next object
-        # over bound of current measure.
-        ordered_objs_per_staff = {s_objid: sorted(s_objs, key=lambda x: x.left)
-                                  for s_objid, s_objs in list(staff_to_objs_map.items())}
-        for s_objid, objs in list(ordered_objs_per_staff.items()):
-            # Vertically, we don't care -- the attachment to staff takes
-            # care of that, we only need horizontal placement.
-            _c_m_idx = 0  # Index of current measure
-            _c_msep_right = measure_nodes[_c_m_idx].outlinks[0]
-            # Left bound of current measure's right measure separator
-            _c_m_right = msep_to_staff_projections[_c_msep_right.id][s_objid][1]
-            for _c_o_idx, o in objs:
-                # If we are out of bounds, move to next measure
-                while o.left > _c_m_right:
-                    _c_m_idx += 1
-                    if _c_m_idx >= len(measure_nodes):
-                        raise ValueError('Object {0}: could not assign to any measure,'
-                                         ' ran out of measures!'.format(o.id))
-                    _c_msep_right = measure_nodes[_c_m_idx].outlinks[0]
-                    _c_m_right = msep_to_staff_projections[_c_msep_right.id][s_objid][1]
-                    staff_and_measure_to_objs_map[s_objid][_c_m_right] = []
-
-                staff_and_measure_to_objs_map[s_objid][_c_m_right].append(o)
-
-        # Infer precedence within the measure.
-        #  - This is the difficult part.
-        #  - First: check the *sum* of durations assigned to the measure
-        #    against the time signature. If it fits only once, then it is
-        #    a monophonic measure and we can happily read it left to right.
-        #  - If the measure is polyphonic, the fun starts!
-        #    With K graph nodes, how many prec. graphs are there?
-        for s_objid in staff_and_measure_to_objs_map:
-            for measure_idx in staff_and_measure_to_objs_map[s_objid]:
-                _c_objs = staff_and_measure_to_objs_map[s_objid][measure_idx]
-                measure_graph = self.measure_precedence_graph(_c_objs)
-
-                # Connect the measure graph source nodes to their preceding
-                # measure separator.
-                l_msep_node = measure_nodes[measure_idx].inlinks[0]
-                for source_node in measure_graph:
-                    l_msep_node.outlinks.append(source_node)
-                    source_node.inlinks.append(l_msep_node)
-
-        return [root_msep]
-
-    def measure_precedence_graph(self, nodes: List[Node]):
-        """Indexed by staff id and measure number, holds the precedence graph
-        for the given measure in the given staff as a list of PrecedenceGraphNode
-        objects that correspond to the source nodes of the precedence subgraph.
-        These nodes then get connected to their leftwards measure separator node.
-
-        :param nodes: List of Nodes, assumed to be all from one
-            measure.
-
-        :returns: A list of PrecedenceGraphNode objects that correspond
-            to the source nodes in the precedence graph for the (implied)
-            measure. (In monophonic music, the list will have one element.)
-            The rest of the measure precedence graph nodes is accessible
-            through the sources' outlinks.
-
-        """
-        _is_monody = self.is_measure_monody(nodes)
-        if _is_monody:
-            source_nodes = self.monody_measure_precedence_graph(nodes)
-            return source_nodes
-
-        else:
-            raise ValueError('Cannot deal with onsets in polyphonic music yet.')
-
-    def monody_measure_precedence_graph(self, nodes: List[Node]):
-        """Infers the precedence graph for a plain monodic measure.
-        The resulting structure is very simple: it's just a chain
-        of the onset-carrying objects from left to right."""
-        nodes = []
-        for c in sorted(nodes, key=lambda x: x.left):
-            potential_durations = self.beats(c)
-
-            # In monody, there should only be one duration
-            if len(potential_durations) > 1:
-                raise ValueError('Object {0}: More than one potential'
-                                 ' duration, even though the measure is'
-                                 ' determined to be monody.'.format(c.id))
-            duration = potential_durations[0]
-
-            node = PrecedenceGraphNode(objid=c.id,
-                                       node=c,
-                                       inlinks=[],
-                                       outlinks=[],
-                                       duration=duration,
-                                       onset=None)
-            nodes.append(node)
-        for n1, n2 in zip(nodes[:-1], nodes[1:]):
-            n1.outlinks.append(n2)
-            n2.inlinks.append(n1)
-        source_nodes = [nodes[0]]
-        return source_nodes
-
-    def is_measure_monody(self, nodes: List[Node]):
-        """Checks whether the given measure is written as simple monody:
-        no two of the onset-carrying objects are active simultaneously.
-
-        Assumptions
-        -----------
-
-        * Detecting monody without looking at the time signature:
-            * All stems in the same direction? --> NOPE: Violin chords in Bach...
-            * All stems in horizontally overlapping noteheads in the same direction?
-              --> NOPE: Again, violin chords in Bach...
-            * Overlapping noteheads share a beam, but not a stem? --> this works,
-              but has false negatives: overlapping quarter notes
-        """
-        raise NotImplementedError()
-
-    def is_measure_chord_monody(self, nodes: List[Node]):
-        """Checks whether the given measure is written as monody potentially
-        with chords. That is: same as monody, but once all onset-carrying objects
-        that share a stem are merged into an equivalence class."""
-        raise NotImplementedError()
-
-    def msep_staff_overlap_bbox(self, measure_separator, staff):
-        """Computes the bounding box for the part of the input
-        ``measure_separator`` that actually overlaps the ``staff``.
-        This is implemented to deal with mseps that curve a lot,
-        so that their left/right bounding box may mistakenly
-        exclude some symbols from their preceding/following measure.
-
-        Returns the (T, L, B, R) bounding box.
-        """
-        intersection = measure_separator.bounding_box_intersection(staff)
-        if intersection is None:
-            # Corner case: measure separator is connected to staff,
-            # but its bounding box does *not* overlap the bbox
-            # of the staff.
-            output_bbox = staff.top, measure_separator.left, \
-                          staff.bottom, measure_separator.right
-        else:
-            # The key step: instead of using the bounding
-            # box intersection, first crop the zeros from
-            # msep intersection mask (well, find out how
-            # many left and right zeros there are).
-            it, il, ib, ir = intersection
-            msep_crop = measure_separator.mask[it, il, ib, ir]
-
-            if msep_crop.sum() == 0:
-                # Corner case: bounding box does encompass staff,
-                # but there is msep foreground pixel in that area
-                # (could happen e.g. with mseps only drawn *around*
-                # staffs).
-                output_bbox = staff.top, measure_separator.left, \
-                              staff.bottom, measure_separator.right
-            else:
-                # The canonical case: measure separator across the staff.
-                msep_crop_vproj = msep_crop.sum(axis=0)
-                _dl = 0
-                _dr = 0
-                for i, v in enumerate(msep_crop_vproj):
-                    if v != 0:
-                        _dl = i
-                        break
-                for i in range(1, len(msep_crop_vproj)):
-                    if msep_crop_vproj[-i] != 0:
-                        _dr = i
-                        break
-                output_bbox = staff.top, measure_separator.left + _dl, \
-                              staff.bottom, measure_separator.right - _dr
-        return output_bbox
-
-    @staticmethod
-    def interpret_numerals(numerals: List[Node]) -> int:
-        """Returns the given numeral Node as a number, left to right."""
-        for n in numerals:
-            if n.class_name not in _CONST.NUMERALS:
-                raise ValueError('Symbol {0} is not a numeral!'.format(n.id))
-        n_str = ''.join([n.class_name[-1]
-                         for n in sorted(numerals, key=operator.attrgetter('left'))])
-        return int(n_str)
-
-    def interpret_time_signature(self, time_signature,
-                                 FRACTIONAL_VERTICAL_IOU_THRESHOLD=0.8):
-        """Converts the time signature into the beat count (in quarter
-        notes) it assigns to its following measures.
-
-        Dealing with numeric time signatures
-        ------------------------------------
-
-        * Is there both a numerator and a denominator?
-          (Is the time sig. "fractional"?)
-           * If there is a letter_other child, then yes; use the letter_other
-             symbol to separate time signature into numerator (top, left) and
-             denominator regions.
-           * If there is no letter_other child, then check if there is sufficient
-             vertical separation between some groups of symbols. Given that it
-             is much more likely that there will be the "fractional" structure,
-             we say:
-
-               If the minimum vertical IoU between two symbols is more than
-               0.8, we consider the time signature non-fractional.
-
-             (The threshold can be controlled through the
-             FRACTIONAL_VERTICAL_IOU_THRESHOLD parameter.)
-
-        * If yes: assign numerals to either num. (top), or denom. (bottom)
-        * If not: assume the number is no. of beats. (In some scores, the
-          base indicator may be attached in form of a note instead of a
-          denumerator, like e.g. scores by Janacek, but we ignore this for now.
-          In early music, 3 can mean "tripla", which is 3/2.)
-
-        Dealing with non-numeric time signatures
-        ----------------------------------------
-
-        * whole-time mark is interpreted as 4/4
-        * alla breve mark is interpreted as 4/4
-
-
-        :returns: The denoted duration of a measure in beats.
-        """
-        members = sorted(self.__children(time_signature,
-                                         clsnames=_CONST.TIME_SIGNATURE_MEMBERS),
-                         key=lambda x: x.top)
-        logging.info('Interpreting time signature {0}'.format(time_signature.id))
-        logging.info('... Members {0}'.format([m.class_name for m in members]))
-
-        # Whole-time mark? Alla breve?
-        if len(members) == 0:
-            raise NotationGraphError('Time signature has no members: {0}'
-                                     ''.format(time_signature.id))
-
-        is_whole = False
-        is_alla_breve = False
-        for m in members:
-            if m.class_name == 'whole-time_mark':
-                is_whole = True
-            if m.class_name == 'alla_breve':
-                is_alla_breve = True
-
-        if is_whole or is_alla_breve:
-            logging.info('Time signature {0}: whole or alla breve, returning 4.0'
-                         ''.format(time_signature.id))
-            return 4.0
-
-        # Process numerals
-        logging.info('... Found numeric time signature, determining whether'
-                     ' it is fractional.')
-
-        # Does the time signature have a fraction-like format?
-        is_fraction_like = True
-        has_letter_other = (len([m for m in members if m.class_name == 'letter_other']) > 0)
-        #  - Does it have a separator slash?
-        if has_letter_other:
-            logging.info('... Has fraction slash')
-            is_fraction_like = True
-        #  - Does it have less than 2 members?
-        elif len(members) < 2:
-            logging.info('... Just one member')
-            is_fraction_like = False
-        #  - If it has 2 or more members, determine minimal IoU and compare
-        #    against FRACTIONAL_VERTICAL_IOU_THRESHOLD. If the minimal IoU
-        #    is under the threshold, then consider the numerals far apart
-        #    vertically so that they constitute a fraction.
-        else:
-            logging.info('... Must check for min. vertical overlap')
-            vertical_overlaps = []
-            for _i_m, m1 in enumerate(members[:-1]):
-                for m2 in members[_i_m:]:
-                    vertical_overlaps.append(bounding_box_dice_coefficient(m1.bounding_box, m2.bounding_box))
-            logging.info('... Vertical overlaps found: {0}'.format(vertical_overlaps))
-            if min(vertical_overlaps) < FRACTIONAL_VERTICAL_IOU_THRESHOLD:
-                is_fraction_like = True
-            else:
-                is_fraction_like = False
-
-        numerals = sorted(self.__children(time_signature, _CONST.NUMERALS),
-                          key=lambda x: x.top)
-        if not is_fraction_like:
-            logging.info('... Non-fractional numeric time sig.')
-            # Read numeral left to right, this is the beat count
-            if len(numerals) == 0:
-                raise NotationGraphError('Time signature has no numerals, but is'
-                                         ' not fraction-like! {0}'
-                                         ''.format(time_signature.id))
-            beats = OnsetsInferenceEngine.interpret_numerals(numerals)
-            logging.info('... Beats: {0}'.format(beats))
-            return beats
-
-        else:
-            logging.info('... Fractional time sig.')
-            # Split into numerator and denominator
-            #  - Sort numerals top to bottom
-            #  - Find largest gap
-            #  - Everything above largest gap is numerator, everything below
-            #    is denominator.
-            numerals_topdown = sorted(numerals, key=lambda c: (c.top + c.bottom) / 2)
-            gaps = [((c2.bottom + c2.top) / 2) - ((c1.bottom + c2.top) / 2)
-                    for c1, c2 in zip(numerals_topdown[:-1], numerals_topdown[1:])]
-            largest_gap_idx = max(list(range(len(gaps))), key=lambda i: gaps[i]) + 1
-            numerator = numerals[:largest_gap_idx]
-            denominator = numerals[largest_gap_idx:]
-            beat_count = OnsetsInferenceEngine.interpret_numerals(numerator)
-            beat_units = OnsetsInferenceEngine.interpret_numerals(denominator)
-
-            beats = beat_count / (beat_units / 4)
-            logging.info('...signature : {0} / {1}, beats: {2}'
-                         ''.format(beat_count, beat_units, beats))
-
-            return beats
-
-    def onsets(self, nodes: List[Node]):
-        """Infers the onsets of notes in the given Nodes.
-
-        The onsets are measured in beats.
-
-        :returns: A id --> onset dict for all notehead-type
-            Nodes.
-        """
-        # We first find the precedence graph. (This is the hard
-        # part.)
-        # The precedence graph is a DAG structure of PrecedenceGraphNode
-        # objects. The infer_precedence() method returns a list
-        # of the graph's source nodes (of which there is in fact
-        # only one, the way it is currently defined).
-        precedence_graph = self.infer_precedence_from_annotations(nodes)
-        for node in precedence_graph:
-            node.onset = 0
-
-        # Once we have the precedence graph, we need to walk it.
-        # It is a DAG, so we simply do a BFS from each source.
-        # Whenever a node has more incoming predecessors,
-        # we need to wait until they are *all* resolved,
-        # and check whether they agree.
-        queue = []
-        # Note: the queue should be prioritized by *onset*, not number
-        # of links from initial node. Leades to trouble with unprocessed
-        # ancestors...
-        for node in precedence_graph:
-            if len(node.inlinks) == 0:
-                queue.append(node)
-
-        onsets = {}
-
-        logging.debug('Size of initial queue: {0}'.format(len(queue)))
-        logging.debug('Initial queue: {0}'.format([(q.obj.id, q.onset) for q in queue]))
-
-        # We will only be appending to the queue, so the
-        # start of the queue is defined simply by the index.
-        __qstart = 0
-        __prec_clsnames = _CONST.classes_affecting_onsets
-        __n_prec_nodes = len([c for c in nodes
-                              if c.class_name in __prec_clsnames])
-        __delayed_prec_nodes = dict()
-        while (len(queue) - __qstart) > 0:
-            # if len(queue) > 2 * __n_prec_nodes:
-            #     logging.warning('Safety valve triggered: queue growing endlessly!')
-            #     break
-
-            q = queue[__qstart]
-            logging.debug('Current @{0}: {1}'.format(__qstart, q.obj.id))
-            logging.debug('Will add @{0}: {1}'.format(__qstart, q.outlinks))
-
-            __qstart += 1
-            for post_q in q.outlinks:
-                if post_q not in queue:
-                    queue.append(post_q)
-
-            logging.debug('Queue state: {0}'
-                          ''.format([ppq.obj.id for ppq in queue[__qstart:]]))
-
-            logging.debug('  {0} has onset: {1}'.format(q.node_id, q.onset))
-            if q.onset is not None:
-                if q.onset > 0:
-                    break
-                onsets[q.obj.id] = q.onset
-                continue
-
-            prec_qs = q.inlinks
-            prec_onsets = [pq.onset for pq in prec_qs]
-            # If the node did not yet get all its ancestors processed,
-            # send it down the queue.
-            if None in prec_onsets:
-                logging.warning('Found node with predecessor that has no onset yet; delaying processing: {0}'
-                                ''.format(q.obj.id))
-                queue.append(q)
-                if q in __delayed_prec_nodes:
-                    logging.warning('This node has already been delayed once! Breaking.')
-                    logging.warning('Queue state: {0}'
-                                    ''.format([ppq.obj.id for ppq in queue[__qstart:]]))
-                    break
-                else:
-                    __delayed_prec_nodes[q.obj.id] = q
-                    continue
-
-            prec_durations = [pq.duration for pq in prec_qs]
-
-            logging.debug('    Prec_onsets @{0}: {1}'.format(__qstart - 1, prec_onsets))
-            logging.debug('    Prec_durations @{0}: {1}'.format(__qstart - 1, prec_durations))
-
-            onset_proposals = [o + d for o, d in zip(prec_onsets, prec_durations)]
-            if min(onset_proposals) != max(onset_proposals):
-                if self.strategy.permissive_desynchronization:
-                    logging.warning('Object {0}: onsets not synchronized from'
-                                    ' predecessors: {1}'.format(q.obj.id,
-                                                                onset_proposals))
-                    onset = max(onset_proposals)
-                else:
-                    raise ValueError('Object {0}: onsets not synchronized from'
-                                     ' predecessors: {1}'.format(q.obj.id,
-                                                                 onset_proposals))
-            else:
-                onset = onset_proposals[0]
-
-            q.onset = onset
-            # Some nodes do not have a Node assigned.
-            if q.obj is not None:
-                onsets[q.obj.id] = onset
-                ### DEBUG -- add this to the Data dict
-                q.obj.data['onset_beats'] = onset
-
-        return onsets
-
-    def __children(self, c, clsnames):
-        """Retrieve the children of the given Node ``c``
-        that have class in ``clsnames``."""
-        return [self.id_to_node_mapping[o] for o in c.outlinks
-                if self.id_to_node_mapping[o].class_name in clsnames]
-
-    def __parents(self, c, clsnames):
-        """Retrieve the parents of the given Node ``c``
-        that have class in ``clsnames``."""
-        return [self.id_to_node_mapping[i] for i in c.inlinks
-                if self.id_to_node_mapping[i].class_name in clsnames]
-
-    def __warning_or_error(self, message):
-        if self.strategy.permissive:
-            logging.warning(message)
-        else:
-            raise ValueError(message)
-
-    def process_ties(self, nodes: List[Node], durations, onsets):
-        """Modifies the durations and onsets so that ties are taken into
-        account.
-
-        Every left-hand note in a tie gets its duration extended by the
-        right-hand note's duration. Every right-hand note's onset is removed.
-
-        :returns: the modified durations and onsets.
-        """
-        logging.info('Processing ties...')
-        g = NotationGraph(nodes=nodes)
-
-        def __get_tie_notes(_tie, graph):
-            notes = graph.parents(_tie, class_filter=['noteheadFull', 'notehead-empty'])
-            if len(notes) == 0:
-                raise NotationGraphError('No notes from tie {0}'.format(_tie.id))
-            if len(notes) == 1:
-                return [notes[0]]
-            if len(notes) > 2:
-                raise NotationGraphError('More than two notes from tie {0}'.format(_tie.id))
-            # Now it has to be 2
-            l, r = sorted(notes, key=lambda n: n.left)
-            return l, r
-
-        def _is_note_left(c, _tie, graph):
-            tie_notes = __get_tie_notes(_tie, graph)
-            if len(tie_notes) == 2:
-                l, r = tie_notes
-                return l.id == c.id
-            else:
-                return True
-
-        new_onsets = copy.deepcopy(onsets)
-        new_durations = copy.deepcopy(durations)
-        # Sorting notes right to left. This means: for notes in the middle
-        # of two ties, its duration is already updated and it can be removed from
-        # the new onsets dict by the time we process the note on the left
-        # of the leftward tie (its predecessor).
-        for k in sorted(onsets, key=lambda x: onsets[x], reverse=True):
-            ties = g.children(k, class_filter=[_CONST.TIE_CLASS_NAME])
-            if len(ties) == 0:
-                continue
-
-            if len(ties) > 1:
-                # Pick the rightmost tie (we're processing onsets from the right)
-                tie = max(ties, key=lambda x: x.left)
-            else:
-                tie = ties[0]
-            n = g[k]
-            tie_notes = __get_tie_notes(tie, graph=g)
-            if len(tie_notes) != 2:
-                continue
-
-            l, r = tie_notes
-            if l.id == n.id:
-                logging.info('Note {0} is left in tie {1}'
-                             ''.format(l.id, tie.id))
-                new_durations[l.id] += new_durations[r.id]
-                del new_onsets[r.id]
-
-        new_durations = {k: new_durations[k] for k in new_onsets}
-        return new_durations, new_onsets
-
-
-class PrecedenceGraphNode(object):
-    """A helper plain-old-data class for onset extraction.
-    The ``inlinks`` and ``outlinks`` attributes are lists
-    of other ``PrecedenceGraphNode`` instances.
-    """
-
-    def __init__(self, objid=None, node: Node = None, inlinks=None, outlinks=None,
-                 onset=None, duration=0):
-        # Optional link to Nodes, or just a placeholder ID.
-        self.obj = node
-        if objid is None and node is not None:
-            objid = node.id
-        self.node_id = objid
-
-        self.inlinks = []
-        if inlinks:
-            self.inlinks = inlinks
-        self.outlinks = []
-        if outlinks:
-            self.outlinks = outlinks
-
-        self.onset = onset
-        '''Counting from the start of the musical sequence, how many
-        beat units pass before this object?'''
-
-        self.duration = duration
-        '''By how much musical time does the object delay the onsets
-        of its descendants in the precedence graph?'''
-
-
-class MIDIBuilder(object):
-
-    def midi_matrix_to_pdo(self, midi_matrix, framerate=20, tempo=120):
-        """Builds the pitch, duration and onset dicts from a given MIDI
-        matrix. Does *not* take into account possible re-articulations:
-        repeated adjacent notes are transformed into just one.
-
-        :param midi_matrix: A ``128 x n_frames`` binary numpy array.
-            Expected to be in the less intuitive format, where pitch
-            ``J`` is encoded in row ``(128 - J)`` -- you would plot this
-            with ``origin=lower`` in the ``imshow()`` call.
-
-        :param FPS: each frame in the MIDI matrix corresponds to ``1 / FPS``
-            of a second. Used together with ``tempo`` to determine durations
-            in beats.
-
-        :param tempo: The tempo in which the MIDI matrix should be interpreted.
-            This does not actually matter for the output MIDI -- you can
-            balance it out by using a different ``FPS`` value. However, it is
-            necessary to compute durations and onsets in beats, since this is
-            what the MIDI building functions in ``midiutil.MidiFile`` expect.
-
-        :returns: ``pitches, durations, onsets``. These are dicts indexed
-            by note ID (equivalent to notehead objids in MuNG context).
-            Pitches contain for each note the MIDI pitch code, durations
-            contain its duration in beats, and onsets contain its onset
-            in beats.
-        """
-        pitches = dict()
-        durations = dict()
-        onsets = dict()
-
-        # Collect pitch activities.
-
-        # For each pitch, contains a list of (start_frame, end_frame+1) pairs.
-        activities = collections.defaultdict(list)
-
-        n_frames = midi_matrix.shape[1]
-        n_pitch_classes = midi_matrix.shape[0]
-        currently_active = dict()
-        for i_frame in range(n_frames):
-            # Collect onsets
-            frame = midi_matrix[:, i_frame]
-            for idx, entry in enumerate(frame):
-                # pitch = n_pitch_classes - idx
-                pitch = idx
-                if entry != 0:
-                    if pitch not in currently_active:
-                        # Start activity
-                        currently_active[pitch] = i_frame
-                else:
-                    if pitch in currently_active:
-                        activities[pitch].append((currently_active[pitch], i_frame))
-                        del currently_active[pitch]
-
-        # Convert pitch activities into onset/pitch/duration dicts.
-        notes = []
-        for pitch in activities:
-            for onset_frame, end_frame in activities[pitch]:
-                notes.append((onset_frame, pitch, end_frame - onset_frame))
-        # Sort by start and from lowest to highest:
-        ordered_by_start_frame = sorted(notes)
-
-        # Distribute into pitch/duration/onset dicts
-        for event_idx, (onset_frame, pitch, duration_frames) in enumerate(notes):
-            onset_beats = self.frames2beats(onset_frame,
-                                            framerate=framerate,
-                                            tempo=tempo)
-            duration_beats = self.frames2beats(duration_frames,
-                                               framerate=framerate,
-                                               tempo=tempo)
-            pitches[event_idx] = pitch
-            durations[event_idx] = duration_beats
-            onsets[event_idx] = onset_beats
-
-        logging.debug('{} note events, last onset: beat {} (seconds: {})'
-                      ''.format(len(notes), notes[-1][0], notes[-1][0] * tempo / 60.))
-
-        return pitches, durations, onsets
-
-    def frames2beats(self, n_frames, framerate, tempo):
-        """Converts a number of frames to duration in beats,
-        given a framerate and tempo."""
-        return (n_frames / float(framerate)) * (tempo / 60.)
-
-    def build_midi(self, pitches, durations, onsets, selection=None, tempo=120):
-        from midiutil.MidiFile import MIDIFile
-
-        # create your MIDI object
-        mf = MIDIFile(1)  # only 1 track
-        track = 0  # the only track
-
-        time = 0  # start at the beginning
-        mf.addTrackName(track, time, "Sample Track")
-        mf.addTempo(track, time, tempo)
-
-        channel = 0
-        volume = 100
-
-        keys = list(pitches.keys())
-
-        min_onset = 0
-        if selection is not None:
-            keys = [k for k in keys if k in selection]
-            min_onset = min([onsets[k] for k in keys if k in onsets])
-
-        for objid in keys:
-            if (objid in onsets) and (objid in durations):
-                pitch = pitches[objid]
-                onset = onsets[objid] - min_onset
-                duration = durations[objid]
-                mf.addNote(track, channel, pitch, onset, duration, volume)
-
-        return mf
-
-
-def play_midi(midi,
-              tmp_dir,
-              soundfont='~/.fluidsynth/FluidR3_GM.sf2',
-              cleanup=False):
-    """Plays (or attempts to play) the given MIDIFile object.
-
-    :param midi: A ``midiutils.MidiFile.MIDIFile`` object
-        containing the data that you wish to play.
-
-    :param tmp_dir: A writeable directory where the MIDI will be
-        exported into a temporary file.
-
-    :param soundfont: A *.sf2 soundfont for FluidSynth to load.
-    """
-    from midi2audio import FluidSynth
-
-    import uuid
-    tmp_midi_path = os.path.join(tmp_dir, 'play_' + str(uuid.uuid4())[:8] + '.mid')
-    with open(tmp_midi_path, 'wb') as hdl:
-        midi.writeFile(hdl)
-    if not os.path.isfile(tmp_midi_path):
-        logging.warning('Could not write MIDI data to temp file {0}!'.format(tmp_midi_path))
-        return
-
-    fs = FluidSynth(soundfont)
-    fs.play_midi(tmp_midi_path)
-    # Here's hoping it's a blocking call. Otherwise, just leave the MIDI;
-    # MUSCIMarker cleans its tmp dir whenever it exits.
-    if cleanup:
-        os.unlink(tmp_midi_path)
+import collections
+import copy
+import logging
+import operator
+from typing import List, Dict, Tuple
+
+from mung.constants import InferenceEngineConstants
+from mung.graph import group_staffs_into_systems, NotationGraph, NotationGraphError
+from mung.node import bounding_box_dice_coefficient, Node
+
+_CONST = InferenceEngineConstants()
+
+
+class OnsetsInferenceStrategy(object):
+    def __init__(self):
+        self.permissive_desynchronization = True
+        self.precedence_only_for_objects_connected_to_staff = True
+        self.permissive = True
+
+
+class PitchInferenceStrategy(object):
+    def __init__(self):
+        self.permissive = True
+
+
+class PitchInferenceEngineState(object):
+    """This class represents the state of the MIDI pitch inference
+    engine during inference.
+
+    Reading pitch is a stateful operations. One needs to remember
+    how stafflines and staffspaces map to pitch codes. This is governed
+    by two things:
+
+    * The clef, which governs
+    * The accidentals: key signatures and inline accidentals.
+
+    Clef and key signature have unlimited scope which only changes when
+    a new key signature is introduced (or the piece ends). The key
+    signature affects all pitches in the given step class (F, C, G, ...)
+    regardless of octave. Inline accidentals have scope until the next
+    measure separator, and they are only valid within their own octave.
+
+    The pitch inference algorithm is run for each staff separately.
+
+    Base pitch representation
+    -------------------------
+
+    The base pitch corresponds to the pitch encoded by a notehead
+    simply sitting on the given staffline/staffspace, without any
+    regard to accidentals (key signature or inline). It is computed
+    by *distance from center staffline* of a staff, with positive
+    distance corresponding to going *up* and negative for going *down*
+    from the center staffline.
+
+    Accidentals representation
+    --------------------------
+
+    The accidentals are associated also with each staffline/staffspace,
+    as counted from the current center. (This means i.a. that
+    the octave periodicity is 7, not 12.)
+
+    There are two kinds of accidentals based on scope: key signature,
+    and inline. Inline accidentals are valid only up to the next
+    measure_separator, while key signature accidentals are valid
+    up until the key signature changes. Key signature accidentals
+    also apply across all octaves, while inline accidentals only apply
+    on the specific staffline.
+
+    Note that inline accidentals may *cancel* key signature
+    accidentals: they override the key signature when given.
+
+    Key accidentals are given **mod 7**.
+
+    Pitch inference procedure
+    -------------------------
+
+    Iterate through the relevant objects on a staff, sorted left-to-right
+    by left edge.
+    """
+
+    def __init__(self):
+
+        self.base_pitch = None  # type: int
+        '''The MIDI code corresponding to the middle staffline,
+        without modification by key or inline accidentals.'''
+
+        self.base_pitch_step = None  # type: int
+        '''The name of the base pitch: C, D, E, etc.'''
+
+        self.base_pitch_octave = None  # type: int
+        '''The octave where the pitch resides. C4 = c', the middle C.'''
+
+        self.current_clef = None  # type:Node
+        '''Holds the clef Node that is currently valid.'''
+
+        self.current_delta_steps = None  # type: List[int]
+        '''Holds for each staffline delta step (i.e. staffline delta mod 7)
+        the MIDI pitch codes.'''
+
+        self.current_clef_delta_shift = 0  # type: int
+        '''If the clef is in a non-standard position, this number is added
+        to the pitch computation delta.'''
+
+        self.key_accidentals = {}  # type: Dict[int,str]
+        self.inline_accidentals = {}  # type: Dict[int,str]
+
+    def reset(self):
+        self.base_pitch = None
+        self.current_clef = None
+        self.current_delta_steps = None
+        self.key_accidentals = {}
+        self.inline_accidentals = {}
+
+    def __str__(self):
+        lines = list()
+        lines.append('Current pitch inference state:')
+        lines.append('\tbase_pitch: {0}'.format(self.base_pitch))
+        lines.append('\tbase_pitch_step: {0}'.format(self.base_pitch_step))
+        lines.append('\tbase_pitch_octave: {0}'.format(self.base_pitch_octave))
+        if self.current_clef is not None:
+            lines.append('\t_current_clef: {0}'.format(self.current_clef.id))
+        else:
+            lines.append('\t_current_clef: None')
+        lines.append('\t_current_delta_steps: {0}'.format(self.current_delta_steps))
+        lines.append('\t_current_clef_delta_shift: {0}'.format(self.current_clef_delta_shift))
+        lines.append('\tkey_accidentals: {0}'.format(self.key_accidentals))
+        lines.append('\tinline_accidentals: {0}'.format(self.inline_accidentals))
+        return '\n'.join(lines)
+
+    def init_base_pitch(self, clef: Node = None, delta: int = 0):
+        """Initializes the base pitch while taking into account
+        the displacement of the clef from its initial position."""
+        self.init_base_pitch_default_staffline(clef)
+        self.current_clef_delta_shift = -1 * delta
+
+    def init_base_pitch_default_staffline(self, clef: Node = None):
+        """Based solely on the clef class name and assuming
+        default stafflines, initialize the base pitch.
+        By default, initializes as though given a gClef."""
+
+        # There should be a mechanism for clefs that are connected
+        # directly to a staffline -- in non-standard positions
+        # (mostly cClefs, like page 03, but there is no reason
+        #  to limit this to cClefs).
+
+        if (clef is None) or (clef.class_name == _CONST.G_CLEF):
+            new_base_pitch = 71
+            new_delta_steps = [0, 1, 2, 2, 1, 2, 2, 2]
+            new_base_pitch_step = 6  # Index into pitch steps.
+            new_base_pitch_octave = 4
+        elif clef.class_name == _CONST.F_CLEF:
+            new_base_pitch = 50
+            new_delta_steps = [0, 2, 1, 2, 2, 2, 1, 2]
+            new_base_pitch_step = 1
+            new_base_pitch_octave = 3
+        elif clef.class_name == _CONST.C_CLEF:
+            new_base_pitch = 60
+            new_delta_steps = [0, 2, 2, 1, 2, 2, 2, 1]
+            new_base_pitch_step = 0
+            new_base_pitch_octave = 4
+        else:
+            raise ValueError('Unrecognized clef class_name: {0}'
+                             ''.format(clef.class_name))
+
+        # Shift the key and inline accidental deltas
+        # according to the change.
+        if self.current_clef is not None:
+            transposition_delta = _CONST.CLEF_CHANGE_DELTA[self.current_clef.class_name][clef.class_name]
+            if transposition_delta != 0:
+                new_key_accidentals = {
+                    (d + transposition_delta) % 7: v
+                    for d, v in list(self.key_accidentals.items())
+                }
+                new_inline_accidentals = {
+                    d + transposition_delta: v
+                    for d, v in list(self.inline_accidentals.items())
+                }
+                self.key_accidentals = new_key_accidentals
+                self.inline_accidentals = new_inline_accidentals
+
+        self.base_pitch = new_base_pitch
+        self.base_pitch_step = new_base_pitch_step
+        self.base_pitch_octave = new_base_pitch_octave
+        self.current_clef = clef
+        self.current_delta_steps = new_delta_steps
+
+    def set_key(self, number_of_sharps: int = 0, number_of_flats: int = 0):
+        """Initialize the staffline delta --> key accidental map.
+        Currently works only on standard key signatures, where
+        there are no repeating accidentals, no double sharps/flats,
+        and the order of accidentals is the standard major/minor system.
+
+        However, we can deal at least with key signatures that combine
+        sharps and flats (if not more than 7), as seen e.g. in harp music.
+
+        :param number_of_sharps: How many sharps are there in the key signature?
+
+        :param number_of_flats: How many flats are there in the key signature?
+        """
+        if number_of_flats + number_of_sharps > 7:
+            raise ValueError('Cannot deal with key signature that has'
+                             ' more than 7 sharps + flats!')
+
+        if self.base_pitch is None:
+            raise ValueError('Cannot initialize key if base pitch is not known.')
+
+        new_key_accidentals = {}
+
+        # The pitches (F, C, G, D, ...) have to be re-cast
+        # in terms of deltas, mod 7.
+        if (self.current_clef is None) or (self.current_clef.class_name == _CONST.G_CLEF):
+            deltas_sharp = [4, 1, 5, 2, 6, 3, 0]
+            deltas_flat = [0, 3, 6, 2, 5, 1, 4]
+        elif self.current_clef.class_name == _CONST.C_CLEF:
+            deltas_sharp = [3, 0, 4, 1, 5, 2, 6]
+            deltas_flat = [6, 2, 5, 1, 4, 0, 3]
+        elif self.current_clef.class_name == _CONST.F_CLEF:
+            deltas_sharp = [2, 6, 3, 0, 4, 1, 5]
+            deltas_flat = [5, 1, 4, 0, 3, 6, 2]
+        else:
+            raise ValueError("Incorrect clef node set as current_clef {0}.".format(self.current_clef))
+
+        for d in deltas_sharp[:number_of_sharps]:
+            new_key_accidentals[d] = 'sharp'
+        for d in deltas_flat[:number_of_flats]:
+            new_key_accidentals[d] = 'flat'
+
+        self.key_accidentals = new_key_accidentals
+
+    def set_inline_accidental(self, delta: int, accidental: Node):
+        self.inline_accidentals[delta] = accidental.class_name
+
+    def reset_inline_accidentals(self):
+        self.inline_accidentals = {}
+
+    def accidental(self, delta: int) -> int:
+        """Returns the modification, in MIDI code, corresponding
+        to the staffline given by the delta."""
+        pitch_mod = 0
+
+        step_delta = delta % 7
+        if step_delta in self.key_accidentals:
+            if self.key_accidentals[step_delta] == 'sharp':
+                pitch_mod = 1
+            elif self.key_accidentals[step_delta] == 'double_sharp':
+                pitch_mod = 2
+            elif self.key_accidentals[step_delta] == 'flat':
+                pitch_mod = -1
+            elif self.key_accidentals[step_delta] == 'double_flat':
+                pitch_mod = -2
+
+        # Inline accidentals override key accidentals.
+        if delta in self.inline_accidentals:
+            if self.inline_accidentals[delta] == 'natural':
+                logging.info('Natural at delta = {0}'.format(delta))
+                pitch_mod = 0
+            elif self.inline_accidentals[delta] == 'sharp':
+                pitch_mod = 1
+            elif self.inline_accidentals[delta] == 'double_sharp':
+                pitch_mod = 2
+            elif self.inline_accidentals[delta] == 'flat':
+                pitch_mod = -1
+            elif self.inline_accidentals[delta] == 'double_flat':
+                pitch_mod = -2
+        return pitch_mod
+
+    def pitch(self, delta: int) -> int:
+        """Given a staffline delta, returns the current MIDI pitch code.
+
+        (This method is the main interface of the PitchInferenceEngineState.)
+
+        :delta: Distance in stafflines + staffspaces from the middle staffline.
+            Negative delta means distance *below*, positive delta is *above*.
+
+        :returns: The MIDI pitch code for the given delta.
+        """
+        delta += self.current_clef_delta_shift
+
+        # Split this into octave and step components.
+        delta_step = delta % 7
+        delta_octave = delta // 7
+
+        # From the base pitch and clef:
+        step_pitch = self.base_pitch \
+                     + sum(self.current_delta_steps[:delta_step + 1]) \
+                     + (delta_octave * 12)
+        accidental_pitch = self.accidental(delta)
+
+        pitch = step_pitch + accidental_pitch
+
+        if self.current_clef_delta_shift != 0:
+            logging.info('PitchInferenceState: Applied clef-based delta {0},'
+                         ' resulting delta was {1}, pitch {2}'
+                         ''.format(self.current_clef_delta_shift,
+                                   delta, pitch))
+
+        return pitch
+
+    def pitch_name(self, delta: int) -> Tuple[str, int]:
+        """Given a staffline delta, returns the name of the corrensponding pitch."""
+        delta += self.current_clef_delta_shift
+
+        output_step = _CONST.PITCH_STEPS[(self.base_pitch_step + delta) % 7]
+        output_octave = self.base_pitch_octave + ((delta + self.base_pitch_step) // 7)
+
+        output_mod = ''
+        accidental = self.accidental(delta)
+        if accidental == 1:
+            output_mod = _CONST.ACCIDENTAL_CODES['sharp']
+        elif accidental == 2:
+            output_mod = _CONST.ACCIDENTAL_CODES['double_sharp']
+        elif accidental == -1:
+            output_mod = _CONST.ACCIDENTAL_CODES['flat']
+        elif accidental == 2:
+            output_mod = _CONST.ACCIDENTAL_CODES['double_flat']
+
+        return output_step + output_mod, output_octave
+
+
+class PitchInferenceEngine(object):
+    """The Pitch Inference Engine extracts MIDI from the notation
+    graph. To get the MIDI, there are two streams of information
+    that need to be combined: pitches and onsets, where the onsets
+    are necessary both for ON and OFF events.
+
+    Pitch inference is done through the ``infer_pitches()`` method.
+
+    Onsets inference is done in two stages. First, the durations
+    of individual notes (and rests) are computed, then precedence
+    relationships are found and based on the precedence graph
+    and durations, onset times are computed.
+
+    Onset inference
+    ---------------
+
+    Onsets are computed separately by measure, which enables time
+    signature constraint checking.
+
+    (This can be implemented in the precedence graph structure,
+    by (a) not allowing precedence edges to cross measure separators,
+    (b) chaining measure separators, or it can be implemented
+    directly in code. The first option is way more elegant.)
+
+    Creating the precedence graph
+    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+    * Get measure separators.
+    * Chain measure separators in precedence relationships.
+    * Group Nodes by bins between measure separators.
+    * For each staff participating in the current measure
+      (as defined by the relevant measure separator outlinks):
+
+        * Infer precedence between the participating notes & rests,
+        * Attach the sources of the resulting DAG to the leftward
+          measure_separator (if there is none, just leave them
+          as sources).
+
+    Invariants
+    ^^^^^^^^^^
+
+    * There is exactly one measure separator starting each measure,
+      except for the first measure, which has none. That implies:
+      when there are multiple disconnected barlines marking the interface
+      of the same two measures within a system, they are joined under
+      a single measure_separator anyway.
+    * Staff groupings are correct, and systems are read top-down.
+
+    """
+
+    def __init__(self, strategy=PitchInferenceStrategy()):
+        # Static temp data from which the pitches are inferred
+        self.id_to_node_mapping = {}
+
+        self.strategy = strategy
+
+        self.staves = None
+
+        self.clefs = None
+        self.clef_to_staff_map = None
+        self.staff_to_clef_map = None
+
+        self.key_signatures = None
+        self.key_to_staff_map = None
+        self.staff_to_key_map = None
+
+        self.measure_separators = None
+        self.staff_to_msep_map = None
+
+        self.noteheads = None
+        self.staff_to_noteheads_map = None
+
+        # Dynamic temp data: things that change as the pitches are inferred.
+        self.pitch_state = PitchInferenceEngineState()
+
+        # Results
+        self.pitches = None
+        self.pitches_per_staff = None
+
+        self.pitch_names = None
+        self.pitch_names_per_staff = None
+
+        # self.durations_beats = None
+        # self.durations_beats_per_staff = None
+
+    def reset(self):
+        self.__init__()
+
+    def infer_pitches(self, nodes: List[Node], with_names=False):
+        """The main workhorse for pitch inference.
+        Gets a list of Nodes and for each notehead-type
+        symbol, outputs a MIDI code corresponding to the pitch
+        encoded by that notehead.
+
+        Notehead
+        --------
+
+        * Check for ties; if there is an incoming tie, apply
+          the last pitch. (This is necessary because of ties
+          that go across barlines and maintain inline accidentals.)
+        * Determine its staffline delta from the middle staffline.
+        * Check for inline accidentals, apply them to inference state.
+        * Query pitch state with this staffline delta.
+
+        Ties are problematic, because they may reach across
+        staff breaks. This can only be resolved after all staves
+        are resolved and assigned to systems, because until then,
+        it is not clear which staff corresponds to which in the next
+        system. Theoretically, this is near-impossible to resolve,
+        because staves may not continue on the next system (e.g.,
+        instruments that do not play for some time in orchestral scores),
+        so simple staff counting is not foolproof. Some other matching
+        mechanism has to be found, e.g. matching outgoing and incoming
+        ties on the end and beginning of adjacent systems.
+
+        Measure separator
+        -----------------
+
+        * Reset all inline accidentals to empty.
+
+        Clef change
+        -----------
+
+        * Change base pitch
+        * Recompute the key and inline signature delta indexes
+
+        Key change
+        ----------
+
+        * Recompute key deltas
+
+        :param with_names: If set, will return also a dict of
+            id --> pitch names (e.g., {123: 'F#3'}).
+
+        :returns: A dict of ``id`` to MIDI pitch code, with
+            an entry for each (pitched) notehead. If ``with_names``
+            is given, returns a tuple with the id --> MIDI
+            and id --> pitch name dicts.
+
+        """
+        self.id_to_node_mapping = {c.id: c for c in nodes}
+
+        # Initialize pitch temp data.
+        self._collect_symbols_for_pitch_inference(nodes)
+
+        # Staff processing: this is where the inference actually
+        # happens.
+        self.pitches_per_staff = {}
+        self.pitches = {}
+        self.pitch_names_per_staff = {}
+        self.pitch_names = {}
+        # self.durations_beats = {}
+        # self.durations_beats_per_staff = {}
+
+        for staff in self.staves:
+            self.process_staff(staff)
+            self.pitches.update(self.pitches_per_staff[staff.id])
+
+        if with_names:
+            return copy.deepcopy(self.pitches), copy.deepcopy(self.pitch_names)
+        else:
+            return copy.deepcopy(self.pitches)
+
+    def process_staff(self, staff):
+
+        self.pitches_per_staff[staff.id] = {}
+        self.pitch_names_per_staff[staff.id] = {}
+
+        # self.durations_beats_per_staff[staff.id] = {}
+
+        self.pitch_state.reset()
+        self.pitch_state.init_base_pitch()
+
+        queue = sorted(
+            self.staff_to_clef_map[staff.id]
+            + self.staff_to_key_map[staff.id]
+            + self.staff_to_msep_map[staff.id]
+            + self.staff_to_noteheads_map[staff.id],
+            key=lambda x: x.left)
+
+        for q in queue:
+            logging.info('process_staff(): processing object {0}-{1}'
+                         ''.format(q.class_name, q.id))
+            if q.class_name in _CONST.CLEF_CLASS_NAMES:
+                self.process_clef(q)
+            elif q.class_name in _CONST.KEY_SIGNATURE:
+                self.process_key_signature(q)
+            elif q.class_name in _CONST.MEASURE_SEPARATOR_CLASS_NAMES:
+                self.process_measure_separator(q)
+            elif q.class_name in _CONST.NOTEHEAD_CLASS_NAMES:
+                p, pn = self.process_notehead(q, with_name=True)
+                self.pitches[q.id] = p
+                self.pitches_per_staff[staff.id][q.id] = p
+                self.pitch_names[q.id] = pn
+                self.pitch_names_per_staff[staff.id][q.id] = pn
+
+                ### DEBUG
+                if q.id in [131, 83, 89, 94]:
+                    logging.info('PitchInferenceEngine: Processing notehead {0}'
+                                 ''.format(q.id))
+                    logging.info('{0}'.format(self.pitch_state))
+
+                # b = self.beats(q)
+                # self.durations_beats[q.id] = b
+                # self.durations_beats_per_staff[staff.id][q.id] = b
+
+        return self.pitches_per_staff[staff.id]
+
+    def process_notehead(self, notehead, with_name=False):
+        """This is the main workhorse of the pitch inference engine.
+
+        :param notehead: The notehead-class Node for which we
+            want to infer pitch.
+
+        :param with_name: If set, will return not only the MIDI pitch
+            code, but the name of the encoded note (e.g., F#3) as well.
+        """
+        # Processing ties
+        # ---------------
+        ties = self.__children(notehead, [_CONST.TIE_CLASS_NAME])
+        for t in ties:
+            tied_noteheads = self.__parents(t, _CONST.NOTEHEAD_CLASS_NAMES)
+
+            # Corner cases: mistakes and staff breaks
+            if len(tied_noteheads) > 2:
+                raise ValueError('Tie {0}: joining together more than 2'
+                                 ' noteheads!'.format(t.id))
+            if len(tied_noteheads) < 2:
+                logging.warning('Tie {0}: only one notehead. Staff break?'
+                                ''.format(t.id))
+                break
+
+            left_tied_notehead = min(tied_noteheads, key=lambda x: x.left)
+            if left_tied_notehead.id != notehead.id:
+                try:
+                    p = self.pitches[left_tied_notehead.id]
+                    if with_name:
+                        pn = self.pitch_names[left_tied_notehead.id]
+                        return p, pn
+                    else:
+                        return p
+
+                except KeyError:
+                    raise KeyError('Processing tied notehead {0}:'
+                                   ' preceding notehead {1} has no pitch!'
+                                   ''.format(notehead.id, left_tied_notehead.id))
+
+            # If the condition doesn't hold, then this is the leftward
+            # note in the tie, and its pitch needs to be determined.
+
+        # Obtain notehead delta
+        # ---------------------
+        delta = self.staffline_delta(notehead)
+
+        # ### DEBUG
+        # if notehead.id == 200:
+        #     logging.info('Notehead {0}: delta {1}'.format(notehead.unique_id, delta))
+        #     logging.info('\tdelta_step: {0}'.format(delta % 7))
+        #     logging.info('\tdelta_step pitch sum: {0}'
+        #                  ''.format(sum(self.pitch_state._current_delta_steps[:(delta % 7)+1])))
+
+        # Processing inline accidentals
+        # -----------------------------
+        accidentals = self.__children(notehead, _CONST.ACCIDENTAL_CLASS_NAMES)
+
+        if len(accidentals) > 0:
+
+            # Sanity checks
+            if len(accidentals) > 2:
+                self.__warning_or_error('More than two accidentals attached to notehead'
+                                        ' {0}'.format(notehead.id))
+            elif len(accidentals) == 2:
+                naturals = [a for a in accidentals if a.class_name == 'natural']
+                non_naturals = [a for a in accidentals if a.class_name != 'natural']
+                if len(naturals) == 0:
+                    self.__warning_or_error('More than one non-natural accidental'
+                                            ' attached to notehead {0}'
+                                            ''.format(notehead.id))
+
+                if len(non_naturals) == 0:
+                    self.__warning_or_error('Two naturals attached to one notehead {0}'
+                                            ''.format(notehead.id))
+                    self.pitch_state.set_inline_accidental(delta, naturals[0])
+                else:
+                    self.pitch_state.set_inline_accidental(delta, non_naturals[0])
+
+            elif len(accidentals) == 1:
+                self.pitch_state.set_inline_accidental(delta, accidentals[0])
+
+        # Get the actual pitch
+        # --------------------
+        p = self.pitch_state.pitch(delta)
+
+        ### DEBUG
+        if notehead.id in [131, 83, 89, 94]:
+            logging.info('PitchInferenceEngine: results of pitch processing'
+                         ' for notehead {0}'.format(notehead.id))
+            logging.info('\tties: {0}'.format(ties))
+            logging.info('\taccidentals: {0}'.format(accidentals))
+            logging.info('\tdelta: {0}'.format(delta))
+            logging.info('\tpitch: {0}'.format(p))
+
+        if with_name is True:
+            pn = self.pitch_state.pitch_name(delta)
+            return p, pn
+        else:
+            return p
+
+    def staffline_delta(self, notehead: Node):
+        """Computes the staffline delta (distance from middle stafflines,
+        measured in stafflines and staffspaces) for the given notehead
+        (or any other symbol connected to a staffline/staffspace).
+        Accounts for leger lines.
+        """
+        current_staff = self.__children(notehead, ['staff'])[0]
+        staffline_objects = self.__children(notehead,
+                                            _CONST.STAFFLINE_CLASS_NAMES)
+
+        # Leger lines
+        # ------------
+        if len(staffline_objects) == 0:
+
+            # Processing leger lines:
+            #  - count leger lines
+            lls = self.__children(notehead, _CONST.LEGER_LINE)
+            n_lls = len(lls)
+            if n_lls == 0:
+                raise ValueError('Notehead with no staffline or staffspace,'
+                                 ' but also no leger lines: {0}'
+                                 ''.format(notehead.id))
+
+            #  Determine: is notehead above or below staff?
+            is_above_staff = (notehead.top < current_staff.top)
+
+            #  Determine: is notehead on/next to (closest) leger line?
+            #    This needs to be done *after* we know whether the notehead
+            #    is above/below staff: if the notehead is e.g. above,
+            #    then it would be weird to find out it is in the
+            #    mini-staffspace *below* the closest leger line,
+            #    signalling a mistake in the data.
+            closest_ll = min(lls, key=lambda x: (x.top - notehead.top) ** 2 + (x.bottom - notehead.bottom) ** 2)
+
+            # Determining whether the notehead is on a leger
+            # line or in the adjacent temp staffspace.
+            # This uses a magic number, ON_STAFFLINE_RATIO_THRESHOLD.
+            on_leger_line = True
+
+            ### DEBUG!!!
+            dtop, dbottom = 1, 1
+
+            # Weird situation with notehead vertically *inside* bbox
+            # of leger line (could happen with slanted LLs and very small
+            # noteheads).
+            if closest_ll.top <= notehead.top <= notehead.bottom <= closest_ll.bottom:
+                on_leger_line = True
+
+            # No vertical overlap between LL and notehead
+            elif closest_ll.top > notehead.bottom:
+                on_leger_line = False
+            elif notehead.top > closest_ll.bottom:
+                on_leger_line = False
+
+            # Complicated situations: overlap
+            else:
+                # Notehead "around" leger line.
+                if notehead.top < closest_ll.top <= closest_ll.bottom < notehead.bottom:
+                    dtop = closest_ll.top - notehead.top
+                    dbottom = notehead.bottom - closest_ll.bottom
+
+                    if min(dtop, dbottom) / max(dtop, dbottom) \
+                            < _CONST.ON_STAFFLINE_RATIO_THRESHOLD:
+                        on_leger_line = False
+
+                        # Check orientation congruent with rel. to staff.
+                        # If it is wrong (e.g., notehead mostly under LL
+                        # but above staffline, and looks like off-LL),
+                        # change back to on-LL.
+                        if (dtop > dbottom) and not is_above_staff:
+                            on_leger_line = True
+                            logging.debug('Notehead in LL space with wrong orientation '
+                                          'w.r.t. staff:'
+                                          ' {0}'.format(notehead.id))
+                        if (dbottom > dtop) and is_above_staff:
+                            on_leger_line = True
+                            logging.debug('Notehead in LL space with wrong orientation '
+                                          'w.r.t. staff:'
+                                          ' {0}'.format(notehead.id))
+
+                # Notehead interlaced with leger line, notehead on top
+                elif notehead.top < closest_ll.top <= notehead.bottom <= closest_ll.bottom:
+                    # dtop = closest_ll.top - notehead.top
+                    # dbottom = max(notehead.bottom - closest_ll.top, 1)
+                    # if float(dbottom) / float(dtop) \
+                    #         < _CONST.ON_STAFFLINE_RATIO_TRHESHOLD:
+                    on_leger_line = False
+
+                # Notehead interlaced with leger line, leger line on top
+                elif closest_ll.top <= notehead.top <= closest_ll.bottom < notehead.bottom:
+                    # dtop = max(closest_ll.bottom - notehead.top, 1)
+                    # dbottom = notehead.bottom - closest_ll.bottom
+                    # if float(dtop) / float(dbottom) \
+                    #         < _CONST.ON_STAFFLINE_RATIO_TRHESHOLD:
+                    on_leger_line = False
+
+                else:
+                    raise ValueError('Strange notehead {0} vs. leger line {1}'
+                                     ' situation: bbox notehead {2}, LL {3}'
+                                     ''.format(notehead.id, closest_ll.id,
+                                               notehead.bounding_box,
+                                               closest_ll.bounding_box))
+
+            delta = (2 * n_lls - 1) + 5
+            if not on_leger_line:
+                delta += 1
+
+            if not is_above_staff:
+                delta *= -1
+
+            return delta
+
+        elif len(staffline_objects) == 1:
+            current_staffline = staffline_objects[0]
+
+            # Count how far from the current staffline we are.
+            #  - Collect staffline objects from the current staff
+            all_staffline_objects = self.__children(current_staff,
+                                                    _CONST.STAFFLINE_CLASS_NAMES)
+
+            #  - Determine their ordering, top to bottom
+            sorted_staffline_objects = sorted(all_staffline_objects,
+                                              key=lambda x: (x.top + x.bottom) / 2.)
+
+            delta = None
+            for i, s in enumerate(sorted_staffline_objects):
+                if s.id == current_staffline.id:
+                    delta = 5 - i
+
+            if delta is None:
+                raise ValueError('Notehead {0} attached to staffline {1},'
+                                 ' which is however not a child of'
+                                 ' the notehead\'s staff {2}!'
+                                 ''.format(notehead.id, current_staffline.id,
+                                           current_staff.id))
+
+            return delta
+
+        else:
+            raise ValueError('Notehead {0} attached to more than one'
+                             ' staffline/staffspace!'.format(notehead.id))
+
+    def process_measure_separator(self, measure_separator):
+        self.pitch_state.reset_inline_accidentals()
+
+    def process_key_signature(self, key_signature):
+        sharps = self.__children(key_signature, ['sharp'])
+        flats = self.__children(key_signature, ['flat'])
+        self.pitch_state.set_key(len(sharps), len(flats))
+
+    def process_clef(self, clef):
+        # Check for staffline children
+        stafflines = self.__children(clef, class_names=_CONST.STAFFLINE_CLASS_NAMES)
+        if len(stafflines) == 0:
+            logging.info('Clef not connected to any staffline, assuming default'
+                         ' position: {0}'.format(clef.id))
+            self.pitch_state.init_base_pitch(clef=clef)
+        else:
+            # Compute clef staffline delta from middle staffline.
+            delta = self.staffline_delta(clef)
+            logging.info('Clef {0}: computed staffline delta {1}'
+                         ''.format(clef.id, delta))
+            self.pitch_state.init_base_pitch(clef=clef, delta=delta)
+
+    def _collect_symbols_for_pitch_inference(self, nodes: List[Node],
+                                             ignore_nonstaff=True):
+        """Extract all symbols from the document relevant for pitch
+        inference and index them in the Engine's temp data structures."""
+        graph = NotationGraph(nodes)
+
+        # Collect staves.
+        self.staves = [c for c in nodes if c.class_name == InferenceEngineConstants.STAFF]
+        logging.info('We have {0} staves.'.format(len(self.staves)))
+
+        # Collect clefs and key signatures per staff.
+        self.clefs = [c for c in nodes
+                      if c.class_name in _CONST.CLEF_CLASS_NAMES]
+        if ignore_nonstaff:
+            self.clefs = [c for c in self.clefs if graph.has_children(c, [InferenceEngineConstants.STAFF])]
+
+        self.key_signatures = [c for c in nodes
+                               if c.class_name == InferenceEngineConstants.KEY_SIGNATURE]
+        if ignore_nonstaff:
+            self.key_signatures = [c for c in self.key_signatures
+                                   if graph.has_children(c, [InferenceEngineConstants.STAFF])]
+
+        self.clef_to_staff_map = {}
+        # There may be more than one clef per staff.
+        self.staff_to_clef_map = collections.defaultdict(list)
+        for c in self.clefs:
+            # Assuming one staff per clef
+            try:
+                s = self.__children(c, [InferenceEngineConstants.STAFF])[0]
+            except (KeyError, ValueError):
+                logging.warning('Clef {0} has no staff attached! Will not be'
+                                ' part of pitch inference.'.format(c.id))
+                continue
+            self.clef_to_staff_map[c.id] = s
+            self.staff_to_clef_map[s.id].append(c)
+
+        self.key_to_staff_map = {}
+        # There may be more than one key signature per staff.
+        self.staff_to_key_map = collections.defaultdict(list)
+        for k in self.key_signatures:
+            try:
+                s = self.__children(k, [InferenceEngineConstants.STAFF])[0]
+            except KeyError:
+                logging.warning('Key signature {0} has no staff attached! Will not be'
+                                ' part of pitch inference.'.format(k.id))
+                continue
+            self.key_to_staff_map[k.id] = s
+            self.staff_to_key_map[s.id].append(k)
+
+        # Collect measure separators.
+        self.measure_separators = [c for c in nodes
+                                   if c.class_name == InferenceEngineConstants.MEASURE_SEPARATOR]
+        if ignore_nonstaff:
+            self.measure_separators = [c for c in self.measure_separators
+                                       if graph.has_children(c, [InferenceEngineConstants.STAFF])]
+
+        self.staff_to_msep_map = collections.defaultdict(list)
+        for m in self.measure_separators:
+            _m_staves = self.__children(m, [InferenceEngineConstants.STAFF])
+            # (Measure separators might belong to multiple staves.)
+            for s in _m_staves:
+                self.staff_to_msep_map[s.id].append(m)
+                # Collect accidentals per notehead.
+
+        # Collect noteheads.
+        self.noteheads = [c for c in nodes
+                          if c.class_name in _CONST.NOTEHEAD_CLASS_NAMES]
+        if ignore_nonstaff:
+            self.noteheads = [c for c in self.noteheads
+                              if graph.has_children(c, [InferenceEngineConstants.STAFF])]
+
+        self.staff_to_noteheads_map = collections.defaultdict(list)
+        for n in self.noteheads:
+            s = self.__children(n, [InferenceEngineConstants.STAFF])[0]
+            self.staff_to_noteheads_map[s.id].append(n)
+
+    def __children(self, c: Node, class_names: List[str]) -> List[Node]:
+        """Retrieve the children of the given Node ``c``
+        that have class in ``clsnames``."""
+        return [self.id_to_node_mapping[o] for o in c.outlinks
+                if self.id_to_node_mapping[o].class_name in class_names]
+
+    def __parents(self, c: Node, class_names: List[str]) -> List[Node]:
+        """Retrieve the parents of the given Node ``c``
+        that have class in ``clsnames``."""
+        return [self.id_to_node_mapping[i] for i in c.inlinks
+                if self.id_to_node_mapping[i].class_name in class_names]
+
+    def __warning_or_error(self, message):
+        if self.strategy.permissive:
+            logging.warning(message)
+        else:
+            raise ValueError(message)
+
+
+class OnsetsInferenceEngine(object):
+
+    def __init__(self, nodes: List[Node], strategy=OnsetsInferenceStrategy()):
+        """Initialize the onset inference engine with the full Node
+        list in a document."""
+        self.id_to_node_mapping = {c.id: c for c in nodes}
+
+        self.strategy = strategy
+
+    def durations(self, nodes: List[Node], ignore_modifiers: bool = False) -> Dict[int, float]:
+        """Returns a dict that contains the durations (in beats)
+        of all Nodes that should be associated with a duration.
+        The dict keys are ``id``.
+
+        :param ignore_modifiers: If set, will ignore duration dots,
+            tuples, and other potential duration modifiers when computing
+            the durations. Effectively, this gives you classes that
+            correspond to note(head) type: whole (4.0), half (2.0),
+            quarter (1.0), eighth (0.5), etc.
+        """
+        # Generate & return the durations dictionary.
+        _relevant_clsnames = _CONST.classes_bearing_duration
+        duration_nodes = [c for c in nodes
+                          if c.class_name in _relevant_clsnames]
+
+        durations = {c.id: self.beats(c, ignore_modifiers=ignore_modifiers)
+                     for c in duration_nodes}
+        return durations
+
+    def beats(self, node: Node, ignore_modifiers=False):
+        if node.class_name in _CONST.NOTEHEAD_CLASS_NAMES:
+            return self.notehead_beats(node,
+                                       ignore_modifiers=ignore_modifiers)
+        elif node.class_name in _CONST.REST_CLASS_NAMES:
+            return self.rest_beats(node,
+                                   ignore_modifiers=ignore_modifiers)
+        else:
+            raise ValueError('Cannot compute beats for object {0} of class {1};'
+                             ' beats only available for notes and rests.'
+                             ''.format(node.id, node.class_name))
+
+    def notehead_beats(self, notehead, ignore_modifiers=False) -> float:
+        """Retrieves the duration for the given notehead, in beats.
+
+        It is possible that the notehead has two stems.
+        In that case, we return all the possible durations:
+        usually at most two, but if there is a duration dot, then
+        there can be up to 4 possibilities.
+
+        Grace notes currently return 0 beats.
+
+        :param ignore_modifiers: If given, will ignore all duration
+            modifiers: Duration dots, tuples, and other potential duration
+            modifiers when computing the durations. Effectively, this
+            gives you classes that correspond to note(head) type:
+            whole (4.0), half (2.0), quarter (1.0), eighth (0.5), etc.
+
+        :returns: A list of possible durations for the given notehead.
+            Mostly its length is just 1; for multi-stem noteheads,
+            you might get more.
+        """
+        beat = [0]
+
+        stems = self.children(notehead, [_CONST.STEM])
+        flags_and_beams = self.children(
+            notehead,
+            _CONST.FLAGS_AND_BEAMS)
+
+        if notehead.class_name in _CONST.GRACE_NOTEHEAD_CLASS_NAMES:
+            logging.warning('Notehead {0}: Grace notes get zero duration!'
+                            ''.format(notehead.id))
+            beat = [0]
+
+        elif len(stems) > 1:
+            logging.warning('Inferring duration for multi-stem notehead: {0}'
+                            ''.format(notehead.id))
+            beat = self.process_multistem_notehead(notehead)
+            if len(beat) > 1:
+                self.__warning_or_error('Cannot deal with multi-stem notehead'
+                                        ' where multiple durations apply.')
+                beat = [max(beat)]
+
+        elif notehead.class_name == _CONST.NOTEHEAD_HALF or notehead.class_name == _CONST.NOTEHEAD_WHOLE:
+            if len(flags_and_beams) != 0:
+                raise ValueError(
+                    'Notehead {0} is empty, but has {1} flags and beams!'.format(notehead.id, len(flags_and_beams)))
+
+            if len(stems) == 0:
+                beat = [4]
+            else:
+                beat = [2]
+
+        elif notehead.class_name == _CONST.NOTEHEAD_FULL:
+            if len(stems) == 0:
+                self.__warning_or_error('Full notehead {0} has no stem!'.format(notehead.id))
+
+            beat = [0.5 ** len(flags_and_beams)]
+
+        else:
+            raise ValueError('Notehead {0}: unknown class_name {1}'
+                             ''.format(notehead.id, notehead.class_name))
+
+        if not ignore_modifiers:
+            duration_modifier = self.compute_duration_modifier(notehead)
+            beat = [b * duration_modifier for b in beat]
+
+        if len(beat) > 1:
+            logging.warning('Notehead {0}: more than 1 duration: {1}, choosing first'
+                            ''.format(notehead.id, beat))
+        return beat[0]
+
+    def compute_duration_modifier(self, notehead: Node):
+        """Computes the duration modifier (multiplicative, in beats)
+        for the given notehead (or rest) from the tuples and duration dots.
+
+        Can handle duration dots within tuples.
+
+        Cannot handle nested/multiple tuples.
+        """
+        duration_modifier = 1
+        # Dealing with tuples:
+        tuples = self.children(notehead, [_CONST.TUPLE])
+        if len(tuples) > 1:
+            raise ValueError('Notehead {0}: Cannot deal with more than one tuple'
+                             ' simultaneously.'.format(notehead.id))
+        if len(tuples) == 1:
+            tuple = tuples[0]
+
+            # Find the number in the tuple.
+            numerals = sorted([self.id_to_node_mapping[o] for o in tuple.outlinks
+                               if self.id_to_node_mapping[o].class_name.startswith('numeral')],
+                              key=lambda x: x.left)
+            # Concatenate numerals left to right.
+            tuple_number = int(''.join([num.class_name[-1] for num in numerals]))
+
+            # Last note in tuple should get complementary duration
+            # to sum to a whole. Otherwise, playing brings slight trouble.
+
+            if tuple_number == 2:
+                # Duola makes notes *longer*
+                duration_modifier = 3 / 2
+            elif tuple_number == 3:
+                duration_modifier = 2 / 3
+            elif tuple_number == 4:
+                # This one also makes notes longer
+                duration_modifier = 4 / 3
+            elif tuple_number == 5:
+                duration_modifier = 4 / 5
+            elif tuple_number == 6:
+                # Most often done for two consecutive triolas,
+                # e.g. 16ths with a 6-tuple filling one beat
+                duration_modifier = 2 / 3
+            elif tuple_number == 7:
+                # Here we get into trouble, because this one
+                # can be both 4 / 7 (7 16th in a beat)
+                # or 8 / 7 (7 32nds in a beat).
+                # In the same vein, we cannot resolve higher
+                # tuples unless we establish precedence/simultaneity.
+                logging.warning('Cannot really deal with higher tuples than 6.')
+                # For MUSCIMA++ specifically, we can cheat: there is only one
+                # septuple, which consists of 7 x 32rd in 1 beat, so they
+                # get 8 / 7.
+                logging.warning('MUSCIMA++ cheat: we know there is only 7 x 32rd in 1 beat'
+                                ' in page 14.')
+                duration_modifier = 8 / 7
+            elif tuple_number == 10:
+                logging.warning('MUSCIMA++ cheat: we know there is only 10 x 32rd in 1 beat'
+                                ' in page 04.')
+                duration_modifier = 4 / 5
+            else:
+                raise NotImplementedError('Notehead {0}: Cannot deal with tuple '
+                                          'number {1}'.format(notehead.id,
+                                                              tuple_number))
+
+        # Duration dots
+        ddots = self.children(notehead, [_CONST.AUGMENTATION_DOT])
+        dot_duration_modifier = 1
+        for i, d in enumerate(ddots):
+            dot_duration_modifier += 1 / (2 ** (i + 1))
+        duration_modifier *= dot_duration_modifier
+
+        return duration_modifier
+
+    def rest_beats(self, rest: Node, ignore_modifiers=False) -> float:
+        """Compute the duration of the given rest in beats.
+
+        :param ignore_modifiers: If given, will ignore all duration
+            modifiers: Duration dots, tuples, and other potential duration
+            modifiers when computing the durations. Effectively, this
+            gives you classes that correspond to note(head) type:
+            whole (4.0), half (2.0), quarter (1.0), eighth (0.5), etc.
+            Also ignores deriving duration from the time signature
+            for whole rests.
+
+        """
+
+        rest_beats_dict = {_CONST.REST_WHOLE: 4,  # !!! We should find the Time Signature.
+                           _CONST.REST_HALF: 2,
+                           _CONST.REST_QUARTER: 1,
+                           _CONST.REST_8TH: 0.5,
+                           _CONST.REST_16TH: 0.25,
+                           _CONST.REST_32ND: 0.125,
+                           _CONST.REST_64TH: 0.0625,
+                           # Technically, these two should just apply time sig.,
+                           # but the measure-factorized precedence graph
+                           # means these durations never have sounding
+                           # descendants anyway:
+                           _CONST.MULTI_MEASURE_REST: 4,
+                           _CONST.REPEAT_ONE_BAR: 4,
+                           }
+
+        try:
+            base_rest_duration = rest_beats_dict[rest.class_name]
+
+        except KeyError:
+            raise KeyError('Symbol {0}: Unknown rest type {1}!'
+                           ''.format(rest.id, rest.class_name))
+
+        # Process the whole rest:
+        #  - if it is the only symbol in the measure, it should take on
+        #    the duration of the current time signature.
+        #  - if it is not the only symbol in the measure, it takes 4 beats
+        #  - Theoretically, it could perhaps take e.g. 6 beats in weird situations
+        #    in a 6/2 time signature, but we don't care about this for now.
+        #
+        # If there is no leftward time signature, we need to infer the time
+        # sig from the other symbols. This necessitates two-pass processing:
+        # first get all available durations, then guess the time signatures
+        # (technically this might also be needed for each measure).
+        if (rest.class_name in _CONST.MEAUSURE_LASTING_CLASS_NAMES) and not ignore_modifiers:
+            base_rest_duration = self.measure_lasting_beats(rest)
+            beat = [base_rest_duration]  # Measure duration should never be ambiguous.
+
+        elif not ignore_modifiers:
+            duration_modifier = self.compute_duration_modifier(rest)
+            beat = [base_rest_duration * duration_modifier]
+
+        else:
+            beat = [base_rest_duration]
+
+        if len(beat) > 1:
+            logging.warning('Rest {0}: more than 1 duration: {1}, choosing first'
+                            ''.format(rest.id, beat))
+        return beat[0]
+
+    def measure_lasting_beats(self, node: Node):
+        """Find the duration of an object that lasts for an entire measure
+        by interpreting the time signature valid for the given point in
+        the score.
+
+        If any assumption is broken, will return the default measure duration:
+        4 beats."""
+        # Find rightmost preceding time signature on the staff.
+        graph = NotationGraph(list(self.id_to_node_mapping.values()))
+
+        # Find current time signature
+        staffs = graph.children(node, class_filter=[_CONST.STAFF])
+
+        if len(staffs) == 0:
+            logging.warning('Interpreting object {0} as measure-lasting, but'
+                            ' it is not attached to any staff! Returning default: 4'
+                            ''.format(node.id))
+            return 4
+
+        if len(staffs) > 1:
+            logging.warning('Interpreting object {0} as measure-lasting, but'
+                            ' it is connected to more than 1 staff: {1}'
+                            ' Returning default: 4'
+                            ''.format(node.id, [s.id for s in staffs]))
+            return 4
+
+        logging.info('Found staffs: {0}'.format([s.id for s in staffs]))
+
+        staff = staffs[0]
+        time_signatures = graph.ancestors(staff, class_filter=_CONST.TIME_SIGNATURES)
+
+        logging.info('Time signatures: {0}'.format([t.id for t in time_signatures]))
+
+        applicable_time_signatures = sorted([t for t in time_signatures
+                                             if t.left < node.left],
+                                            key=operator.attrgetter('left'))
+        logging.info('Applicable time signatures: {0}'.format([t.id for t in time_signatures]))
+
+        if len(applicable_time_signatures) == 0:
+            logging.warning('Interpreting object {0} as measure-lasting, but'
+                            ' there is no applicable time signature. Returnig'
+                            ' default: 4'.format(node.id))
+            return 4
+
+        valid_time_signature = applicable_time_signatures[-1]
+        beats = self.interpret_time_signature(valid_time_signature)
+        return beats
+
+    def process_multistem_notehead(self, notehead):
+        """Attempts to recover the duration options of a multi-stem note."""
+        stems = self.children(notehead, ['stem'])
+        flags_and_beams = self.children(
+            notehead,
+            _CONST.FLAGS_AND_BEAMS)
+
+        if len(flags_and_beams) == 0:
+            if notehead.class_name == _CONST.NOTEHEAD_FULL:
+                return [1]
+            elif notehead.class_name in _CONST.NOTEHEADS_EMPTY:
+                return [2]
+
+        if notehead.class_name in _CONST.NOTEHEADS_EMPTY:
+            raise NotationGraphError('Empty notehead with flags and beams: {0}'
+                                     ''.format(notehead.id))
+
+        n_avg_x = notehead.top + (notehead.bottom - notehead.top) / 2.0
+        print('Notehead {0}: avg_x = {1}'.format(notehead.id, n_avg_x))
+        f_and_b_above = []
+        f_and_b_below = []
+        for c in flags_and_beams:
+            c_avg_x = c.top + (c.bottom - c.top) / 2.0
+            print('Beam/flag {0}: avg_x = {1}'.format(c.id, c_avg_x))
+            if c_avg_x < n_avg_x:
+                f_and_b_above.append(c)
+                print('Appending above')
+            else:
+                f_and_b_below.append(c)
+                print('Appending below')
+
+        beat_above = 0.5 ** len(f_and_b_above)
+        beat_below = 0.5 ** len(f_and_b_below)
+
+        if beat_above != beat_below:
+            raise NotImplementedError('Cannot deal with multi-stem note'
+                                      ' that has different pre-modification'
+                                      ' durations: {0} vs {1}'
+                                      '{2}'.format(beat_above, beat_below, notehead.id))
+
+        beat = [beat_above]
+
+        tuples = self.children(notehead, [_CONST.TUPLE])
+        if len(tuples) % 2 != 0:
+            raise NotImplementedError('Cannot deal with multi-stem note'
+                                      ' that has an uneven number of tuples:'
+                                      ' {0}'.format(notehead.id))
+
+        duration_modifier = self.compute_duration_modifier(notehead)
+        beat = [b * duration_modifier for b in beat]
+
+        return beat
+
+    ##########################################################################
+    # Onsets inference
+    def infer_precedence_from_annotations(self, nodes: List[Node]):
+        """Infer precedence graph based solely on the "green lines"
+        in MUSCIMA++ annotation: precedence edges. These are encoded
+        in the data as inlink/outlink lists
+        in ``Node.data['precedence_inlinks']``,
+        and ``Node.data['precedence_outlinks']``.
+
+        :param nodes: A list of Nodes, not necessarily
+            only those that participate in the precedence graph.
+
+        :return: The list of source nodes of the precedence graph.
+        """
+        _relevant_clsnames = _CONST.classes_bearing_duration
+        precedence_nodes = [c for c in nodes
+                            if c.class_name in _relevant_clsnames]
+
+        if self.strategy.precedence_only_for_objects_connected_to_staff:
+            precedence_nodes = [c for c in precedence_nodes
+                                if len(self.children(c, [_CONST.STAFF])) > 0]
+
+        durations = {c.id: self.beats(c) for c in precedence_nodes}
+
+        p_nodes = {}
+        for c in precedence_nodes:
+            p_node = PrecedenceGraphNode(objid=c.id,
+                                         node=c,
+                                         inlinks=[],
+                                         outlinks=[],
+                                         duration=durations[c.id],
+                                         )
+            p_nodes[c.id] = p_node
+
+        for c in p_nodes.values():
+            inlinks = []
+            outlinks = []
+            if 'precedence_inlinks' in c.data:
+                inlinks = c.data['precedence_inlinks']
+            if 'precedence_outlinks' in c.data:
+                outlinks = c.data['precedence_outlinks']
+            p_node = p_nodes[c.node_id]
+            p_node.outlinks = [p_nodes[o] for o in outlinks]
+            p_node.inlinks = [p_nodes[i] for i in inlinks]
+
+        # Join staves/systems!
+
+        # ...systems:
+        systems = group_staffs_into_systems(nodes,
+                                            use_fallback_measure_separators=True)
+
+        if len(systems) == 1:
+            logging.info('Single-system score, no staff chaining needed.')
+            source_nodes = [n for n in list(p_nodes.values()) if len(n.inlinks) == 0]
+            return source_nodes
+
+        # Check all systems same no. of staffs
+        _system_lengths = [len(s) for s in systems]
+        if len(set(_system_lengths)) > 1:
+            raise ValueError('Cannot deal with variable number of staffs'
+                             ' w.r.t. systems! Systems: {0}'.format(systems))
+
+        staff_chains = [[] for _ in systems[0]]
+        for system in systems:
+            for i, staff in enumerate(system):
+                staff_chains[i].append(staff)
+
+        # Now, join the last --> first nodes within chains.
+        # - Assign objects to staffs
+        objid2staff = {}
+        for c in nodes:
+            staffs = self.children(c, [InferenceEngineConstants.STAFF])
+            if len(staffs) == 1:
+                objid2staff[c.id] = staffs[0].id
+
+        # - Assign staffs to sink nodes
+        sink_nodes2staff = {}
+        staff2sink_nodes = collections.defaultdict(list)
+        for node in list(p_nodes.values()):
+            if len(node.outlinks) == 0:
+                try:
+                    staff = self.children(node.obj, [InferenceEngineConstants.STAFF])[0]
+                except IndexError:
+                    logging.error('Object {0} is a sink node in the precedence graph, but has no staff!'
+                                  ''.format(node.obj.id))
+                    raise
+                sink_nodes2staff[node.obj.id] = staff.id
+                staff2sink_nodes[staff.id].append(node)
+
+        # Note that this means you should never have a sink node
+        # unless it's at the end of the staff. All notes have to lead
+        # somewhere. This is suboptimal; we should filter out non-maximal
+        # sink nodes. But since we do not know whether the sink nodes
+        # are maximal until we are done inferring onsets, we have to stick
+        # with this.
+        # The alternative is to only connect to the next staff the *rightmost*
+        # sink node. This risks *not* failing if the sink nodes of a staff
+        # are not synchronized properly.
+
+        # - Assign staffs to source nodes
+        source_nodes2staff = {}
+        staff2source_nodes = collections.defaultdict(list)
+        for node in list(p_nodes.values()):
+            if len(node.inlinks) == 0:
+                staff = self.children(node.obj, [InferenceEngineConstants.STAFF])[0]
+                source_nodes2staff[node.obj.id] = staff.id
+                staff2source_nodes[staff.id].append(node)
+
+        # - For each staff chain, link the sink nodes of the prev
+        #   to the source nodes of the next staff.
+        for staff_chain in staff_chains:
+            staffs = sorted(staff_chain, key=lambda x: x.top)
+            for (s1, s2) in zip(staffs[:-1], staffs[1:]):
+                sinks = staff2sink_nodes[s1.id]
+                sources = staff2source_nodes[s2.id]
+                for sink in sinks:
+                    for source in sources:
+                        sink.outlinks.append(source)
+                        source.inlinks.append(sink)
+
+        source_nodes = [n for n in list(p_nodes.values()) if len(n.inlinks) == 0]
+        return source_nodes
+
+    def infer_precedence(self, nodes: List[Node]):
+        """This is the most complex part of onset computation.
+
+        The output of this method is a **precedence graph**. The precedence
+        graph is a Directed Acyclic Graph (DAG) consisting of
+        :class:`PrecedenceGraphNode` objects. Each node represents some
+        musical concept that participates in establishing the onsets
+        by having a *duration*. The invariant of the graph is that
+        the onset of a node is the sum of the durations on each of its
+        predecessor paths to a root node (which has onset 0).
+
+        Not all nodes necessarily have nonzero duration (although these
+        nodes can technically be factored out).
+
+        Once the precedence graph is formed, then a breadth-first search
+        (rather than DFS, to more easily spot/resolve conflicts at multi-source
+        precedence graph nodes) simply accumulates durations.
+        Conflicts can be resolved through failing (currently implemented),
+        or looking up possible errors in assigning durations and attempting
+        to fix them.
+
+        Forming the precedence graph itself is difficult, because
+        of polyphonic (and especially pianoform) music. Practically the only
+        actual constraint followed throughout music is that *within a voice*
+        notes are read left-to-right. The practice of aligning e.g. whole
+        notes in an outer voice to the beginning of the bar rather than
+        to the middle took over only cca. 1800 or later.
+
+        An imperfect but overwhelmingly valid constraint is that notes taking
+        up a certain proportion of the measure are not written to the *right*
+        of the proportional horizontal span in the measure corresponding
+        to their duration in time. However, this is *not* uniform across
+        the measure: e.g., if the first voice is 2-8-8-8-8 and the second
+        is 2-2, then the first half can be very narrow and the second
+        quite wide, with the second lower-voice half-note in the middle
+        of that part. However, the *first* lower-voice half-note will
+        at least *not* be positioned in the horizontal span where
+        the 8th notes in the upper voice are.
+
+        Which Nodes participate in the precedence graph?
+        ------------------------------------------------------
+
+        We directly derive precedence graph nodes from the following
+        Nodes:
+
+        * Noteheads: empty, full, and grace noteheads of both kinds, which
+          are assigned duration based on their type (e.g., quarter, 16th, etc.)
+          and then may be further modified by duration dots and/or tuples.
+        * Rests of all kinds, which get duration via a simple table based
+          on the rest class and tuple/dot modification.
+        * Measure separators, which get a duration of 0.
+
+        The assumption of our symbol classes is that there are no rests
+        shorter than 64th.
+
+        Furthermore, we add synthetic nodes representing:
+
+        * Root measure separator, with duration 0 **and** onset 0,
+          which initializes the onset computations along the graph
+        * Measure nodes, with durations derived from time signatures
+          valid for the given measures.
+
+        Constructing the precedence graph
+        ---------------------------------
+
+        We factor the precedence graph into measures, and then infer precedence
+        for each measure separately, in order to keep the problem tractable
+        and in order for errors not to propagate too far. The inference
+        graph construction algorithm is therefore split into two steps:
+
+        * Construct the "spine" of the precedence graph from measure nodes,
+        * Construct the single-measure precedence subgraphs (further factored
+          by staff).
+
+        The difficulties lie primarily in step 2.
+
+        (Note that ties are currently disregarded: the second note
+        of the tie normally gets an onset. After all, conceptually,
+        it is a separate note with an onset, it just does not get played.)
+
+        Precedence graph spine
+        ^^^^^^^^^^^^^^^^^^^^^^
+
+        The **spine** of the precedence graph is a single path of alternating
+        ``measure_separator`` and ``measure`` nodes. ``measure_separator``
+        nodes are constructed from the Nodes, and ``measure`` nodes
+        are created artificially between consecutive ``measure_separator``
+        nodes. The measure separator nodes have a duration of 0, while
+        the duration of the measure nodes is inferred from the time signature
+        valid for that measure. An artificial root measure_separator node
+        is created to serve as the source of the entire precedence graph.
+
+        Thus, the first part of the algorithm is, at a high level:
+
+        * Order measure separators,
+        * Assign time signatures to measures and compute measure durations
+          from time signatures.
+
+        **Gory details:** In step 1, we assume that systems are ordered
+        top-down in time, that all systems are properly grouped using
+        ``staff_grouping`` symbols, that measure separators are strictly
+        monotonous (i.e., the same subset of possible onsets belongs to
+        the i-th measure on each staff, which is an assumption that does
+        *not* hold for isorhythmic motets and basically anything pre-16th
+        century).
+
+        In step 2, we assume that time signatures are always written within
+        the measure that *precedes* the first measure for which they are
+        valid, with the exception of the first time signature on the system.
+
+        We also currently assume that a given measure has the same number
+        of beats across all staves within a system (so: no polytempi for now).
+
+        Measure subgraphs
+        ^^^^^^^^^^^^^^^^^
+
+        There are again two high-level steps:
+
+        * Assign other onset-carrying objects (noteheads and rests)
+          to measures, to prepare the second phase that iterates over
+          these groups per measure (and staff).
+        * For each measure group, compute the subgraph and attach
+          its sources to the preceding measure separator node.
+
+        The first one can be resolved easily by looking at (a) staff
+        assignment, (b) horizontal position with respect to measure
+        separators. Noting that long measure separators might not
+        really be straight, we use the intersection of the separator
+        with the given staff.
+
+        The second step is the difficult one. We describe the algorithm
+        for inferring precedence, simultaneity span minimization,
+        in a separate section.
+
+
+        Simultaneity span minimization
+        ------------------------------
+
+        Inferring precedence in polyphonic music is non-trivial, especially
+        if one wants to handle handwritten music, and even more so when
+        extending the scope before the 1800s. We infer precedence using
+        the principle that notes which are supposed to be played together
+        should be as close to each other horizontally as possible: from
+        all the possible precedence assignments that fulfill notation
+        rule constraints, choose the one which minimizes the horizontal
+        span assigned to each unit of musical time in the bar.
+
+        The algorithm is initialized as follows:
+
+        * Determine the shortest subdivision of the measure (in beats)
+          which has to be treated independently. This generally corresponds
+          to the shortest note in the measure.
+        * Initialize the assignment table: for each onset-carrying object,
+          we will assign it to one of the time bins.
+
+        There are some rules of music notation that we use to prune the space
+        of possible precedence assignments by associating the notes (or rests)
+        into blocks:
+
+        * Beamed groups without intervening rests
+        * Tied note pairs
+        * Notes that share a stem
+        * Notes within a tuple
+
+        Rests within beamed groups (e.g., 8th - 8th_rest - 8th) are a problem.
+        A decision needs to be made whether the rest does belong to the group
+        or not.
+
+        """
+
+        if not self.measure_separators:
+            self._collect_symbols_for_pitch_inference(nodes)
+
+        measure_separators = [c for c in nodes
+                              if c.class_name in _CONST.MEASURE_SEPARATOR_CLASS_NAMES]
+
+        ######################################################################
+        # An important feature of measure-factorized onset inference
+        # instead of going left-to-right per part throughout is resistance
+        # to staves appearing & disappearing on line breaks (e.g. orchestral
+        # scores). Measures are (very, very often) points of synchronization
+        #  -- after all, that is their purpose.
+
+        # We currently DO NOT aim to process renaissance & medieval scores:
+        # especially motets may often have de-synchronized measure separators.
+
+        # Add the relationships between the measure separator nodes.
+        #  - Get staves to which the mseps are connected
+        msep_staffs = {m.id: self.children(m, [InferenceEngineConstants.STAFF])
+                       for m in measure_separators}
+        #  - Sort first by bottom-most staff to which the msep is connected
+        #    to get systems
+        #  - Sort left-to-right within systems to get final ordering of mseps
+        ordered_mseps = sorted(measure_separators,
+                               key=lambda m: (max([s.bottom
+                                                   for s in msep_staffs[m.id]]),
+                                              m.left))
+        ordered_msep_nodes = [PrecedenceGraphNode(node=m,
+                                                  inlinks=[],
+                                                  outlinks=[],
+                                                  onset=None,
+                                                  duration=0)
+                              for m in ordered_mseps]
+
+        # Add root node: like measure separator, but for the first measure.
+        # This one is the only one which is initialized with onset,
+        # with the value onset=0.
+        root_msep = PrecedenceGraphNode(objid=-1,
+                                        node=None,
+                                        inlinks=[], outlinks=[],
+                                        duration=0,
+                                        onset=0)
+
+        # Create measure bins. i-th measure ENDS at i-th ordered msep.
+        # We assume that every measure has a rightward separator.
+        measures = [(None, ordered_mseps[0])] + [(ordered_mseps[i], ordered_mseps[i + 1])
+                                                 for i in range(len(ordered_mseps) - 1)]
+        measure_nodes = [PrecedenceGraphNode(objid=None,
+                                             node=None,
+                                             inlinks=[root_msep],
+                                             outlinks=[ordered_msep_nodes[0]],
+                                             duration=0,  # Durations will be filled in
+                                             onset=None)] + \
+                        [PrecedenceGraphNode(objid=None,
+                                             node=None,
+                                             inlinks=[ordered_msep_nodes[i + 1]],
+                                             outlinks=[ordered_msep_nodes[i + 2]],
+                                             duration=0,  # Durations will be filled in
+                                             onset=None)
+                         for i in range(len(ordered_msep_nodes) - 2)]
+        #: A list of PrecedenceGraph nodes. These don't really need any Node
+        #  or id, they are just introducing through their duration the offsets
+        #  between measure separators (mseps have legit 0 duration, so that they
+        #  do not move the notes in their note descendants).
+        #  The list is already ordered.
+
+        # Add measure separator inlinks and outlinks.
+        for m_node in measure_nodes:
+            r_sep = m_node.outlinks[0]
+            r_sep.inliks.append(m_node)
+            if len(m_node.inlinks) > 0:
+                l_sep = m_node.inlinks[0]
+                l_sep.outlinks.append(m_node)
+
+        # Finally, hang the first measure on the root msep node.
+        root_msep.outlinks.append(measure_nodes[0])
+
+        ######################################################################
+        # Now, compute measure node durations from time signatures.
+        #  This is slightly non-trivial. Normally, a time signature is
+        #  (a) at the start of the staff, (b) right before the msep starting
+        #  the measure to which it should apply. However, sometimes the msep
+        #  comes up (c) at the *start* of the measure to which it should
+        #  apply. We IGNORE option (c) for now.
+        #
+        #  - Collect all time signatures
+        time_signatures = [c for c in nodes
+                           if c.class_name in _CONST.TIME_SIGNATURES]
+
+        #  - Assign time signatures to measure separators that *end*
+        #    the bars. (Because as opposed to the starting mseps,
+        #    the end mseps are (a) always there, (b) usually on the
+        #    same staff, (c) if not on the same staff, then they are
+        #    an anticipation at the end of a system, and will be repeated
+        #    at the beginning of the next one anyway.)
+        time_signatures_to_first_measure = {}
+        for t in time_signatures:
+            s = self.children(t, [InferenceEngineConstants.STAFF])[0]
+            # - Find the measure pairs
+            for i, (left_msep, right_msep) in enumerate(measures):
+                if s not in msep_staffs[right_msep.id]:
+                    continue
+                if (left_msep is None) or (s not in msep_staffs[left_msep.id]):
+                    # Beginning of system, valid already for the current bar.
+                    time_signatures_to_first_measure[t.id] = i
+                else:
+                    # Use i + 1, because the time signature is valid
+                    # for the *next* measure.
+                    time_signatures_to_first_measure[t.id] = i + 1
+
+        # - Interpret time signatures.
+        time_signature_durations = {t.id: self.interpret_time_signature(t)
+                                    for t in time_signatures}
+
+        # - Reverse map: for each measure, the time signature valid
+        #   for the measure.
+        measure_to_time_signature = [None for _ in measures]
+        time_signatures_sorted = sorted(time_signatures,
+                                        key=lambda x: time_signatures_to_first_measure[x.id])
+        for t1, t2 in zip(time_signatures_sorted[:-1], time_signatures_sorted[1:]):
+            affected_measures = list(range(time_signatures_to_first_measure[t1.id],
+                                           time_signatures_to_first_measure[t2.id]))
+            for i in affected_measures:
+                # Check for conflicting time signatures previously
+                # assigned to this measure.
+                if measure_to_time_signature[i] is not None:
+                    _competing_time_sig = measure_to_time_signature[i]
+                    if (time_signature_durations[t1.id] !=
+                            time_signature_durations[_competing_time_sig.id]):
+                        raise ValueError('Trying to overwrite time signature to measure'
+                                         ' assignment at measure {0}: new time sig'
+                                         ' {1} with value {2}, previous time sig {3}'
+                                         ' with value {4}'
+                                         ''.format(i, t1.id,
+                                                   time_signature_durations[t1.id],
+                                                   _competing_time_sig.id,
+                                                   time_signature_durations[_competing_time_sig.id]))
+
+                measure_to_time_signature[i] = t1
+
+        logging.debug('Checking that every measure has a time signature assigned.')
+        for i, (msep1, msep2) in enumerate(measures):
+            if measure_to_time_signature[i] is None:
+                raise ValueError('Measure without time signature: {0}, between'
+                                 'separators {1} and {2}'
+                                 ''.format(i, msep1.id, msep2.id))
+
+        # - Apply to each measure node the duration corresponding
+        #   to its time signature.
+        for i, m in enumerate(measure_nodes):
+            _tsig = measure_to_time_signature[i]
+            m.duration = time_signature_durations[_tsig.id]
+
+        # ...
+        # Now, the "skeleton" of the precedence graph consisting
+        # pf measure separator and measure nodes is complete.
+        ######################################################################
+
+        ######################################################################
+        # Collecting onset-carrying objects (at this point, noteheads
+        # and rests; the repeat-measure object that would normally
+        # affect duration is handled through measure node durations.
+        onset_objs = [c for c in nodes
+                      if c.class_name in _CONST.classes_bearing_duration]
+
+        # Assign onset-carrying objects to measures (their left msep).
+        # (This is *not* done by assigning outlinks to measure nodes,
+        # we are now just factorizing the space of possible precedence
+        # graphs.)
+        #  - This is done by iterating over staves.
+        staff_to_objs_map = collections.defaultdict(list)
+        for c in onset_objs:
+            ss = self.children(c, [InferenceEngineConstants.STAFF])
+            for s in ss:
+                staff_to_objs_map[s.id].append(c)
+
+        #  - Noteheads and rests are all connected to staves,
+        #    which immediately gives us for each staff the subset
+        #    of eligible symbols for each measure.
+        #  - We can just take the vertical projection of each onset
+        #    object and find out which measures it overlaps with.
+        #    To speed this up, we can just check whether the middles
+        #    of objects fall to the region delimited by the measure
+        #    separators. Note that sometimes the barlines making up
+        #    the measure separator are heavily bent, so it would
+        #    be prudent to perhaps use just the intersection of
+        #    the given barline and the current staff.
+
+        # Preparation: we need for each valid (staff, msep) combination
+        # the bounding box of their intersection, in order to deal with
+        # more curved measure separators.
+
+        msep_to_staff_projections = {}
+        #: For each measure separator, for each staff it connects to,
+        #  the bounding box of the measure separator's intersection with
+        #  that staff.
+        for msep in measure_separators:
+            msep_to_staff_projections[msep.id] = {}
+            for s in msep_staffs[msep.id]:
+                intersection_bbox = self.msep_staff_overlap_bbox(msep, s)
+                msep_to_staff_projections[msep.id][s.id] = intersection_bbox
+
+        staff_and_measure_to_objs_map = collections.defaultdict(
+            collections.defaultdict(list))
+        #: Per staff (indexed by id) and measure (by order no.), keeps a list of
+        #  Nodes from that staff that fall within that measure.
+
+        # Iterate over objects left to right, shift measure if next object
+        # over bound of current measure.
+        ordered_objs_per_staff = {s_objid: sorted(s_objs, key=lambda x: x.left)
+                                  for s_objid, s_objs in list(staff_to_objs_map.items())}
+        for s_objid, objs in list(ordered_objs_per_staff.items()):
+            # Vertically, we don't care -- the attachment to staff takes
+            # care of that, we only need horizontal placement.
+            _c_m_idx = 0  # Index of current measure
+            _c_msep_right = measure_nodes[_c_m_idx].outlinks[0]
+            # Left bound of current measure's right measure separator
+            _c_m_right = msep_to_staff_projections[_c_msep_right.id][s_objid][1]
+            for _c_o_idx, o in objs:
+                # If we are out of bounds, move to next measure
+                while o.left > _c_m_right:
+                    _c_m_idx += 1
+                    if _c_m_idx >= len(measure_nodes):
+                        raise ValueError('Object {0}: could not assign to any measure,'
+                                         ' ran out of measures!'.format(o.id))
+                    _c_msep_right = measure_nodes[_c_m_idx].outlinks[0]
+                    _c_m_right = msep_to_staff_projections[_c_msep_right.id][s_objid][1]
+                    staff_and_measure_to_objs_map[s_objid][_c_m_right] = []
+
+                staff_and_measure_to_objs_map[s_objid][_c_m_right].append(o)
+
+        # Infer precedence within the measure.
+        #  - This is the difficult part.
+        #  - First: check the *sum* of durations assigned to the measure
+        #    against the time signature. If it fits only once, then it is
+        #    a monophonic measure and we can happily read it left to right.
+        #  - If the measure is polyphonic, the fun starts!
+        #    With K graph nodes, how many prec. graphs are there?
+        for s_objid in staff_and_measure_to_objs_map:
+            for measure_idx in staff_and_measure_to_objs_map[s_objid]:
+                _c_objs = staff_and_measure_to_objs_map[s_objid][measure_idx]
+                measure_graph = self.measure_precedence_graph(_c_objs)
+
+                # Connect the measure graph source nodes to their preceding
+                # measure separator.
+                l_msep_node = measure_nodes[measure_idx].inlinks[0]
+                for source_node in measure_graph:
+                    l_msep_node.outlinks.append(source_node)
+                    source_node.inlinks.append(l_msep_node)
+
+        return [root_msep]
+
+    def measure_precedence_graph(self, nodes: List[Node]):
+        """Indexed by staff id and measure number, holds the precedence graph
+        for the given measure in the given staff as a list of PrecedenceGraphNode
+        objects that correspond to the source nodes of the precedence subgraph.
+        These nodes then get connected to their leftwards measure separator node.
+
+        :param nodes: List of Nodes, assumed to be all from one
+            measure.
+
+        :returns: A list of PrecedenceGraphNode objects that correspond
+            to the source nodes in the precedence graph for the (implied)
+            measure. (In monophonic music, the list will have one element.)
+            The rest of the measure precedence graph nodes is accessible
+            through the sources' outlinks.
+
+        """
+        _is_monody = self.is_measure_monody(nodes)
+        if _is_monody:
+            source_nodes = self.monody_measure_precedence_graph(nodes)
+            return source_nodes
+
+        else:
+            raise ValueError('Cannot deal with onsets in polyphonic music yet.')
+
+    def monody_measure_precedence_graph(self, nodes: List[Node]):
+        """Infers the precedence graph for a plain monodic measure.
+        The resulting structure is very simple: it's just a chain
+        of the onset-carrying objects from left to right."""
+        nodes = []
+        for c in sorted(nodes, key=lambda x: x.left):
+            potential_durations = self.beats(c)
+
+            # In monody, there should only be one duration
+            if len(potential_durations) > 1:
+                raise ValueError('Object {0}: More than one potential'
+                                 ' duration, even though the measure is'
+                                 ' determined to be monody.'.format(c.id))
+            duration = potential_durations[0]
+
+            node = PrecedenceGraphNode(objid=c.id,
+                                       node=c,
+                                       inlinks=[],
+                                       outlinks=[],
+                                       duration=duration,
+                                       onset=None)
+            nodes.append(node)
+        for n1, n2 in zip(nodes[:-1], nodes[1:]):
+            n1.outlinks.append(n2)
+            n2.inlinks.append(n1)
+        source_nodes = [nodes[0]]
+        return source_nodes
+
+    def is_measure_monody(self, nodes: List[Node]):
+        """Checks whether the given measure is written as simple monody:
+        no two of the onset-carrying objects are active simultaneously.
+
+        Assumptions
+        -----------
+
+        * Detecting monody without looking at the time signature:
+            * All stems in the same direction? --> NOPE: Violin chords in Bach...
+            * All stems in horizontally overlapping noteheads in the same direction?
+              --> NOPE: Again, violin chords in Bach...
+            * Overlapping noteheads share a beam, but not a stem? --> this works,
+              but has false negatives: overlapping quarter notes
+        """
+        raise NotImplementedError()
+
+    def is_measure_chord_monody(self, nodes: List[Node]):
+        """Checks whether the given measure is written as monody potentially
+        with chords. That is: same as monody, but once all onset-carrying objects
+        that share a stem are merged into an equivalence class."""
+        raise NotImplementedError()
+
+    def msep_staff_overlap_bbox(self, measure_separator, staff):
+        """Computes the bounding box for the part of the input
+        ``measure_separator`` that actually overlaps the ``staff``.
+        This is implemented to deal with mseps that curve a lot,
+        so that their left/right bounding box may mistakenly
+        exclude some symbols from their preceding/following measure.
+
+        Returns the (T, L, B, R) bounding box.
+        """
+        intersection = measure_separator.bounding_box_intersection(staff)
+        if intersection is None:
+            # Corner case: measure separator is connected to staff,
+            # but its bounding box does *not* overlap the bbox
+            # of the staff.
+            output_bbox = staff.top, measure_separator.left, \
+                          staff.bottom, measure_separator.right
+        else:
+            # The key step: instead of using the bounding
+            # box intersection, first crop the zeros from
+            # msep intersection mask (well, find out how
+            # many left and right zeros there are).
+            it, il, ib, ir = intersection
+            msep_crop = measure_separator.mask[it, il, ib, ir]
+
+            if msep_crop.sum() == 0:
+                # Corner case: bounding box does encompass staff,
+                # but there is msep foreground pixel in that area
+                # (could happen e.g. with mseps only drawn *around*
+                # staffs).
+                output_bbox = staff.top, measure_separator.left, \
+                              staff.bottom, measure_separator.right
+            else:
+                # The canonical case: measure separator across the staff.
+                msep_crop_vproj = msep_crop.sum(axis=0)
+                _dl = 0
+                _dr = 0
+                for i, v in enumerate(msep_crop_vproj):
+                    if v != 0:
+                        _dl = i
+                        break
+                for i in range(1, len(msep_crop_vproj)):
+                    if msep_crop_vproj[-i] != 0:
+                        _dr = i
+                        break
+                output_bbox = staff.top, measure_separator.left + _dl, \
+                              staff.bottom, measure_separator.right - _dr
+        return output_bbox
+
+    @staticmethod
+    def interpret_numerals(numerals: List[Node]) -> int:
+        """Returns the given numeral Node as a number, left to right."""
+        for n in numerals:
+            if n.class_name not in _CONST.NUMERALS:
+                raise ValueError('Symbol {0} is not a numeral!'.format(n.id))
+        n_str = ''.join([n.class_name[-1]
+                         for n in sorted(numerals, key=operator.attrgetter('left'))])
+        return int(n_str)
+
+    def interpret_time_signature(self, time_signature,
+                                 FRACTIONAL_VERTICAL_IOU_THRESHOLD=0.8):
+        """Converts the time signature into the beat count (in quarter
+        notes) it assigns to its following measures.
+
+        Dealing with numeric time signatures
+        ------------------------------------
+
+        * Is there both a numerator and a denominator?
+          (Is the time sig. "fractional"?)
+           * If there is a letter_other child, then yes; use the letter_other
+             symbol to separate time signature into numerator (top, left) and
+             denominator regions.
+           * If there is no letter_other child, then check if there is sufficient
+             vertical separation between some groups of symbols. Given that it
+             is much more likely that there will be the "fractional" structure,
+             we say:
+
+               If the minimum vertical IoU between two symbols is more than
+               0.8, we consider the time signature non-fractional.
+
+             (The threshold can be controlled through the
+             FRACTIONAL_VERTICAL_IOU_THRESHOLD parameter.)
+
+        * If yes: assign numerals to either num. (top), or denom. (bottom)
+        * If not: assume the number is no. of beats. (In some scores, the
+          base indicator may be attached in form of a note instead of a
+          denumerator, like e.g. scores by Janacek, but we ignore this for now.
+          In early music, 3 can mean "tripla", which is 3/2.)
+
+        Dealing with non-numeric time signatures
+        ----------------------------------------
+
+        * whole-time mark is interpreted as 4/4
+        * alla breve mark is interpreted as 4/4
+
+
+        :returns: The denoted duration of a measure in beats.
+        """
+        members = sorted(self.children(time_signature,
+                                       class_name_filter=_CONST.TIME_SIGNATURE_MEMBERS),
+                         key=lambda x: x.top)
+        logging.info('Interpreting time signature {0}'.format(time_signature.id))
+        logging.info('... Members {0}'.format([m.class_name for m in members]))
+
+        # Whole-time mark? Alla breve?
+        if len(members) == 0:
+            raise NotationGraphError('Time signature has no members: {0}'
+                                     ''.format(time_signature.id))
+
+        is_whole = False
+        is_alla_breve = False
+        for m in members:
+            if m.class_name == _CONST.TIME_SIG_COMMON:
+                is_whole = True
+            if m.class_name == _CONST.TIME_SIG_CUT_COMMON:
+                is_alla_breve = True
+
+        if is_whole or is_alla_breve:
+            logging.info('Time signature {0}: whole or alla breve, returning 4.0'
+                         ''.format(time_signature.id))
+            return 4.0
+
+        # Process numerals
+        logging.info('... Found numeric time signature, determining whether'
+                     ' it is fractional.')
+
+        # Does the time signature have a fraction-like format?
+        is_fraction_like = True
+        has_letter_other = (len([m for m in members if m.class_name == _CONST.LETTER_OTHER]) > 0)
+        #  - Does it have a separator slash?
+        if has_letter_other:
+            logging.info('... Has fraction slash')
+            is_fraction_like = True
+        #  - Does it have less than 2 members?
+        elif len(members) < 2:
+            logging.info('... Just one member')
+            is_fraction_like = False
+        #  - If it has 2 or more members, determine minimal IoU and compare
+        #    against FRACTIONAL_VERTICAL_IOU_THRESHOLD. If the minimal IoU
+        #    is under the threshold, then consider the numerals far apart
+        #    vertically so that they constitute a fraction.
+        else:
+            logging.info('... Must check for min. vertical overlap')
+            vertical_overlaps = []
+            for _i_m, m1 in enumerate(members[:-1]):
+                for m2 in members[_i_m:]:
+                    vertical_overlaps.append(bounding_box_dice_coefficient(m1.bounding_box, m2.bounding_box))
+            logging.info('... Vertical overlaps found: {0}'.format(vertical_overlaps))
+            if min(vertical_overlaps) < FRACTIONAL_VERTICAL_IOU_THRESHOLD:
+                is_fraction_like = True
+            else:
+                is_fraction_like = False
+
+        numerals = sorted(self.children(time_signature, _CONST.NUMERALS),
+                          key=lambda x: x.top)
+        if not is_fraction_like:
+            logging.info('... Non-fractional numeric time sig.')
+            # Read numeral left to right, this is the beat count
+            if len(numerals) == 0:
+                raise NotationGraphError('Time signature has no numerals, but is'
+                                         ' not fraction-like! {0}'
+                                         ''.format(time_signature.id))
+            beats = OnsetsInferenceEngine.interpret_numerals(numerals)
+            logging.info('... Beats: {0}'.format(beats))
+            return beats
+
+        else:
+            logging.info('... Fractional time sig.')
+            # Split into numerator and denominator
+            #  - Sort numerals top to bottom
+            #  - Find largest gap
+            #  - Everything above largest gap is numerator, everything below
+            #    is denominator.
+            numerals_topdown = sorted(numerals, key=lambda c: (c.top + c.bottom) / 2)
+            gaps = [((c2.bottom + c2.top) / 2) - ((c1.bottom + c2.top) / 2)
+                    for c1, c2 in zip(numerals_topdown[:-1], numerals_topdown[1:])]
+            largest_gap_idx = max(list(range(len(gaps))), key=lambda i: gaps[i]) + 1
+            numerator = numerals[:largest_gap_idx]
+            denominator = numerals[largest_gap_idx:]
+            beat_count = OnsetsInferenceEngine.interpret_numerals(numerator)
+            beat_units = OnsetsInferenceEngine.interpret_numerals(denominator)
+
+            beats = beat_count / (beat_units / 4)
+            logging.info('...signature : {0} / {1}, beats: {2}'
+                         ''.format(beat_count, beat_units, beats))
+
+            return beats
+
+    def onsets(self, nodes: List[Node]):
+        """Infers the onsets of notes in the given Nodes.
+
+        The onsets are measured in beats.
+
+        :returns: A id --> onset dict for all notehead-type
+            Nodes.
+        """
+        # We first find the precedence graph. (This is the hard
+        # part.)
+        # The precedence graph is a DAG structure of PrecedenceGraphNode
+        # objects. The infer_precedence() method returns a list
+        # of the graph's source nodes (of which there is in fact
+        # only one, the way it is currently defined).
+        precedence_graph = self.infer_precedence_from_annotations(nodes)
+        for node in precedence_graph:
+            node.onset = 0
+
+        # Once we have the precedence graph, we need to walk it.
+        # It is a DAG, so we simply do a BFS from each source.
+        # Whenever a node has more incoming predecessors,
+        # we need to wait until they are *all* resolved,
+        # and check whether they agree.
+        queue = []
+        # Note: the queue should be prioritized by *onset*, not number
+        # of links from initial node. Leades to trouble with unprocessed
+        # ancestors...
+        for node in precedence_graph:
+            if len(node.inlinks) == 0:
+                queue.append(node)
+
+        onsets = {}
+
+        logging.debug('Size of initial queue: {0}'.format(len(queue)))
+        logging.debug('Initial queue: {0}'.format([(q.obj.id, q.onset) for q in queue]))
+
+        # We will only be appending to the queue, so the
+        # start of the queue is defined simply by the index.
+        qstart = 0
+        delayed_prec_nodes = dict()
+        while (len(queue) - qstart) > 0:
+            # if len(queue) > 2 * n_prec_nodes:
+            #     logging.warning('Safety valve triggered: queue growing endlessly!')
+            #     break
+
+            q = queue[qstart]
+            logging.debug('Current @{0}: {1}'.format(qstart, q.obj.id))
+            logging.debug('Will add @{0}: {1}'.format(qstart, q.outlinks))
+
+            qstart += 1
+            for post_q in q.outlinks:
+                if post_q not in queue:
+                    queue.append(post_q)
+
+            logging.debug('Queue state: {0}'
+                          ''.format([ppq.obj.id for ppq in queue[qstart:]]))
+
+            logging.debug('  {0} has onset: {1}'.format(q.node_id, q.onset))
+            if q.onset is not None:
+                if q.onset > 0:
+                    break
+                onsets[q.obj.id] = q.onset
+                continue
+
+            prec_qs = q.inlinks
+            prec_onsets = [pq.onset for pq in prec_qs]
+            # If the node did not yet get all its ancestors processed,
+            # send it down the queue.
+            if None in prec_onsets:
+                logging.warning('Found node with predecessor that has no onset yet; delaying processing: {0}'
+                                ''.format(q.obj.id))
+                queue.append(q)
+                if q in delayed_prec_nodes:
+                    logging.warning('This node has already been delayed once! Breaking.')
+                    logging.warning('Queue state: {0}'
+                                    ''.format([ppq.obj.id for ppq in queue[qstart:]]))
+                    break
+                else:
+                    delayed_prec_nodes[q.obj.id] = q
+                    continue
+
+            prec_durations = [pq.duration for pq in prec_qs]
+
+            logging.debug('    Prec_onsets @{0}: {1}'.format(qstart - 1, prec_onsets))
+            logging.debug('    Prec_durations @{0}: {1}'.format(qstart - 1, prec_durations))
+
+            onset_proposals = [o + d for o, d in zip(prec_onsets, prec_durations)]
+            if min(onset_proposals) != max(onset_proposals):
+                if self.strategy.permissive_desynchronization:
+                    logging.warning('Object {0}: onsets not synchronized from'
+                                    ' predecessors: {1}'.format(q.obj.id,
+                                                                onset_proposals))
+                    onset = max(onset_proposals)
+                else:
+                    raise ValueError('Object {0}: onsets not synchronized from'
+                                     ' predecessors: {1}'.format(q.obj.id,
+                                                                 onset_proposals))
+            else:
+                onset = onset_proposals[0]
+
+            q.onset = onset
+            # Some nodes do not have a Node assigned.
+            if q.obj is not None:
+                onsets[q.obj.id] = onset
+                ### DEBUG -- add this to the Data dict
+                q.obj.data['onset_beats'] = onset
+
+        return onsets
+
+    def children(self, c, class_name_filter: List[str] = None):
+        """Retrieve the children of the given Node ``c``
+        that have class in ``clsnames``."""
+        if class_name_filter is None:
+            return [self.id_to_node_mapping[o] for o in c.outlinks]
+        else:
+            return [self.id_to_node_mapping[o] for o in c.outlinks
+                    if self.id_to_node_mapping[o].class_name in class_name_filter]
+
+    def __parents(self, c, clsnames: List[str]):
+        """Retrieve the parents of the given Node ``c``
+        that have class in ``clsnames``."""
+        return [self.id_to_node_mapping[i] for i in c.inlinks
+                if self.id_to_node_mapping[i].class_name in clsnames]
+
+    def __warning_or_error(self, message):
+        if self.strategy.permissive:
+            logging.warning(message)
+        else:
+            raise ValueError(message)
+
+    def process_ties(self, nodes: List[Node], durations, onsets):
+        """Modifies the durations and onsets so that ties are taken into
+        account.
+
+        Every left-hand note in a tie gets its duration extended by the
+        right-hand note's duration. Every right-hand note's onset is removed.
+
+        :returns: the modified durations and onsets.
+        """
+        logging.info('Processing ties...')
+        g = NotationGraph(nodes=nodes)
+
+        def __get_tie_notes(_tie, graph):
+            notes = graph.parents(_tie,
+                                  class_filter=[_CONST.NOTEHEAD_FULL, _CONST.NOTEHEAD_HALF, _CONST.NOTEHEAD_WHOLE])
+            if len(notes) == 0:
+                raise NotationGraphError('No notes from tie {0}'.format(_tie.id))
+            if len(notes) == 1:
+                return [notes[0]]
+            if len(notes) > 2:
+                raise NotationGraphError('More than two notes from tie {0}'.format(_tie.id))
+            # Now it has to be 2
+            l, r = sorted(notes, key=lambda n: n.left)
+            return l, r
+
+        def _is_note_left(c, _tie, graph):
+            tie_notes = __get_tie_notes(_tie, graph)
+            if len(tie_notes) == 2:
+                l, r = tie_notes
+                return l.id == c.id
+            else:
+                return True
+
+        new_onsets = copy.deepcopy(onsets)
+        new_durations = copy.deepcopy(durations)
+        # Sorting notes right to left. This means: for notes in the middle
+        # of two ties, its duration is already updated and it can be removed from
+        # the new onsets dict by the time we process the note on the left
+        # of the leftward tie (its predecessor).
+        for k in sorted(onsets, key=lambda x: onsets[x], reverse=True):
+            ties = g.children(k, class_filter=[_CONST.TIE_CLASS_NAME])
+            if len(ties) == 0:
+                continue
+
+            if len(ties) > 1:
+                # Pick the rightmost tie (we're processing onsets from the right)
+                tie = max(ties, key=lambda x: x.left)
+            else:
+                tie = ties[0]
+            n = g[k]
+            tie_notes = __get_tie_notes(tie, graph=g)
+            if len(tie_notes) != 2:
+                continue
+
+            l, r = tie_notes
+            if l.id == n.id:
+                logging.info('Note {0} is left in tie {1}'
+                             ''.format(l.id, tie.id))
+                new_durations[l.id] += new_durations[r.id]
+                del new_onsets[r.id]
+
+        new_durations = {k: new_durations[k] for k in new_onsets}
+        return new_durations, new_onsets
+
+
+class PrecedenceGraphNode(object):
+    """A helper plain-old-data class for onset extraction.
+    The ``inlinks`` and ``outlinks`` attributes are lists
+    of other ``PrecedenceGraphNode`` instances.
+    """
+
+    def __init__(self, objid=None, node: Node = None, inlinks: List[int] = None, outlinks: List[int] = None,
+                 onset=None, duration=0):
+        # Optional link to Nodes, or just a placeholder ID.
+        self.obj = node
+        if objid is None and node is not None:
+            objid = node.id
+        self.node_id = objid
+
+        self.inlinks = []
+        if inlinks:
+            self.inlinks = inlinks
+        self.outlinks = []
+        if outlinks:
+            self.outlinks = outlinks
+
+        self.onset = onset
+        '''Counting from the start of the musical sequence, how many
+        beat units pass before this object?'''
+
+        self.duration = duration
+        '''By how much musical time does the object delay the onsets
+        of its descendants in the precedence graph?'''
+
+        self.data = node.data
```

### Comparing `mung-1.1/scripts/add_staff_relationships.py` & `mung-1.2/scripts/add_staff_relationships.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,333 +1,333 @@
-"""The ``add_staff_relationships.py`` script automates adding
-the relationships of some staff-related symbols to staffs.
-"""
-import argparse
-import collections
-import logging
-import os
-import pprint
-import time
-
-from typing import List
-from collections import defaultdict
-from mung.constants import InferenceEngineConstants as _CONST
-from mung.io import read_nodes_from_file, export_node_list
-from mung.node import link_nodes, Node
-
-
-def add_staff_relationships(nodes: List[Node],
-                            notehead_staffspace_threshold: float = 0.2) -> List[Node]:
-    id_to_node_mapping = {node.id: node for node in nodes}
-
-    ON_STAFFLINE_RATIO_THRESHOLD = notehead_staffspace_threshold
-
-    ##########################################################################
-    logging.info('Find the staff-related symbols')
-    staffs = [c for c in nodes if c.class_name == _CONST.STAFF_CLASS_NAME]
-
-    staff_related_symbols = defaultdict(list)  # type: defaultdict[str, List[Node]]
-    notehead_symbols = defaultdict(list)  # type: defaultdict[str, List[Node]]
-    rest_symbols = defaultdict(list)  # type: defaultdict[str, List[Node]]
-    for node in nodes:
-        if node.class_name in _CONST.STAFF_RELATED_CLASS_NAMES:
-            staff_related_symbols[node.class_name].append(node)
-        if node.class_name in _CONST.NOTEHEAD_CLASS_NAMES:
-            notehead_symbols[node.class_name].append(node)
-        if node.class_name in _CONST.REST_CLASS_NAMES:
-            rest_symbols[node.class_name].append(node)
-
-    ##########################################################################
-    logging.info('Adding staff relationships')
-    #  - Which direction do the relationships lead in?
-    #    Need to define this.
-    #
-    # Staff -> symbol?
-    # Symbol -> staff?
-    # It does not really matter, but it's more intuitive to attach symbols
-    # onto a pre-existing staff. So, symbol -> staff.
-    for class_name, nodes in list(staff_related_symbols.items()):
-        for node in nodes:  # type: Node
-            # Find the related staff. Relatedness is measured by row overlap.
-            # That means we have to modify the staff bounding box to lead
-            # from the leftmost to the rightmost column. This holds
-            # especially for the staff_grouping symbols.
-            for staff in staffs:
-                top, left, bottom, right = staff.bounding_box
-                left = 0
-                right = max(right, node.right)
-                if node.overlaps((top, left, bottom, right)):
-                    link_nodes(node, staff)
-
-    ##########################################################################
-    logging.info('Adding rest --> staff relationships.')
-    for class_name, nodes in list(rest_symbols.items()):
-        for node in nodes:  # type: Node
-            closest_staff = min([s for s in staffs],
-                                key=lambda x: ((x.bottom + x.top) / 2. - (node.bottom + node.top) / 2.) ** 2)
-            link_nodes(node, closest_staff)
-
-    ##########################################################################
-    logging.info('Adding notehead relationships.')
-
-    # NOTE:
-    # This part should NOT rely on staffspace masks in any way!
-    # They are highly unreliable.
-
-    # Sort the staff objects top-down. Assumes stafflines do not cross,
-    # and that there are no crazy curves at the end that would make the lower
-    # stafflines stick out over the ones above them...
-    stafflines = [c for c in nodes if c.class_name == _CONST.STAFFLINE_CLASS_NAME]
-    stafflines = sorted(stafflines, key=lambda c: c.top)
-    staffspaces = [c for c in nodes if c.class_name == _CONST.STAFFSPACE_CLASS_NAME]
-    staffspaces = sorted(staffspaces, key=lambda c: c.top)
-    staves = [c for c in nodes if c.class_name == _CONST.STAFF_CLASS_NAME]
-    staves = sorted(staves, key=lambda c: c.top)
-
-    # Indexing data structures.
-    #
-    # We need to know:
-    #  - per staffline and staffspace: its containing staff
-    _staff_per_ss_sl = {}
-    #  - per staffline and staffspace: its index (top to bottom) within the staff
-    _ss_sl_idx_wrt_staff = {}
-    # Reverse indexes:
-    # If I know which staff (by id) and which index of staffline/staffspace,
-    # I want to retrieve the given staffline/staffspace Node:
-    _staff_and_idx2ss = defaultdict(dict)
-    _staff_and_idx2sl = defaultdict(dict)
-
-    # Build the indexes
-    for _staff in staves:
-        # Keep the top-down ordering from above:
-        _s_stafflines = [_staffline for _staffline in stafflines
-                         if _staff.id in _staffline.inlinks]
-        _s_staffspaces = [_staffspace for _staffspace in staffspaces
-                          if _staff.id in _staffspace.inlinks]
-        for i, _sl in enumerate(_s_stafflines):
-            _staff_per_ss_sl[_sl.id] = _staff
-            _ss_sl_idx_wrt_staff[_sl.id] = i
-            _staff_and_idx2sl[_staff.id][i] = _sl
-            logging.debug('Staff {0}: stafflines {1}'.format(_staff.id,
-                                                             _staff_and_idx2sl[_staff.id]))
-        for i, _ss in enumerate(_s_staffspaces):
-            _staff_per_ss_sl[_ss.id] = _staff
-            _ss_sl_idx_wrt_staff[_ss.id] = i
-            _staff_and_idx2ss[_staff.id][i] = _ss
-
-    logging.debug(pprint.pformat(dict(_staff_and_idx2ss)))
-
-    for class_name, nodes in list(notehead_symbols.items()):
-        for node in nodes:
-
-            ct, cl, cb, cr = node.bounding_box
-
-            ################
-            # Add relationship to given staffline or staffspace.
-
-            # If notehead has leger lines, skip it for now.
-            has_leger_line = False
-            for o in node.outlinks:
-                if id_to_node_mapping[o].class_name == _CONST.LEGER_LINE_CLASS_NAME:
-                    has_leger_line = True
-                    break
-
-            if has_leger_line:
-                # Attach to the appropriate staff:
-                # meaning, staff closest to the innermost leger line.
-                lls = [id_to_node_mapping[o] for o in node.outlinks
-                       if id_to_node_mapping[o].class_name == _CONST.LEGER_LINE_CLASS_NAME]
-                # Furthest from notehead's top is innermost.
-                # (If notehead is below staff and crosses a ll., one
-                #  of these numbers will be negative. But that doesn't matter.)
-                ll_max_dist = max(lls, key=lambda ll: ll.top - node.top)
-                # Find closest staff to max-dist leger ine
-                staff_min_dist = min(staves,
-                                     key=lambda ss: min((ll_max_dist.bottom - ss.top) ** 2,
-                                                        (ll_max_dist.top - ss.bottom) ** 2))
-                link_nodes(node, staff_min_dist)
-                continue
-
-            # - Find the related staffline.
-            # - Because of curved stafflines, this has to be done w.r.t.
-            #   the horizontal position of the notehead.
-            # - Also, because stafflines are NOT filled in (they do not have
-            #   intersections annotated), it is necessary to use a wider
-            #   window than just the notehead.
-            # - We will assume that STAFFLINES DO NOT CROSS.
-            #   (That is a reasonable assumption.)
-            #
-            # - For now, we only work with more or less straight stafflines.
-
-            overlapped_stafflines = []
-            overlapped_staffline_idxs = []
-            for i, staff in enumerate(stafflines):
-                # This is the assumption of straight stafflines!
-                if (ct <= staff.top <= cb) or (ct <= staff.bottom <= cb):
-                    overlapped_stafflines.append(staff)
-                    overlapped_staffline_idxs.append(i)
-
-            if node.id < 10:
-                logging.debug('Notehead {0} ({1}): overlaps {2} stafflines'.format(node.id,
-                                                                                   node.bounding_box,
-                                                                                   len(overlapped_stafflines), ))
-
-            if len(overlapped_stafflines) == 1:
-                staff = overlapped_stafflines[0]
-                dtop = staff.top - ct
-                dbottom = cb - staff.bottom
-                if min(dtop, dbottom) / max(dtop, dbottom) < ON_STAFFLINE_RATIO_THRESHOLD:
-                    logging.info('Notehead {0}, staffline {1}: very small ratio {2:.2f}'
-                                 ''.format(node.id, staff.id,
-                                           min(dtop, dbottom) / max(dtop, dbottom)))
-                    # Staffspace?
-                    #
-                    # To get staffspace:
-                    #  - Get orientation (below? above?)
-                    _is_staffspace_above = False
-                    if dtop > dbottom:
-                        _is_staffspace_above = True
-
-                    #  - Find staffspaces adjacent to the overlapped staffline.
-                    # NOTE: this will fail with single-staffline staves, because
-                    #       they do NOT have the surrounding staffspaces defined...
-                    _staffline_idx_wrt_staff = _ss_sl_idx_wrt_staff[staff.id]
-                    if _is_staffspace_above:
-                        _staffspace_idx_wrt_staff = _staffline_idx_wrt_staff
-                    else:
-                        _staffspace_idx_wrt_staff = _staffline_idx_wrt_staff + 1
-
-                    # Retrieve the given staffsapce
-                    _staff = _staff_per_ss_sl[staff.id]
-                    tgt_staffspace = _staff_and_idx2ss[_staff.id][_staffspace_idx_wrt_staff]
-                    # Link to staffspace
-                    link_nodes(node, tgt_staffspace)
-                    # And link to staff
-                    _c_staff = _staff_per_ss_sl[tgt_staffspace.id]
-                    link_nodes(node, _c_staff)
-
-                else:
-                    # Staffline!
-                    link_nodes(node, staff)
-                    # And staff:
-                    _c_staff = _staff_per_ss_sl[staff.id]
-                    link_nodes(node, _c_staff)
-
-            elif len(overlapped_stafflines) == 0:
-                # Staffspace!
-                # Link to the staffspace with which the notehead has
-                # greatest vertical overlap.
-                #
-                # Interesting corner case:
-                # Sometimes noteheads "hang out" of the upper/lower
-                # staffspace, so they are not entirely covered.
-                overlapped_staffspaces = {}
-                for _ss_i, staff in enumerate(staffspaces):
-                    if staff.top <= node.top <= staff.bottom:
-                        overlapped_staffspaces[_ss_i] = min(staff.bottom, node.bottom) - node.top
-                    elif node.top <= staff.top <= node.bottom:
-                        overlapped_staffspaces[_ss_i] = staff.bottom - max(node.top, staff.top)
-
-                if len(overlapped_staffspaces) == 0:
-                    logging.warning('Notehead {0}: no overlapped staffline object, no leger line!'
-                                    ''.format(node.id))
-                _ss_i_max = max(list(overlapped_staffspaces.keys()),
-                                key=lambda x: overlapped_staffspaces[x])
-                max_overlap_staffspace = staffspaces[_ss_i_max]
-                link_nodes(node, max_overlap_staffspace)
-                _c_staff = _staff_per_ss_sl[max_overlap_staffspace.id]
-                link_nodes(node, _c_staff)
-
-            elif len(overlapped_stafflines) == 2:
-                # Staffspace between those two lines.
-                s1 = overlapped_stafflines[0]
-                s2 = overlapped_stafflines[1]
-
-                _staff1 = _staff_per_ss_sl[s1.id]
-                _staff2 = _staff_per_ss_sl[s2.id]
-                if _staff1.id != _staff2.id:
-                    raise ValueError('Really weird notehead overlapping two stafflines'
-                                     ' from two different staves: {0}'.format(node.id))
-
-                _staffspace_idx = _ss_sl_idx_wrt_staff[s2.id]
-                staff = _staff_and_idx2ss[_staff2.id][_staffspace_idx]
-                link_nodes(node, staff)
-                # And link to staff:
-                _c_staff = _staff_per_ss_sl[staff.id]
-                link_nodes(node, _c_staff)
-
-            elif len(overlapped_stafflines) > 2:
-                raise ValueError('Really weird notehead overlapping more than 2 stafflines:'
-                                 ' {0}'.format(node.id))
-
-    return nodes
-
-
-###############################################################################
-
-
-def build_argument_parser():
-    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-
-    parser.add_argument('-a', '--annot', action='store', required=True,
-                        help='The annotation file for which the staffline and staff'
-                             ' Node relationships should be added.')
-    parser.add_argument('-e', '--export', action='store',
-                        help='A filename to which the output Nodes'
-                             ' should be saved. If not given, will print to'
-                             ' stdout.')
-
-    parser.add_argument('-t', '--notehead_staffspace_threshold', action='store', type=float,
-                        default=0.2,
-                        help='If the ratio of the smaller to the larger lobe w.r.t.'
-                             ' an overlapped staffline is lower than this, we consider'
-                             ' the notehead to belong to the adjacent staffspace.')
-
-    parser.add_argument('-v', '--verbose', action='store_true',
-                        help='Turn on INFO messages.')
-    parser.add_argument('--debug', action='store_true',
-                        help='Turn on DEBUG messages.')
-
-    return parser
-
-
-def main(args):
-    logging.info('Starting main...')
-    _start_time = time.clock()
-
-    ##########################################################################
-    logging.info('Import the Node list')
-    if not os.path.isfile(args.annot):
-        raise ValueError('Annotation file {0} not found!'
-                         ''.format(args.annot))
-    nodes = read_nodes_from_file(args.annot)
-
-    output_nodes = add_staff_relationships(
-        nodes,
-        notehead_staffspace_threshold=args.notehead_staffspace_threshold)
-
-    ##########################################################################
-    logging.info('Export the combined list.')
-    nodes_string = export_node_list(output_nodes)
-
-    if args.export is not None:
-        with open(args.export, 'w') as hdl:
-            hdl.write(nodes_string)
-    else:
-        print(nodes_string)
-
-    _end_time = time.clock()
-    logging.info('add_staff_reationships.py done in {0:.3f} s'
-                 ''.format(_end_time - _start_time))
-
-
-if __name__ == '__main__':
-    parser = build_argument_parser()
-    args = parser.parse_args()
-
-    if args.verbose:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
-    if args.debug:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
-
-    main(args)
+"""The ``add_staff_relationships.py`` script automates adding
+the relationships of some staff-related symbols to staffs.
+"""
+import argparse
+import collections
+import logging
+import os
+import pprint
+import time
+
+from typing import List
+from collections import defaultdict
+from mung.constants import InferenceEngineConstants as _CONST
+from mung.io import read_nodes_from_file, export_node_list
+from mung.node import link_nodes, Node
+
+
+def add_staff_relationships(nodes: List[Node],
+                            notehead_staffspace_threshold: float = 0.2) -> List[Node]:
+    id_to_node_mapping = {node.id: node for node in nodes}
+
+    ON_STAFFLINE_RATIO_THRESHOLD = notehead_staffspace_threshold
+
+    ##########################################################################
+    logging.info('Find the staff-related symbols')
+    staffs = [c for c in nodes if c.class_name == _CONST.STAFF]
+
+    staff_related_symbols = defaultdict(list)  # type: defaultdict[str, List[Node]]
+    notehead_symbols = defaultdict(list)  # type: defaultdict[str, List[Node]]
+    rest_symbols = defaultdict(list)  # type: defaultdict[str, List[Node]]
+    for node in nodes:
+        if node.class_name in _CONST.STAFF_RELATED_CLASS_NAMES:
+            staff_related_symbols[node.class_name].append(node)
+        if node.class_name in _CONST.NOTEHEAD_CLASS_NAMES:
+            notehead_symbols[node.class_name].append(node)
+        if node.class_name in _CONST.REST_CLASS_NAMES:
+            rest_symbols[node.class_name].append(node)
+
+    ##########################################################################
+    logging.info('Adding staff relationships')
+    #  - Which direction do the relationships lead in?
+    #    Need to define this.
+    #
+    # Staff -> symbol?
+    # Symbol -> staff?
+    # It does not really matter, but it's more intuitive to attach symbols
+    # onto a pre-existing staff. So, symbol -> staff.
+    for class_name, nodes in list(staff_related_symbols.items()):
+        for node in nodes:  # type: Node
+            # Find the related staff. Relatedness is measured by row overlap.
+            # That means we have to modify the staff bounding box to lead
+            # from the leftmost to the rightmost column. This holds
+            # especially for the staff_grouping symbols.
+            for staff in staffs:
+                top, left, bottom, right = staff.bounding_box
+                left = 0
+                right = max(right, node.right)
+                if node.overlaps((top, left, bottom, right)):
+                    link_nodes(node, staff)
+
+    ##########################################################################
+    logging.info('Adding rest --> staff relationships.')
+    for class_name, nodes in list(rest_symbols.items()):
+        for node in nodes:  # type: Node
+            closest_staff = min([s for s in staffs],
+                                key=lambda x: ((x.bottom + x.top) / 2. - (node.bottom + node.top) / 2.) ** 2)
+            link_nodes(node, closest_staff)
+
+    ##########################################################################
+    logging.info('Adding notehead relationships.')
+
+    # NOTE:
+    # This part should NOT rely on staffspace masks in any way!
+    # They are highly unreliable.
+
+    # Sort the staff objects top-down. Assumes stafflines do not cross,
+    # and that there are no crazy curves at the end that would make the lower
+    # stafflines stick out over the ones above them...
+    stafflines = [c for c in nodes if c.class_name == _CONST.STAFFLINE]
+    stafflines = sorted(stafflines, key=lambda c: c.top)
+    staffspaces = [c for c in nodes if c.class_name == _CONST.STAFFSPACE]
+    staffspaces = sorted(staffspaces, key=lambda c: c.top)
+    staves = [c for c in nodes if c.class_name == _CONST.STAFF]
+    staves = sorted(staves, key=lambda c: c.top)
+
+    # Indexing data structures.
+    #
+    # We need to know:
+    #  - per staffline and staffspace: its containing staff
+    _staff_per_ss_sl = {}
+    #  - per staffline and staffspace: its index (top to bottom) within the staff
+    _ss_sl_idx_wrt_staff = {}
+    # Reverse indexes:
+    # If I know which staff (by id) and which index of staffline/staffspace,
+    # I want to retrieve the given staffline/staffspace Node:
+    _staff_and_idx2ss = defaultdict(dict)
+    _staff_and_idx2sl = defaultdict(dict)
+
+    # Build the indexes
+    for _staff in staves:
+        # Keep the top-down ordering from above:
+        _s_stafflines = [_staffline for _staffline in stafflines
+                         if _staff.id in _staffline.inlinks]
+        _s_staffspaces = [_staffspace for _staffspace in staffspaces
+                          if _staff.id in _staffspace.inlinks]
+        for i, _sl in enumerate(_s_stafflines):
+            _staff_per_ss_sl[_sl.id] = _staff
+            _ss_sl_idx_wrt_staff[_sl.id] = i
+            _staff_and_idx2sl[_staff.id][i] = _sl
+            logging.debug('Staff {0}: stafflines {1}'.format(_staff.id,
+                                                             _staff_and_idx2sl[_staff.id]))
+        for i, _ss in enumerate(_s_staffspaces):
+            _staff_per_ss_sl[_ss.id] = _staff
+            _ss_sl_idx_wrt_staff[_ss.id] = i
+            _staff_and_idx2ss[_staff.id][i] = _ss
+
+    logging.debug(pprint.pformat(dict(_staff_and_idx2ss)))
+
+    for class_name, nodes in list(notehead_symbols.items()):
+        for node in nodes:
+
+            ct, cl, cb, cr = node.bounding_box
+
+            ################
+            # Add relationship to given staffline or staffspace.
+
+            # If notehead has leger lines, skip it for now.
+            has_leger_line = False
+            for o in node.outlinks:
+                if id_to_node_mapping[o].class_name == _CONST.LEGER_LINE:
+                    has_leger_line = True
+                    break
+
+            if has_leger_line:
+                # Attach to the appropriate staff:
+                # meaning, staff closest to the innermost leger line.
+                lls = [id_to_node_mapping[o] for o in node.outlinks
+                       if id_to_node_mapping[o].class_name == _CONST.LEGER_LINE]
+                # Furthest from notehead's top is innermost.
+                # (If notehead is below staff and crosses a ll., one
+                #  of these numbers will be negative. But that doesn't matter.)
+                ll_max_dist = max(lls, key=lambda ll: ll.top - node.top)
+                # Find closest staff to max-dist leger ine
+                staff_min_dist = min(staves,
+                                     key=lambda ss: min((ll_max_dist.bottom - ss.top) ** 2,
+                                                        (ll_max_dist.top - ss.bottom) ** 2))
+                link_nodes(node, staff_min_dist)
+                continue
+
+            # - Find the related staffline.
+            # - Because of curved stafflines, this has to be done w.r.t.
+            #   the horizontal position of the notehead.
+            # - Also, because stafflines are NOT filled in (they do not have
+            #   intersections annotated), it is necessary to use a wider
+            #   window than just the notehead.
+            # - We will assume that STAFFLINES DO NOT CROSS.
+            #   (That is a reasonable assumption.)
+            #
+            # - For now, we only work with more or less straight stafflines.
+
+            overlapped_stafflines = []
+            overlapped_staffline_idxs = []
+            for i, staff in enumerate(stafflines):
+                # This is the assumption of straight stafflines!
+                if (ct <= staff.top <= cb) or (ct <= staff.bottom <= cb):
+                    overlapped_stafflines.append(staff)
+                    overlapped_staffline_idxs.append(i)
+
+            if node.id < 10:
+                logging.debug('Notehead {0} ({1}): overlaps {2} stafflines'.format(node.id,
+                                                                                   node.bounding_box,
+                                                                                   len(overlapped_stafflines), ))
+
+            if len(overlapped_stafflines) == 1:
+                staff = overlapped_stafflines[0]
+                dtop = staff.top - ct
+                dbottom = cb - staff.bottom
+                if min(dtop, dbottom) / max(dtop, dbottom) < ON_STAFFLINE_RATIO_THRESHOLD:
+                    logging.info('Notehead {0}, staffline {1}: very small ratio {2:.2f}'
+                                 ''.format(node.id, staff.id,
+                                           min(dtop, dbottom) / max(dtop, dbottom)))
+                    # Staffspace?
+                    #
+                    # To get staffspace:
+                    #  - Get orientation (below? above?)
+                    _is_staffspace_above = False
+                    if dtop > dbottom:
+                        _is_staffspace_above = True
+
+                    #  - Find staffspaces adjacent to the overlapped staffline.
+                    # NOTE: this will fail with single-staffline staves, because
+                    #       they do NOT have the surrounding staffspaces defined...
+                    _staffline_idx_wrt_staff = _ss_sl_idx_wrt_staff[staff.id]
+                    if _is_staffspace_above:
+                        _staffspace_idx_wrt_staff = _staffline_idx_wrt_staff
+                    else:
+                        _staffspace_idx_wrt_staff = _staffline_idx_wrt_staff + 1
+
+                    # Retrieve the given staffsapce
+                    _staff = _staff_per_ss_sl[staff.id]
+                    tgt_staffspace = _staff_and_idx2ss[_staff.id][_staffspace_idx_wrt_staff]
+                    # Link to staffspace
+                    link_nodes(node, tgt_staffspace)
+                    # And link to staff
+                    _c_staff = _staff_per_ss_sl[tgt_staffspace.id]
+                    link_nodes(node, _c_staff)
+
+                else:
+                    # Staffline!
+                    link_nodes(node, staff)
+                    # And staff:
+                    _c_staff = _staff_per_ss_sl[staff.id]
+                    link_nodes(node, _c_staff)
+
+            elif len(overlapped_stafflines) == 0:
+                # Staffspace!
+                # Link to the staffspace with which the notehead has
+                # greatest vertical overlap.
+                #
+                # Interesting corner case:
+                # Sometimes noteheads "hang out" of the upper/lower
+                # staffspace, so they are not entirely covered.
+                overlapped_staffspaces = {}
+                for _ss_i, staff in enumerate(staffspaces):
+                    if staff.top <= node.top <= staff.bottom:
+                        overlapped_staffspaces[_ss_i] = min(staff.bottom, node.bottom) - node.top
+                    elif node.top <= staff.top <= node.bottom:
+                        overlapped_staffspaces[_ss_i] = staff.bottom - max(node.top, staff.top)
+
+                if len(overlapped_staffspaces) == 0:
+                    logging.warning('Notehead {0}: no overlapped staffline object, no leger line!'
+                                    ''.format(node.id))
+                _ss_i_max = max(list(overlapped_staffspaces.keys()),
+                                key=lambda x: overlapped_staffspaces[x])
+                max_overlap_staffspace = staffspaces[_ss_i_max]
+                link_nodes(node, max_overlap_staffspace)
+                _c_staff = _staff_per_ss_sl[max_overlap_staffspace.id]
+                link_nodes(node, _c_staff)
+
+            elif len(overlapped_stafflines) == 2:
+                # Staffspace between those two lines.
+                s1 = overlapped_stafflines[0]
+                s2 = overlapped_stafflines[1]
+
+                _staff1 = _staff_per_ss_sl[s1.id]
+                _staff2 = _staff_per_ss_sl[s2.id]
+                if _staff1.id != _staff2.id:
+                    raise ValueError('Really weird notehead overlapping two stafflines'
+                                     ' from two different staves: {0}'.format(node.id))
+
+                _staffspace_idx = _ss_sl_idx_wrt_staff[s2.id]
+                staff = _staff_and_idx2ss[_staff2.id][_staffspace_idx]
+                link_nodes(node, staff)
+                # And link to staff:
+                _c_staff = _staff_per_ss_sl[staff.id]
+                link_nodes(node, _c_staff)
+
+            elif len(overlapped_stafflines) > 2:
+                raise ValueError('Really weird notehead overlapping more than 2 stafflines:'
+                                 ' {0}'.format(node.id))
+
+    return nodes
+
+
+###############################################################################
+
+
+def build_argument_parser():
+    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+
+    parser.add_argument('-a', '--annot', action='store', required=True,
+                        help='The annotation file for which the staffline and staff'
+                             ' Node relationships should be added.')
+    parser.add_argument('-e', '--export', action='store',
+                        help='A filename to which the output Nodes'
+                             ' should be saved. If not given, will print to'
+                             ' stdout.')
+
+    parser.add_argument('-t', '--notehead_staffspace_threshold', action='store', type=float,
+                        default=0.2,
+                        help='If the ratio of the smaller to the larger lobe w.r.t.'
+                             ' an overlapped staffline is lower than this, we consider'
+                             ' the notehead to belong to the adjacent staffspace.')
+
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='Turn on INFO messages.')
+    parser.add_argument('--debug', action='store_true',
+                        help='Turn on DEBUG messages.')
+
+    return parser
+
+
+def main(args):
+    logging.info('Starting main...')
+    _start_time = time.clock()
+
+    ##########################################################################
+    logging.info('Import the Node list')
+    if not os.path.isfile(args.annot):
+        raise ValueError('Annotation file {0} not found!'
+                         ''.format(args.annot))
+    nodes = read_nodes_from_file(args.annot)
+
+    output_nodes = add_staff_relationships(
+        nodes,
+        notehead_staffspace_threshold=args.notehead_staffspace_threshold)
+
+    ##########################################################################
+    logging.info('Export the combined list.')
+    nodes_string = export_node_list(output_nodes)
+
+    if args.export is not None:
+        with open(args.export, 'w') as hdl:
+            hdl.write(nodes_string)
+    else:
+        print(nodes_string)
+
+    _end_time = time.clock()
+    logging.info('add_staff_reationships.py done in {0:.3f} s'
+                 ''.format(_end_time - _start_time))
+
+
+if __name__ == '__main__':
+    parser = build_argument_parser()
+    args = parser.parse_args()
+
+    if args.verbose:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
+    if args.debug:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
+
+    main(args)
```

### Comparing `mung-1.1/scripts/add_staffline_symbols.py` & `mung-1.2/scripts/add_staffline_symbols.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,457 +1,457 @@
-"""The script ``add_staffline_symbols.py`` takes as input a CVC-MUSCIMA
-(page, writer) index and a corresponding NodeList file
-and adds to the NodeList staffline and staff objects."""
-import argparse
-import logging
-import os
-import time
-
-import numpy
-
-from skimage.io import imread
-from skimage.morphology import watershed
-from skimage.filters import gaussian
-from typing import Tuple
-
-from mung.dataset import CvcMuscimaDataset
-from mung.io import read_nodes_from_file, export_node_list
-from mung.node import Node
-from mung.utils import compute_connected_components
-
-from mung.constants import InferenceEngineConstants as _CONST
-
-
-def build_argument_parser():
-    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-
-    parser.add_argument('-i', '--staff_imfile', action='store',
-                        help='The image file with the staff-only image.'
-                             ' If not given, will use -n, -w and -r'
-                             ' to load it from the CVC-MUSCIMA staff removal'
-                             ' ground truth.')
-
-    parser.add_argument('-n', '--number', action='store', type=int,
-                        help='Number of the CVC-MUSCIMA page (1 - 20)')
-    parser.add_argument('-w', '--writer', action='store', type=int,
-                        help='Writer of the CVC-MUSCIMA page (1 - 50)')
-
-    parser.add_argument('-r', '--root', action='store',
-                        default=os.getenv('CVC_MUSCIMA_ROOT', None),
-                        help='Path to CVC-MUSCIMA dataset root. By default, will attempt'
-                             ' to read the CVC_MUSCIMA_ROOT env var. If that does not'
-                             ' work, the script will fail.')
-
-    parser.add_argument('-a', '--annot', action='store',  # required=True,
-                        help='The annotation file for which the staffline and staff'
-                             ' Nodes should be added. If not supplied, default'
-                             ' document/collection names will be used and Nodes will'
-                             ' be numberd from 0 in the output.')
-    parser.add_argument('-e', '--export', action='store',
-                        help='A filename to which the output NodeList'
-                             ' should be saved. If not given, will print to'
-                             ' stdout.')
-    parser.add_argument('--stafflines_only', action='store_true',
-                        help='If set, will only output stafflines, not other symbols.')
-
-    parser.add_argument('-v', '--verbose', action='store_true',
-                        help='Turn on INFO messages.')
-    parser.add_argument('--debug', action='store_true',
-                        help='Turn on DEBUG messages.')
-
-    return parser
-
-
-def main(args):
-    logging.info('Starting main...')
-    _start_time = time.clock()
-
-    ########################################################
-    # Load gt image.
-    logging.info('Loading staffline image.')
-    #  - Initialize Dataset. This checks for the root.
-
-    if args.staff_imfile is None:
-        cvc_dataset = CvcMuscimaDataset(root=args.root)
-        args.staff_imfile = cvc_dataset.imfile(page=args.number,
-                                               writer=args.writer,
-                                               distortion='ideal',
-                                               mode='staff_only')
-
-    # - Load the image.
-    gt = (imread(args.staff_imfile, as_grey=True) * 255).astype('uint8')
-
-    # - Cast as binary mask.
-    gt[gt > 0] = 1
-
-    ########################################################
-    # Locate stafflines in gt image.
-    logging.info('Getting staffline connected components.')
-
-    #  - Get connected components in gt image.
-    connected_components, labels, bboxes = compute_connected_components(gt)
-
-    #  - Use vertical dimension of CCs to determine which ones belong together
-    #    to form stafflines. (Criterion: row overlap.)
-    n_rows, n_cols = gt.shape
-    intervals = [[] for _ in range(n_rows)]  # For each row: which CCs have pxs on that row?
-    for label, (t, l, b, r) in list(bboxes.items()):
-        if label == 0:
-            continue
-        # Ignore very short staffline segments that can easily be artifacts
-        # and should not affect the vertical range of the staffline anyway.
-        if (r - l) < 8:
-            continue
-        for row in range(t, b):
-            intervals[row].append(label)
-
-    logging.info('Grouping staffline connected components into stafflines.')
-    staffline_components = []  # For each staffline, we collect the CCs that it is made of
-    _in_staffline = False
-    _current_staffline_components = []
-    for r_labels in intervals:
-        if not _in_staffline:
-            # Last row did not contain staffline components.
-            if len(r_labels) == 0:
-                # No staffline component on current row
-                continue
-            else:
-                _in_staffline = True
-                _current_staffline_components += r_labels
-        else:
-            # Last row contained staffline components.
-            if len(r_labels) == 0:
-                # Current staffline has no more rows.
-                staffline_components.append(set(_current_staffline_components))
-                _current_staffline_components = []
-                _in_staffline = False
-                continue
-            else:
-                # Current row contains staffline components: the current
-                # staffline continues.
-                _current_staffline_components += r_labels
-
-    logging.info('No. of stafflines, with component groups: {0}'
-                 ''.format(len(staffline_components)))
-
-    # Now: merge the staffline components into one bbox/mask.
-    logging.info('Merging staffline components into staffline bboxes and masks.')
-    staffline_bboxes = []
-    staffline_masks = []
-    for sc in sorted(staffline_components,
-                     key=lambda c: min([bboxes[cc][0]
-                                        for cc in c])):  # Sorted top-down
-        st, sl, sb, sr = n_rows, n_cols, 0, 0
-        for component in sc:
-            t, l, b, r = bboxes[component]
-            st, sl, sb, sr = min(t, st), min(l, sl), max(b, sb), max(r, sr)
-        _sm = gt[st:sb, sl:sr]
-        staffline_bboxes.append((st, sl, sb, sr))
-        staffline_masks.append(_sm)
-
-    # Check if n. of stafflines is divisible by 5
-    n_stafflines = len(staffline_bboxes)
-    logging.info('\tTotal stafflines: {0}'.format(n_stafflines))
-    if n_stafflines % 5 != 0:
-        import matplotlib.pyplot as plt
-        stafllines_mask_image = numpy.zeros(gt.shape)
-        for i, (_sb, _sm) in enumerate(zip(staffline_bboxes, staffline_masks)):
-            t, l, b, r = _sb
-            stafllines_mask_image[t:b, l:r] = min(255, (i * 333) % 255 + 40)
-        plt.imshow(stafllines_mask_image, cmap='jet', interpolation='nearest')
-        plt.show()
-        raise ValueError('No. of stafflines is not divisible by 5!')
-
-    logging.info('Creating staff bboxes and masks.')
-
-    #  - Go top-down and group the stafflines by five to get staves.
-    #    (The staffline bboxes are already sorted top-down.)
-    staff_bboxes = []
-    staff_masks = []
-
-    for i in range(n_stafflines // 5):
-        _sbb = staffline_bboxes[5 * i:5 * (i + 1)]
-        _st = min([bb[0] for bb in _sbb])
-        _sl = min([bb[1] for bb in _sbb])
-        _sb = max([bb[2] for bb in _sbb])
-        _sr = max([bb[3] for bb in _sbb])
-        staff_bboxes.append((_st, _sl, _sb, _sr))
-        staff_masks.append(gt[_st:_sb, _sl:_sr])
-
-    logging.info('Total staffs: {0}'.format(len(staff_bboxes)))
-
-    ##################################################################
-    # (Optionally fill in missing pixels, based on full image.)
-    logging.info('SKIP: fill in missing pixels based on full image.')
-    #  - Load full image
-    #  - Find gap regions
-    #  - Obtain gap region masks from full image
-    #  - Add gap region mask to staffline mask.
-
-    # Create the Nodes for stafflines and staffs:
-    #  - Load corresponding annotation, to which the stafflines and
-    #    staves should be added. (This is needed to correctly set docname
-    #    and node_ids.)
-    if not args.annot:
-        nodes = []
-        next_node_id = 0
-        dataset = 'FCNOMR'
-        document = os.path.splitext(os.path.basename(args.staff_imfile))[0]
-    else:
-        if not os.path.isfile(args.annot):
-            raise ValueError('Annotation file {0} does not exist!'.format(args.annot))
-
-        logging.info('Creating Nodes...')
-        nodes = read_nodes_from_file(args.annot)
-        logging.info('Non-staffline Nodes: {0}'.format(len(nodes)))
-        next_node_id = max([c.id for c in nodes]) + 1
-        dataset = nodes[0].dataset
-        document = nodes[0].document
-
-    #  - Create the staffline Nodes
-    stafflines = []
-    for sl_bb, sl_m in zip(staffline_bboxes, staffline_masks):
-        t, l, b, r = sl_bb
-        c = Node(id_=next_node_id,
-                 class_name=_CONST.STAFFLINE_CLASS_NAME,
-                 top=t, left=l, height=b - t, width=r - l,
-                 mask=sl_m,
-                 dataset=dataset, document=document)
-        stafflines.append(c)
-        next_node_id += 1
-
-    if not args.stafflines_only:
-
-        #  - Create the staff Nodes
-        staffs = []
-        for s_bb, s_m in zip(staff_bboxes, staff_masks):
-            t, l, b, r = s_bb
-            c = Node(id_=next_node_id,
-                     class_name=_CONST.STAFF_CLASS_NAME,
-                     top=t, left=l, height=b - t, width=r - l,
-                     mask=s_m,
-                     dataset=dataset, document=document)
-            staffs.append(c)
-            next_node_id += 1
-
-        #  - Add the inlinks/outlinks
-        for i, sc in enumerate(staffs):
-            sl_from = 5 * i
-            sl_to = 5 * (i + 1)
-            for sl in stafflines[sl_from:sl_to]:
-                sl.inlinks.append(sc.id)
-                sc.outlinks.append(sl.id)
-
-        # Add the staffspaces.
-        staffspaces = []
-        for i, staff in enumerate(staffs):
-            current_stafflines = [sc for sc in stafflines if sc.id in staff.outlinks]
-            sorted_stafflines = sorted(current_stafflines, key=lambda x: x.top)
-
-            current_staffspaces = []
-
-            # Percussion single-line staves do not have staffspaces.
-            if len(sorted_stafflines) == 1:
-                continue
-
-            # Internal staffspace
-            for s1, s2 in zip(sorted_stafflines[:-1], sorted_stafflines[1:]):
-                # s1 is the UPPER staffline, s2 is the LOWER staffline
-                # Left and right limits: to simplify things, we take the column
-                # *intersection* of (s1, s2). This gives the invariant that
-                # the staffspace is limited from top and bottom in each of its columns.
-                l = max(s1.left, s2.left)
-                r = min(s1.right, s2.right)
-
-                # Shift s1, s2 to the right by this much to have the cols. align
-                # All of these are non-negative.
-                dl1, dl2 = l - s1.left, l - s2.left
-                dr1, dr2 = s1.right - r, s2.right - r
-
-                # The stafflines are not necessarily straight,
-                # so top is given for the *topmost bottom edge* of the top staffline + 1
-
-                # First create mask
-                canvas = numpy.zeros((s2.bottom - s1.top, r - l), dtype='uint8')
-
-                # Paste masks into canvas.
-                # This assumes that the top of the bottom staffline is below
-                # the top of the top staffline... and that the bottom
-                # of the top staffline is above the bottom of the bottom
-                # staffline. This may not hold in very weird situations,
-                # but it's good for now.
-                logging.debug(s1.bounding_box, s1.mask.shape)
-                logging.debug(s2.bounding_box, s2.mask.shape)
-                logging.debug(canvas.shape)
-                logging.debug('l={0}, dl1={1}, dl2={2}, r={3}, dr1={4}, dr2={5}'
-                              ''.format(l, dl1, dl2, r, dr1, dr2))
-                # canvas[:s1.height, :] += s1.mask[:, dl1:s1.width-dr1]
-                # canvas[-s2.height:, :] += s2.mask[:, dl2:s2.width-dr2]
-
-                # We have to deal with staffline interruptions.
-                # One way to do this
-                # is watershed fill: put markers along the bottom and top
-                # edge, use mask * 10000 as elevation
-
-                s1_above, s1_below = staffline_surroundings_mask(s1)
-                s2_above, s2_below = staffline_surroundings_mask(s2)
-
-                # Get bounding boxes of the individual stafflines' masks
-                # that intersect with the staffspace bounding box, in terms
-                # of the staffline bounding box.
-                s1_t, s1_l, s1_b, s1_r = 0, dl1, \
-                                         s1.height, s1.width - dr1
-                s1_h, s1_w = s1_b - s1_t, s1_r - s1_l
-                s2_t, s2_l, s2_b, s2_r = canvas.shape[0] - s2.height, dl2, \
-                                         canvas.shape[0], s2.width - dr2
-                s2_h, s2_w = s2_b - s2_t, s2_r - s2_l
-
-                logging.debug(s1_t, s1_l, s1_b, s1_r, (s1_h, s1_w))
-
-                # We now take the intersection of s1_below and s2_above.
-                # If there is empty space in the middle, we fill it in.
-                staffspace_mask = numpy.ones(canvas.shape)
-                staffspace_mask[s1_t:s1_b, :] -= (1 - s1_below[:, dl1:s1.width - dr1])
-                staffspace_mask[s2_t:s2_b, :] -= (1 - s2_above[:, dl2:s2.width - dr2])
-
-                ss_top = s1.top
-                ss_bottom = s2.bottom
-                ss_left = l
-                ss_right = r
-
-                staffspace = Node(next_node_id, _CONST.STAFFSPACE_CLASS_NAME,
-                                  top=ss_top, left=ss_left,
-                                  height=ss_bottom - ss_top,
-                                  width=ss_right - ss_left,
-                                  mask=staffspace_mask,
-                                  dataset=dataset, document=document)
-
-                staffspace.inlinks.append(staff.id)
-                staff.outlinks.append(staffspace.id)
-
-                current_staffspaces.append(staffspace)
-
-                next_node_id += 1
-
-            # Add top and bottom staffspace.
-            # These outer staffspaces will have the width
-            # of their bottom neighbor, and height derived
-            # from its mask columns.
-            # This is quite approximate, but it should do.
-
-            # Upper staffspace
-            tsl = sorted_stafflines[0]
-            tsl_heights = tsl.mask.sum(axis=0)
-            tss = current_staffspaces[0]
-            tss_heights = tss.mask.sum(axis=0)
-
-            uss_top = max(0, tss.top - max(tss_heights))
-            uss_left = tss.left
-            uss_width = tss.width
-            # We use 1.5, so that large noteheads
-            # do not "hang out" of the staffspace.
-            uss_height = int(tss.height / 1.2)
-            # Shift because of height downscaling:
-            uss_top += tss.height - uss_height
-            uss_mask = tss.mask[:uss_height, :] * 1
-
-            staffspace = Node(next_node_id, _CONST.STAFFSPACE_CLASS_NAME,
-                              top=uss_top, left=uss_left,
-                              height=uss_height,
-                              width=uss_width,
-                              mask=uss_mask,
-                              dataset=dataset, document=document)
-            current_staffspaces.append(staffspace)
-            staff.outlinks.append(staffspace.id)
-            staffspace.inlinks.append(staff.id)
-            next_node_id += 1
-
-            # Lower staffspace
-            bss = current_staffspaces[-1]
-            bss_heights = bss.mask.sum(axis=0)
-            bsl = sorted_stafflines[-1]
-            bsl_heights = bsl.mask.sum(axis=0)
-
-            lss_top = bss.bottom  # + max(bsl_heights)
-            lss_left = bss.left
-            lss_width = bss.width
-            lss_height = int(bss.height / 1.2)
-            lss_mask = bss.mask[:lss_height, :] * 1
-
-            staffspace = Node(next_node_id, _CONST.STAFFSPACE_CLASS_NAME,
-                              top=lss_top, left=lss_left,
-                              height=lss_height,
-                              width=lss_width,
-                              mask=lss_mask,
-                              dataset=dataset, document=document)
-            current_staffspaces.append(staffspace)
-            staff.outlinks.append(staffspace.id)
-            staffspace.inlinks.append(staff.id)
-            next_node_id += 1
-
-            # ################ End of dealing with upper/lower staffspace ######
-
-            # Add to current list
-            staffspaces += current_staffspaces
-
-        # - Join the lists together
-        nodes_with_staffs = nodes \
-                            + stafflines \
-                            + staffspaces \
-                            + staffs
-
-    else:
-        nodes_with_staffs = nodes + stafflines
-
-    logging.info('Exporting the new Node list: {0} objects'
-                 ''.format(len(nodes_with_staffs)))
-    # - Export the combined list.
-    nodes_string = export_node_list(nodes_with_staffs)
-    if args.export is not None:
-        with open(args.export, 'w') as hdl:
-            hdl.write(nodes_string)
-    else:
-        print(nodes_string)
-
-    _end_time = time.clock()
-    logging.info('add_staffline_symbols.py done in {0:.3f} s'
-                 ''.format(_end_time - _start_time))
-
-
-def staffline_surroundings_mask(staffline: Node) -> Tuple[numpy.ndarray, numpy.ndarray]:
-    """Find the parts of the staffline's bounding box which lie
-    above or below the actual staffline.
-
-    These areas will be very small for straight stafflines,
-    but might be considerable when staffline curvature grows.
-    """
-    # We segment both masks into "above staffline" and "below staffline"
-    # areas.
-    elevation = staffline.mask * 255
-    # Blur, to plug small holes somewhat:
-    elevation = gaussian(elevation, sigma=1.0)
-    # Prepare the segmentation markers: 1 is ABOVE, 2 is BELOW
-    markers = numpy.zeros(staffline.mask.shape)
-    markers[0, :] = 1
-    markers[-1, :] = 2
-    markers[staffline.mask != 0] = 0
-    seg = watershed(elevation, markers)
-
-    bmask = numpy.ones(seg.shape)
-    bmask[seg != 2] = 0
-    tmask = numpy.ones(seg.shape)
-    tmask[seg != 1] = 0
-
-    return bmask, tmask
-
-
-if __name__ == '__main__':
-    parser = build_argument_parser()
-    args = parser.parse_args()
-
-    if args.verbose:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
-    if args.debug:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
-
-    main(args)
+"""The script ``add_staffline_symbols.py`` takes as input a CVC-MUSCIMA
+(page, writer) index and a corresponding NodeList file
+and adds to the NodeList staffline and staff objects."""
+import argparse
+import logging
+import os
+import time
+
+import numpy
+
+from skimage.io import imread
+from skimage.morphology import watershed
+from skimage.filters import gaussian
+from typing import Tuple
+
+from mung.dataset import CvcMuscimaDataset
+from mung.io import read_nodes_from_file, export_node_list
+from mung.node import Node
+from mung.utils import compute_connected_components
+
+from mung.constants import InferenceEngineConstants as _CONST
+
+
+def build_argument_parser():
+    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+
+    parser.add_argument('-i', '--staff_imfile', action='store',
+                        help='The image file with the staff-only image.'
+                             ' If not given, will use -n, -w and -r'
+                             ' to load it from the CVC-MUSCIMA staff removal'
+                             ' ground truth.')
+
+    parser.add_argument('-n', '--number', action='store', type=int,
+                        help='Number of the CVC-MUSCIMA page (1 - 20)')
+    parser.add_argument('-w', '--writer', action='store', type=int,
+                        help='Writer of the CVC-MUSCIMA page (1 - 50)')
+
+    parser.add_argument('-r', '--root', action='store',
+                        default=os.getenv('CVC_MUSCIMA_ROOT', None),
+                        help='Path to CVC-MUSCIMA dataset root. By default, will attempt'
+                             ' to read the CVC_MUSCIMA_ROOT env var. If that does not'
+                             ' work, the script will fail.')
+
+    parser.add_argument('-a', '--annot', action='store',  # required=True,
+                        help='The annotation file for which the staffline and staff'
+                             ' Nodes should be added. If not supplied, default'
+                             ' document/collection names will be used and Nodes will'
+                             ' be numberd from 0 in the output.')
+    parser.add_argument('-e', '--export', action='store',
+                        help='A filename to which the output NodeList'
+                             ' should be saved. If not given, will print to'
+                             ' stdout.')
+    parser.add_argument('--stafflines_only', action='store_true',
+                        help='If set, will only output stafflines, not other symbols.')
+
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='Turn on INFO messages.')
+    parser.add_argument('--debug', action='store_true',
+                        help='Turn on DEBUG messages.')
+
+    return parser
+
+
+def main(args):
+    logging.info('Starting main...')
+    _start_time = time.clock()
+
+    ########################################################
+    # Load gt image.
+    logging.info('Loading staffline image.')
+    #  - Initialize Dataset. This checks for the root.
+
+    if args.staff_imfile is None:
+        cvc_dataset = CvcMuscimaDataset(root=args.root)
+        args.staff_imfile = cvc_dataset.imfile(page=args.number,
+                                               writer=args.writer,
+                                               distortion='ideal',
+                                               mode='staff_only')
+
+    # - Load the image.
+    gt = (imread(args.staff_imfile, as_grey=True) * 255).astype('uint8')
+
+    # - Cast as binary mask.
+    gt[gt > 0] = 1
+
+    ########################################################
+    # Locate stafflines in gt image.
+    logging.info('Getting staffline connected components.')
+
+    #  - Get connected components in gt image.
+    connected_components, labels, bboxes = compute_connected_components(gt)
+
+    #  - Use vertical dimension of CCs to determine which ones belong together
+    #    to form stafflines. (Criterion: row overlap.)
+    n_rows, n_cols = gt.shape
+    intervals = [[] for _ in range(n_rows)]  # For each row: which CCs have pxs on that row?
+    for label, (t, l, b, r) in list(bboxes.items()):
+        if label == 0:
+            continue
+        # Ignore very short staffline segments that can easily be artifacts
+        # and should not affect the vertical range of the staffline anyway.
+        if (r - l) < 8:
+            continue
+        for row in range(t, b):
+            intervals[row].append(label)
+
+    logging.info('Grouping staffline connected components into stafflines.')
+    staffline_components = []  # For each staffline, we collect the CCs that it is made of
+    _in_staffline = False
+    _current_staffline_components = []
+    for r_labels in intervals:
+        if not _in_staffline:
+            # Last row did not contain staffline components.
+            if len(r_labels) == 0:
+                # No staffline component on current row
+                continue
+            else:
+                _in_staffline = True
+                _current_staffline_components += r_labels
+        else:
+            # Last row contained staffline components.
+            if len(r_labels) == 0:
+                # Current staffline has no more rows.
+                staffline_components.append(set(_current_staffline_components))
+                _current_staffline_components = []
+                _in_staffline = False
+                continue
+            else:
+                # Current row contains staffline components: the current
+                # staffline continues.
+                _current_staffline_components += r_labels
+
+    logging.info('No. of stafflines, with component groups: {0}'
+                 ''.format(len(staffline_components)))
+
+    # Now: merge the staffline components into one bbox/mask.
+    logging.info('Merging staffline components into staffline bboxes and masks.')
+    staffline_bboxes = []
+    staffline_masks = []
+    for sc in sorted(staffline_components,
+                     key=lambda c: min([bboxes[cc][0]
+                                        for cc in c])):  # Sorted top-down
+        st, sl, sb, sr = n_rows, n_cols, 0, 0
+        for component in sc:
+            t, l, b, r = bboxes[component]
+            st, sl, sb, sr = min(t, st), min(l, sl), max(b, sb), max(r, sr)
+        _sm = gt[st:sb, sl:sr]
+        staffline_bboxes.append((st, sl, sb, sr))
+        staffline_masks.append(_sm)
+
+    # Check if n. of stafflines is divisible by 5
+    n_stafflines = len(staffline_bboxes)
+    logging.info('\tTotal stafflines: {0}'.format(n_stafflines))
+    if n_stafflines % 5 != 0:
+        import matplotlib.pyplot as plt
+        stafllines_mask_image = numpy.zeros(gt.shape)
+        for i, (_sb, _sm) in enumerate(zip(staffline_bboxes, staffline_masks)):
+            t, l, b, r = _sb
+            stafllines_mask_image[t:b, l:r] = min(255, (i * 333) % 255 + 40)
+        plt.imshow(stafllines_mask_image, cmap='jet', interpolation='nearest')
+        plt.show()
+        raise ValueError('No. of stafflines is not divisible by 5!')
+
+    logging.info('Creating staff bboxes and masks.')
+
+    #  - Go top-down and group the stafflines by five to get staves.
+    #    (The staffline bboxes are already sorted top-down.)
+    staff_bboxes = []
+    staff_masks = []
+
+    for i in range(n_stafflines // 5):
+        _sbb = staffline_bboxes[5 * i:5 * (i + 1)]
+        _st = min([bb[0] for bb in _sbb])
+        _sl = min([bb[1] for bb in _sbb])
+        _sb = max([bb[2] for bb in _sbb])
+        _sr = max([bb[3] for bb in _sbb])
+        staff_bboxes.append((_st, _sl, _sb, _sr))
+        staff_masks.append(gt[_st:_sb, _sl:_sr])
+
+    logging.info('Total staffs: {0}'.format(len(staff_bboxes)))
+
+    ##################################################################
+    # (Optionally fill in missing pixels, based on full image.)
+    logging.info('SKIP: fill in missing pixels based on full image.')
+    #  - Load full image
+    #  - Find gap regions
+    #  - Obtain gap region masks from full image
+    #  - Add gap region mask to staffline mask.
+
+    # Create the Nodes for stafflines and staffs:
+    #  - Load corresponding annotation, to which the stafflines and
+    #    staves should be added. (This is needed to correctly set docname
+    #    and node_ids.)
+    if not args.annot:
+        nodes = []
+        next_node_id = 0
+        dataset = 'FCNOMR'
+        document = os.path.splitext(os.path.basename(args.staff_imfile))[0]
+    else:
+        if not os.path.isfile(args.annot):
+            raise ValueError('Annotation file {0} does not exist!'.format(args.annot))
+
+        logging.info('Creating Nodes...')
+        nodes = read_nodes_from_file(args.annot)
+        logging.info('Non-staffline Nodes: {0}'.format(len(nodes)))
+        next_node_id = max([c.id for c in nodes]) + 1
+        dataset = nodes[0].dataset
+        document = nodes[0].document
+
+    #  - Create the staffline Nodes
+    stafflines = []
+    for sl_bb, sl_m in zip(staffline_bboxes, staffline_masks):
+        t, l, b, r = sl_bb
+        c = Node(id_=next_node_id,
+                 class_name=_CONST.STAFFLINE,
+                 top=t, left=l, height=b - t, width=r - l,
+                 mask=sl_m,
+                 dataset=dataset, document=document)
+        stafflines.append(c)
+        next_node_id += 1
+
+    if not args.stafflines_only:
+
+        #  - Create the staff Nodes
+        staffs = []
+        for s_bb, s_m in zip(staff_bboxes, staff_masks):
+            t, l, b, r = s_bb
+            c = Node(id_=next_node_id,
+                     class_name=_CONST.STAFF,
+                     top=t, left=l, height=b - t, width=r - l,
+                     mask=s_m,
+                     dataset=dataset, document=document)
+            staffs.append(c)
+            next_node_id += 1
+
+        #  - Add the inlinks/outlinks
+        for i, sc in enumerate(staffs):
+            sl_from = 5 * i
+            sl_to = 5 * (i + 1)
+            for sl in stafflines[sl_from:sl_to]:
+                sl.inlinks.append(sc.id)
+                sc.outlinks.append(sl.id)
+
+        # Add the staffspaces.
+        staffspaces = []
+        for i, staff in enumerate(staffs):
+            current_stafflines = [sc for sc in stafflines if sc.id in staff.outlinks]
+            sorted_stafflines = sorted(current_stafflines, key=lambda x: x.top)
+
+            current_staffspaces = []
+
+            # Percussion single-line staves do not have staffspaces.
+            if len(sorted_stafflines) == 1:
+                continue
+
+            # Internal staffspace
+            for s1, s2 in zip(sorted_stafflines[:-1], sorted_stafflines[1:]):
+                # s1 is the UPPER staffline, s2 is the LOWER staffline
+                # Left and right limits: to simplify things, we take the column
+                # *intersection* of (s1, s2). This gives the invariant that
+                # the staffspace is limited from top and bottom in each of its columns.
+                l = max(s1.left, s2.left)
+                r = min(s1.right, s2.right)
+
+                # Shift s1, s2 to the right by this much to have the cols. align
+                # All of these are non-negative.
+                dl1, dl2 = l - s1.left, l - s2.left
+                dr1, dr2 = s1.right - r, s2.right - r
+
+                # The stafflines are not necessarily straight,
+                # so top is given for the *topmost bottom edge* of the top staffline + 1
+
+                # First create mask
+                canvas = numpy.zeros((s2.bottom - s1.top, r - l), dtype='uint8')
+
+                # Paste masks into canvas.
+                # This assumes that the top of the bottom staffline is below
+                # the top of the top staffline... and that the bottom
+                # of the top staffline is above the bottom of the bottom
+                # staffline. This may not hold in very weird situations,
+                # but it's good for now.
+                logging.debug(s1.bounding_box, s1.mask.shape)
+                logging.debug(s2.bounding_box, s2.mask.shape)
+                logging.debug(canvas.shape)
+                logging.debug('l={0}, dl1={1}, dl2={2}, r={3}, dr1={4}, dr2={5}'
+                              ''.format(l, dl1, dl2, r, dr1, dr2))
+                # canvas[:s1.height, :] += s1.mask[:, dl1:s1.width-dr1]
+                # canvas[-s2.height:, :] += s2.mask[:, dl2:s2.width-dr2]
+
+                # We have to deal with staffline interruptions.
+                # One way to do this
+                # is watershed fill: put markers along the bottom and top
+                # edge, use mask * 10000 as elevation
+
+                s1_above, s1_below = staffline_surroundings_mask(s1)
+                s2_above, s2_below = staffline_surroundings_mask(s2)
+
+                # Get bounding boxes of the individual stafflines' masks
+                # that intersect with the staffspace bounding box, in terms
+                # of the staffline bounding box.
+                s1_t, s1_l, s1_b, s1_r = 0, dl1, \
+                                         s1.height, s1.width - dr1
+                s1_h, s1_w = s1_b - s1_t, s1_r - s1_l
+                s2_t, s2_l, s2_b, s2_r = canvas.shape[0] - s2.height, dl2, \
+                                         canvas.shape[0], s2.width - dr2
+                s2_h, s2_w = s2_b - s2_t, s2_r - s2_l
+
+                logging.debug(s1_t, s1_l, s1_b, s1_r, (s1_h, s1_w))
+
+                # We now take the intersection of s1_below and s2_above.
+                # If there is empty space in the middle, we fill it in.
+                staffspace_mask = numpy.ones(canvas.shape)
+                staffspace_mask[s1_t:s1_b, :] -= (1 - s1_below[:, dl1:s1.width - dr1])
+                staffspace_mask[s2_t:s2_b, :] -= (1 - s2_above[:, dl2:s2.width - dr2])
+
+                ss_top = s1.top
+                ss_bottom = s2.bottom
+                ss_left = l
+                ss_right = r
+
+                staffspace = Node(next_node_id, _CONST.STAFFSPACE,
+                                  top=ss_top, left=ss_left,
+                                  height=ss_bottom - ss_top,
+                                  width=ss_right - ss_left,
+                                  mask=staffspace_mask,
+                                  dataset=dataset, document=document)
+
+                staffspace.inlinks.append(staff.id)
+                staff.outlinks.append(staffspace.id)
+
+                current_staffspaces.append(staffspace)
+
+                next_node_id += 1
+
+            # Add top and bottom staffspace.
+            # These outer staffspaces will have the width
+            # of their bottom neighbor, and height derived
+            # from its mask columns.
+            # This is quite approximate, but it should do.
+
+            # Upper staffspace
+            tsl = sorted_stafflines[0]
+            tsl_heights = tsl.mask.sum(axis=0)
+            tss = current_staffspaces[0]
+            tss_heights = tss.mask.sum(axis=0)
+
+            uss_top = max(0, tss.top - max(tss_heights))
+            uss_left = tss.left
+            uss_width = tss.width
+            # We use 1.5, so that large noteheads
+            # do not "hang out" of the staffspace.
+            uss_height = int(tss.height / 1.2)
+            # Shift because of height downscaling:
+            uss_top += tss.height - uss_height
+            uss_mask = tss.mask[:uss_height, :] * 1
+
+            staffspace = Node(next_node_id, _CONST.STAFFSPACE,
+                              top=uss_top, left=uss_left,
+                              height=uss_height,
+                              width=uss_width,
+                              mask=uss_mask,
+                              dataset=dataset, document=document)
+            current_staffspaces.append(staffspace)
+            staff.outlinks.append(staffspace.id)
+            staffspace.inlinks.append(staff.id)
+            next_node_id += 1
+
+            # Lower staffspace
+            bss = current_staffspaces[-1]
+            bss_heights = bss.mask.sum(axis=0)
+            bsl = sorted_stafflines[-1]
+            bsl_heights = bsl.mask.sum(axis=0)
+
+            lss_top = bss.bottom  # + max(bsl_heights)
+            lss_left = bss.left
+            lss_width = bss.width
+            lss_height = int(bss.height / 1.2)
+            lss_mask = bss.mask[:lss_height, :] * 1
+
+            staffspace = Node(next_node_id, _CONST.STAFFSPACE,
+                              top=lss_top, left=lss_left,
+                              height=lss_height,
+                              width=lss_width,
+                              mask=lss_mask,
+                              dataset=dataset, document=document)
+            current_staffspaces.append(staffspace)
+            staff.outlinks.append(staffspace.id)
+            staffspace.inlinks.append(staff.id)
+            next_node_id += 1
+
+            # ################ End of dealing with upper/lower staffspace ######
+
+            # Add to current list
+            staffspaces += current_staffspaces
+
+        # - Join the lists together
+        nodes_with_staffs = nodes \
+                            + stafflines \
+                            + staffspaces \
+                            + staffs
+
+    else:
+        nodes_with_staffs = nodes + stafflines
+
+    logging.info('Exporting the new Node list: {0} objects'
+                 ''.format(len(nodes_with_staffs)))
+    # - Export the combined list.
+    nodes_string = export_node_list(nodes_with_staffs)
+    if args.export is not None:
+        with open(args.export, 'w') as hdl:
+            hdl.write(nodes_string)
+    else:
+        print(nodes_string)
+
+    _end_time = time.clock()
+    logging.info('add_staffline_symbols.py done in {0:.3f} s'
+                 ''.format(_end_time - _start_time))
+
+
+def staffline_surroundings_mask(staffline: Node) -> Tuple[numpy.ndarray, numpy.ndarray]:
+    """Find the parts of the staffline's bounding box which lie
+    above or below the actual staffline.
+
+    These areas will be very small for straight stafflines,
+    but might be considerable when staffline curvature grows.
+    """
+    # We segment both masks into "above staffline" and "below staffline"
+    # areas.
+    elevation = staffline.mask * 255
+    # Blur, to plug small holes somewhat:
+    elevation = gaussian(elevation, sigma=1.0)
+    # Prepare the segmentation markers: 1 is ABOVE, 2 is BELOW
+    markers = numpy.zeros(staffline.mask.shape)
+    markers[0, :] = 1
+    markers[-1, :] = 2
+    markers[staffline.mask != 0] = 0
+    seg = watershed(elevation, markers)
+
+    bmask = numpy.ones(seg.shape)
+    bmask[seg != 2] = 0
+    tmask = numpy.ones(seg.shape)
+    tmask[seg != 1] = 0
+
+    return bmask, tmask
+
+
+if __name__ == '__main__':
+    parser = build_argument_parser()
+    args = parser.parse_args()
+
+    if args.verbose:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
+    if args.debug:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
+
+    main(args)
```

### Comparing `mung-1.1/scripts/analyze_agreement.py` & `mung-1.2/scripts/analyze_agreement.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,440 +1,440 @@
-#!/usr/bin/env python
-"""``analyze_agreement.py`` is a script that analyzes the agreement between two
-annotations of the same file. The script measures:
-
-* Object counts: are they the same?
-* Object assignment: given the least-squares mapping of objects
-  onto each other, to what extent do they differ?
-
-For an overview of command-line options, call::
-
-  analyze_agreement.py -h
-
-Alignment algorithm
--------------------
-
-The script uses a greedy alignment procedure.
-
-First, it computes for each ``(truth, prediction)`` symbol pair
-their recall, precision, and f-score over pixels that fall within
-the mask (bounding box overlap may be misleading, mainly for
-parallel beams).
-
-Each predicted symbol is then aligned to the ground truth symbol
-with the highest f-score. If the symbol classes of a ``(truth, prediction)``
-pair do not match, their score gets set to 0. (This can be turned
-off using the ``--no_strict_class_names`` option.)
-
-Next, the alignment is cleaned up: if multiple predictions are
-aligned to a single ground truth, the one with the highest f-score
-is chosen and the other predicted symbols are considered
-unaligned.
-
-Computing the output f-score
-----------------------------
-
-Finally, we sum all the f-scores of ``(truth, prediction)``
-symbol pairs in the alignment.
-
-Ground truth symbols that are not aligned to any predicted object
-also contribute a zero to the overall f-score.
-
-"""
-import argparse
-import collections
-import logging
-import pprint
-import time
-
-import numpy
-from typing import List, Tuple, Optional
-
-from mung.io import read_nodes_from_file
-from mung.node import Node
-
-
-def bounding_box_intersection(origin: Tuple[int, int, int, int], intersect: Tuple[int, int, int, int]) \
-        -> Optional[Tuple[int, int, int, int]]:
-    """Returns the coordinates of the origin bounding box that
-    are intersected by the intersect bounding box.
-
-    >>> bounding_box = 10, 100, 30, 110
-    >>> other_bbox = 20, 100, 40, 105
-    >>> bounding_box_intersection(bounding_box, other_bbox)
-    (10, 0, 20, 5)
-    >>> bounding_box_intersection(other_bbox, bounding_box)
-    (0, 0, 10, 5)
-    >>> containing_bbox = 4, 55, 44, 115
-    >>> bounding_box_intersection(bounding_box, containing_bbox)
-    (0, 0, 20, 10)
-    >>> contained_bbox = 12, 102, 22, 108
-    >>> bounding_box_intersection(bounding_box, contained_bbox)
-    (2, 2, 12, 8)
-    >>> non_overlapping_bbox = 0, 0, 3, 3
-    >>> bounding_box_intersection(bounding_box, non_overlapping_bbox) is None
-    True
-
-    """
-    o_t, o_l, o_b, o_r = origin
-    t, l, b, r = intersect
-
-    out_top = max(t, o_t)
-    out_left = max(l, o_l)
-    out_bottom = min(b, o_b)
-    out_right = min(r, o_r)
-
-    if (out_top < out_bottom) and (out_left < out_right):
-        return out_top - o_t, \
-               out_left - o_l, \
-               out_bottom - o_t, \
-               out_right - o_l
-    else:
-        return None
-
-
-def pixel_metrics(truth: Node, prediction: Node) -> Tuple[float, float, float]:
-    """Computes the recall, precision and f-score for the prediction
-    Node given the truth Node."""
-    recall, precision, fscore = 0, 0, 0
-
-    intersection_truth = bounding_box_intersection(truth.bounding_box,
-                                                   prediction.bounding_box)
-    if intersection_truth is None:
-        logging.debug('No intersection for Nodes: t={0},'
-                      ' p={1}'.format(truth.bounding_box,
-                                      prediction.bounding_box))
-        return recall, precision, fscore
-
-    intersection_pred = bounding_box_intersection(prediction.bounding_box,
-                                                  truth.bounding_box)
-
-    logging.debug('Found intersection for Nodes: t={0},'
-                  ' p={1}'.format(truth.bounding_box,
-                                  prediction.bounding_box))
-
-    tt, tl, tb, tr = intersection_truth
-    pt, pl, pb, pr = intersection_pred
-    crop_truth = truth.mask[tt:tb, tl:tr]
-    crop_pred = prediction.mask[pt:pb, pl:pr]
-
-    # Assumes the mask values are 1...
-
-    n_truth = float(truth.mask.sum())
-    n_pred = float(prediction.mask.sum())
-    n_common = float((crop_truth * crop_pred).sum())
-
-    # There are no zero-pixel objects, but the overlap may be nonzero
-    if n_truth == 0:
-        recall = 0.0
-        precision = 0.0
-    elif n_pred == 0:
-        recall = 0.0
-        precision = 0.0
-    else:
-        recall = n_common / n_truth
-        precision = n_common / n_pred
-
-    if (recall == 0) or (precision == 0):
-        fscore = 0
-    else:
-        fscore = 2 * recall * precision / (recall + precision)
-
-    return recall, precision, fscore
-
-
-def compute_recall_precision_fscore(truth: List[Node], prediction: List[Node]) \
-        -> Tuple[numpy.ndarray, numpy.ndarray, numpy.ndarray]:
-    """Computes Node pixel-level metrics.
-
-    :param truth: A list of the ground truth Nodes.
-
-    :param prediction: A list of the predicted Nodes.
-
-    :returns: Three matrices with shape ``(len(truth), len(prediction)``:
-        recall, precision, and f-score for each truth/prediction Node
-        pair. Truth Nodes are rows, prediction columns.
-    """
-    recall = numpy.zeros((len(truth), len(prediction)))
-    precision = numpy.zeros((len(truth), len(prediction)))
-    fscore = numpy.zeros((len(truth), len(prediction)))
-
-    for i, t in enumerate(truth):
-        for j, p in enumerate(prediction):
-            r, p, f = pixel_metrics(t, p)
-            recall[i, j] = r
-            precision[i, j] = p
-            fscore[i, j] = f
-
-    return recall, precision, fscore
-
-
-def align_nodes(truth: List[Node], prediction: List[Node], fscore=None) -> List[Tuple[int, int]]:
-    """Aligns prediction Nodes to truth.
-
-    :param truth: A list of the ground truth Nodes.
-
-    :param prediction: A list of the predicted Nodes.
-
-    :returns: A list of (t, p) pairs of Node indices into
-        the truth and prediction lists. There will be one
-        pair for each predicted symbol.
-    """
-    if fscore is None:
-        _, _, fscore = compute_recall_precision_fscore(truth, prediction)
-
-    # For each prediction (column), pick the highest-scoring
-    # True symbol.
-    closest_truths = list(fscore.argmax(axis=0))
-
-    # Checking for duplicate "best ground truth" alignments.
-    # This does *not* check for duplicates in the sense
-    # "multiple predictions aligned to the same truth"
-    # or "multiple truths aligned to the same prediction",
-    # it only acts as a tie-breaker in case one prediction overlaps
-    # to the same degree multiple truth objects (e.g. a single sharp
-    # in a key signature).
-    closest_truth_distance = [fscore[ct, j]
-                              for j, ct in enumerate(closest_truths)]
-    equidistant_closest_truths = [[i for i, x in enumerate(fscore[:, j])
-                                   if x == ct]
-                                  for j, ct in enumerate(closest_truth_distance)]
-
-    class_name_aware_closest_truths = []
-    for j, ects in enumerate(equidistant_closest_truths):
-        best_truth_i = int(ects[0])
-
-        # If there is more than one tied best choice,
-        # try to choose the truth Node that has the same
-        # class as the predicted Node.
-        if len(ects) > 1:
-            ects_c = {truth[int(i)].class_name: i for i in ects}
-            j_class_name = prediction[j].class_name
-            if j_class_name in ects_c:
-                best_truth_i = int(ects_c[j_class_name])
-
-        class_name_aware_closest_truths.append(best_truth_i)
-
-    alignment = [(t, p) for p, t in enumerate(class_name_aware_closest_truths)]
-    return alignment
-
-
-def compute_recall_precision_fscore_given_an_alignment(alignment: List[Tuple[int, int]], individual_recalls,
-                                                       individual_precisions, n_not_aligned: int = 0,
-                                                       strict_classnames: bool = True,
-                                                       truths: List[Node] = None, predictions: List[Node] = None)\
-        -> Tuple[float, float, float]:
-    if strict_classnames:
-        if not truths:
-            raise ValueError('If strict_classnames is requested, must supply truths Nodes!')
-        if not predictions:
-            raise ValueError('If strict_classnames is requested, must supply predictions Nodes!')
-
-    total_recall, total_precision = 0, 0
-
-    for i, j in alignment:
-
-        # Check for strict_classnames only at this stage.
-        # The purpose is: if two people mark the same object
-        # differently, we do want to know "it should be aligned
-        # to each other, but the classes don't fit" -- we don't
-        # want to maybe align it to an overlapping object of
-        # the corresponding wrong class.
-        if strict_classnames:
-            t_c = truths[i]
-            p_c = predictions[j]
-            if t_c.class_name != p_c.class_name:
-                continue
-
-        total_recall += individual_recalls[i, j]
-        total_precision += individual_precisions[i, j]
-
-    # This is not correct...? What about the zeros?
-    #  - Prediction with no GT is in the alignment, so it counts towards
-    #    the len(alignment) denominator.
-    #  - GT with no prediction aligned to it contributes zero, but is
-    #    not counted towards the denominator.
-    total_recall /= len(alignment) + n_not_aligned
-    total_precision /= len(alignment) + n_not_aligned
-
-    if (total_recall == 0) or (total_precision == 0):
-        total_fscore = 0.0
-    else:
-        total_fscore = 2 * total_recall * total_precision / (total_recall + total_precision)
-    return total_recall, total_precision, total_fscore
-
-
-##############################################################################
-
-
-def build_argument_parser():
-    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-
-    parser.add_argument('-t', '--true', action='store', required=True,
-                        help='The Nodes file you want to consider'
-                             ' ground truth.')
-    parser.add_argument('-p', '--prediction', action='store', required=True,
-                        help='The Nodes file you want to consider'
-                             ' the prediction.')
-
-    parser.add_argument('-e', '--export', action='store',
-                        help='If set, will export the problematic Nodes'
-                             ' to this file.')
-
-    parser.add_argument('--analyze_alignment', action='store_true',
-                        help='If set, will check whether the alignment is 1:1,'
-                             ' and print out the irregularities.')
-    parser.add_argument('--analyze_classnames', action='store_true',
-                        help='If set, will check whether the Nodes aligned'
-                             ' to each other have the same class labels'
-                             ' and print out the irregularities.')
-    parser.add_argument('--no_strict_classnames', action='store_true',
-                        help='If set, will not require aligned objects\' classnames'
-                             ' to match before computing pixel-wise overlap'
-                             ' metrics.')
-    parser.add_argument('--log_alignment', action='store_true',
-                        help='Print how the true and predicted objects are'
-                             ' paired.')
-
-    parser.add_argument('--print_fscore_only', action='store_true',
-                        help='If set, only print the total F-score number.'
-                             ' Useful for using in an automated pipeline.')
-
-    parser.add_argument('-v', '--verbose', action='store_true',
-                        help='Turn on INFO messages.')
-    parser.add_argument('--debug', action='store_true',
-                        help='Turn on DEBUG messages.')
-
-    return parser
-
-
-def main(args):
-    logging.info('Starting main...')
-    _start_time = time.clock()
-
-    # The algorithm:
-    #  - build the cost function(s) for a pair of Nodes
-    #  - align the objects, using the cost function
-
-    # First alignment: try just matching a predicted object to the nearest
-    # true object.
-    # First distance function: proportion of shared pixels.
-    # Rule: if two objects don't share a pixel, they cannot be considered related.
-    # Object classes do not factor into this so far.
-
-    ground_truth_nodes = read_nodes_from_file(args.true)
-    predicted_nodes = read_nodes_from_file(args.prediction)
-
-    _parse_time = time.clock()
-    logging.info('Parsing {0} true and {1} prediction Nodes took {2:.2f} s'
-                 ''.format(len(ground_truth_nodes), len(predicted_nodes), _parse_time - _start_time))
-
-    recall, precision, fscore = compute_recall_precision_fscore(ground_truth_nodes, predicted_nodes)
-
-    _rpf_time = time.clock()
-    logging.info('Computing {0} entries of r/p/f matrices took {1:.2f} s'
-                 ''.format(len(ground_truth_nodes) * len(predicted_nodes), _rpf_time - _parse_time))
-
-    alignment_tp = align_nodes(ground_truth_nodes, predicted_nodes, fscore=fscore)
-    alignment_pt = align_nodes(predicted_nodes, ground_truth_nodes, fscore=fscore.T)
-
-    # Intersect alignments
-    _aln_tp_set = frozenset(alignment_tp)
-    alignment_tp_symmetric = [(t, p) for p, t in alignment_pt
-                              if (t, p) in _aln_tp_set
-                              and (ground_truth_nodes[t].class_name == predicted_nodes[p].class_name)]
-    truth_not_aligned = [t for p, t in alignment_pt
-                         if (t, p) not in alignment_tp_symmetric]
-    n_truth_not_aligned = len(truth_not_aligned)
-    preds_not_aligned = [p for t, p in alignment_tp
-                         if (t, p) not in alignment_tp_symmetric]
-    n_preds_not_aligned = len(preds_not_aligned)
-    n_not_aligned = n_truth_not_aligned + n_preds_not_aligned
-
-    _aln_time = time.clock()
-    logging.info('Computing alignment took {0:.2f} s'
-                 ''.format(_aln_time - _rpf_time))
-
-    # Now compute agreement: precision and recall on pixels
-    # of the aligned Nodes.
-
-    # We apply strict classnames only here, after the Nodes have been
-    # aligned to each other using pixel metrics.
-    strict_classnames = (not args.no_strict_classnames)
-    total_r, total_p, total_f = compute_recall_precision_fscore_given_an_alignment(alignment_tp_symmetric, recall, precision,
-                                                                                   n_not_aligned=n_not_aligned,
-                                                                                   strict_classnames=strict_classnames,
-                                                                                   truths=ground_truth_nodes,
-                                                                                   predictions=predicted_nodes)
-
-    if not args.print_fscore_only:
-        print('Truth objs.:\t{0}'.format(len(ground_truth_nodes)))
-        print('Pred. objs.:\t{0}'.format(len(predicted_nodes)))
-        print('Aligned objs.:\t{0}'.format(len(alignment_tp_symmetric)))
-        print('==============================================')
-        print('Recall:\t\t{0:.3f}\nPrecision:\t{1:.3f}\nF-score:\t{2:.3f}'
-              ''.format(total_r, total_p, total_f))
-        print('')
-    else:
-        print('{0:.3f}'.format(total_f))
-        return
-
-    if args.log_alignment:
-        print('==============================================')
-        print('Alignments:\n{0}'.format('\n'.join([
-            '({0}: {1}) -- ({2}: {3})'.format(ground_truth_nodes[t].id, ground_truth_nodes[t].class_name,
-                                              predicted_nodes[p].id, predicted_nodes[p].class_name)
-            for t, p in alignment_tp_symmetric
-        ])))
-        print('Truth, not aligned:\n{0}'.format('\n'.join(['({0}: {1})'.format(ground_truth_nodes[t].id, ground_truth_nodes[t].class_name)
-                                                           for t in truth_not_aligned])))
-        print(
-            'Preds, not aligned:\n{0}'.format('\n'.join(['({0}: {1})'.format(predicted_nodes[p].id, predicted_nodes[p].class_name)
-                                                         for p in preds_not_aligned])))
-
-    ##########################################################################
-    # Check if the alignment is a pairing -- find truth objects
-    # with more than one prediction aligned to them.
-    if args.analyze_alignment:
-        t_aln_dict = collections.defaultdict(list)
-        for i, j in alignment_tp_symmetric:
-            t_aln_dict[i].append(predicted_nodes[j])
-
-        multiple_truths = [ground_truth_nodes[i] for i in t_aln_dict
-                           if len(t_aln_dict[i]) > 1]
-        multiple_truths_aln_dict = {t: t_aln_dict[t]
-                                    for t in t_aln_dict
-                                    if len(t_aln_dict[t]) > 1}
-
-        print('Truth multi-aligned Node classes:\n{0}'
-              ''.format(pprint.pformat(
-            {(ground_truth_nodes[t].id, ground_truth_nodes[t].class_name): [(p.id, p.class_name)
-                                                  for p in t_aln_dict[t]]
-             for t in multiple_truths_aln_dict})))
-
-    ##########################################################################
-    # Check if the aligned objects have the same classes
-    if args.analyze_classnames:
-        different_classnames_pairs = []
-        for i, j in alignment_tp_symmetric:
-            if ground_truth_nodes[i].class_name != predicted_nodes[j].class_name:
-                different_classnames_pairs.append((ground_truth_nodes[i], predicted_nodes[j]))
-        print('Aligned pairs with different class_names:\n{0}'
-              ''.format('\n'.join(['{0}.{1}\t{2}.{3}'
-                                   ''.format(t.id, t.class_name, p.id, p.class_name)
-                                   for t, p in different_classnames_pairs])))
-
-    _end_time = time.clock()
-    logging.info('analyze_agreement.py done in {0:.3f} s'.format(_end_time - _start_time))
-
-
-if __name__ == '__main__':
-    parser = build_argument_parser()
-    args = parser.parse_args()
-
-    if args.verbose:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
-    if args.debug:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
-
-    main(args)
+#!/usr/bin/env python
+"""``analyze_agreement.py`` is a script that analyzes the agreement between two
+annotations of the same file. The script measures:
+
+* Object counts: are they the same?
+* Object assignment: given the least-squares mapping of objects
+  onto each other, to what extent do they differ?
+
+For an overview of command-line options, call::
+
+  analyze_agreement.py -h
+
+Alignment algorithm
+-------------------
+
+The script uses a greedy alignment procedure.
+
+First, it computes for each ``(truth, prediction)`` symbol pair
+their recall, precision, and f-score over pixels that fall within
+the mask (bounding box overlap may be misleading, mainly for
+parallel beams).
+
+Each predicted symbol is then aligned to the ground truth symbol
+with the highest f-score. If the symbol classes of a ``(truth, prediction)``
+pair do not match, their score gets set to 0. (This can be turned
+off using the ``--no_strict_class_names`` option.)
+
+Next, the alignment is cleaned up: if multiple predictions are
+aligned to a single ground truth, the one with the highest f-score
+is chosen and the other predicted symbols are considered
+unaligned.
+
+Computing the output f-score
+----------------------------
+
+Finally, we sum all the f-scores of ``(truth, prediction)``
+symbol pairs in the alignment.
+
+Ground truth symbols that are not aligned to any predicted object
+also contribute a zero to the overall f-score.
+
+"""
+import argparse
+import collections
+import logging
+import pprint
+import time
+
+import numpy
+from typing import List, Tuple, Optional
+
+from mung.io import read_nodes_from_file
+from mung.node import Node
+
+
+def bounding_box_intersection(origin: Tuple[int, int, int, int], intersect: Tuple[int, int, int, int]) \
+        -> Optional[Tuple[int, int, int, int]]:
+    """Returns the coordinates of the origin bounding box that
+    are intersected by the intersect bounding box.
+
+    >>> bounding_box = 10, 100, 30, 110
+    >>> other_bbox = 20, 100, 40, 105
+    >>> bounding_box_intersection(bounding_box, other_bbox)
+    (10, 0, 20, 5)
+    >>> bounding_box_intersection(other_bbox, bounding_box)
+    (0, 0, 10, 5)
+    >>> containing_bbox = 4, 55, 44, 115
+    >>> bounding_box_intersection(bounding_box, containing_bbox)
+    (0, 0, 20, 10)
+    >>> contained_bbox = 12, 102, 22, 108
+    >>> bounding_box_intersection(bounding_box, contained_bbox)
+    (2, 2, 12, 8)
+    >>> non_overlapping_bbox = 0, 0, 3, 3
+    >>> bounding_box_intersection(bounding_box, non_overlapping_bbox) is None
+    True
+
+    """
+    o_t, o_l, o_b, o_r = origin
+    t, l, b, r = intersect
+
+    out_top = max(t, o_t)
+    out_left = max(l, o_l)
+    out_bottom = min(b, o_b)
+    out_right = min(r, o_r)
+
+    if (out_top < out_bottom) and (out_left < out_right):
+        return out_top - o_t, \
+               out_left - o_l, \
+               out_bottom - o_t, \
+               out_right - o_l
+    else:
+        return None
+
+
+def pixel_metrics(truth: Node, prediction: Node) -> Tuple[float, float, float]:
+    """Computes the recall, precision and f-score for the prediction
+    Node given the truth Node."""
+    recall, precision, fscore = 0, 0, 0
+
+    intersection_truth = bounding_box_intersection(truth.bounding_box,
+                                                   prediction.bounding_box)
+    if intersection_truth is None:
+        logging.debug('No intersection for Nodes: t={0},'
+                      ' p={1}'.format(truth.bounding_box,
+                                      prediction.bounding_box))
+        return recall, precision, fscore
+
+    intersection_pred = bounding_box_intersection(prediction.bounding_box,
+                                                  truth.bounding_box)
+
+    logging.debug('Found intersection for Nodes: t={0},'
+                  ' p={1}'.format(truth.bounding_box,
+                                  prediction.bounding_box))
+
+    tt, tl, tb, tr = intersection_truth
+    pt, pl, pb, pr = intersection_pred
+    crop_truth = truth.mask[tt:tb, tl:tr]
+    crop_pred = prediction.mask[pt:pb, pl:pr]
+
+    # Assumes the mask values are 1...
+
+    n_truth = float(truth.mask.sum())
+    n_pred = float(prediction.mask.sum())
+    n_common = float((crop_truth * crop_pred).sum())
+
+    # There are no zero-pixel objects, but the overlap may be nonzero
+    if n_truth == 0:
+        recall = 0.0
+        precision = 0.0
+    elif n_pred == 0:
+        recall = 0.0
+        precision = 0.0
+    else:
+        recall = n_common / n_truth
+        precision = n_common / n_pred
+
+    if (recall == 0) or (precision == 0):
+        fscore = 0
+    else:
+        fscore = 2 * recall * precision / (recall + precision)
+
+    return recall, precision, fscore
+
+
+def compute_recall_precision_fscore(truth: List[Node], prediction: List[Node]) \
+        -> Tuple[numpy.ndarray, numpy.ndarray, numpy.ndarray]:
+    """Computes Node pixel-level metrics.
+
+    :param truth: A list of the ground truth Nodes.
+
+    :param prediction: A list of the predicted Nodes.
+
+    :returns: Three matrices with shape ``(len(truth), len(prediction)``:
+        recall, precision, and f-score for each truth/prediction Node
+        pair. Truth Nodes are rows, prediction columns.
+    """
+    recall = numpy.zeros((len(truth), len(prediction)))
+    precision = numpy.zeros((len(truth), len(prediction)))
+    fscore = numpy.zeros((len(truth), len(prediction)))
+
+    for i, t in enumerate(truth):
+        for j, p in enumerate(prediction):
+            r, p, f = pixel_metrics(t, p)
+            recall[i, j] = r
+            precision[i, j] = p
+            fscore[i, j] = f
+
+    return recall, precision, fscore
+
+
+def align_nodes(truth: List[Node], prediction: List[Node], fscore=None) -> List[Tuple[int, int]]:
+    """Aligns prediction Nodes to truth.
+
+    :param truth: A list of the ground truth Nodes.
+
+    :param prediction: A list of the predicted Nodes.
+
+    :returns: A list of (t, p) pairs of Node indices into
+        the truth and prediction lists. There will be one
+        pair for each predicted symbol.
+    """
+    if fscore is None:
+        _, _, fscore = compute_recall_precision_fscore(truth, prediction)
+
+    # For each prediction (column), pick the highest-scoring
+    # True symbol.
+    closest_truths = list(fscore.argmax(axis=0))
+
+    # Checking for duplicate "best ground truth" alignments.
+    # This does *not* check for duplicates in the sense
+    # "multiple predictions aligned to the same truth"
+    # or "multiple truths aligned to the same prediction",
+    # it only acts as a tie-breaker in case one prediction overlaps
+    # to the same degree multiple truth objects (e.g. a single sharp
+    # in a key signature).
+    closest_truth_distance = [fscore[ct, j]
+                              for j, ct in enumerate(closest_truths)]
+    equidistant_closest_truths = [[i for i, x in enumerate(fscore[:, j])
+                                   if x == ct]
+                                  for j, ct in enumerate(closest_truth_distance)]
+
+    class_name_aware_closest_truths = []
+    for j, ects in enumerate(equidistant_closest_truths):
+        best_truth_i = int(ects[0])
+
+        # If there is more than one tied best choice,
+        # try to choose the truth Node that has the same
+        # class as the predicted Node.
+        if len(ects) > 1:
+            ects_c = {truth[int(i)].class_name: i for i in ects}
+            j_class_name = prediction[j].class_name
+            if j_class_name in ects_c:
+                best_truth_i = int(ects_c[j_class_name])
+
+        class_name_aware_closest_truths.append(best_truth_i)
+
+    alignment = [(t, p) for p, t in enumerate(class_name_aware_closest_truths)]
+    return alignment
+
+
+def compute_recall_precision_fscore_given_an_alignment(alignment: List[Tuple[int, int]], individual_recalls,
+                                                       individual_precisions, n_not_aligned: int = 0,
+                                                       strict_classnames: bool = True,
+                                                       truths: List[Node] = None, predictions: List[Node] = None)\
+        -> Tuple[float, float, float]:
+    if strict_classnames:
+        if not truths:
+            raise ValueError('If strict_classnames is requested, must supply truths Nodes!')
+        if not predictions:
+            raise ValueError('If strict_classnames is requested, must supply predictions Nodes!')
+
+    total_recall, total_precision = 0, 0
+
+    for i, j in alignment:
+
+        # Check for strict_classnames only at this stage.
+        # The purpose is: if two people mark the same object
+        # differently, we do want to know "it should be aligned
+        # to each other, but the classes don't fit" -- we don't
+        # want to maybe align it to an overlapping object of
+        # the corresponding wrong class.
+        if strict_classnames:
+            t_c = truths[i]
+            p_c = predictions[j]
+            if t_c.class_name != p_c.class_name:
+                continue
+
+        total_recall += individual_recalls[i, j]
+        total_precision += individual_precisions[i, j]
+
+    # This is not correct...? What about the zeros?
+    #  - Prediction with no GT is in the alignment, so it counts towards
+    #    the len(alignment) denominator.
+    #  - GT with no prediction aligned to it contributes zero, but is
+    #    not counted towards the denominator.
+    total_recall /= len(alignment) + n_not_aligned
+    total_precision /= len(alignment) + n_not_aligned
+
+    if (total_recall == 0) or (total_precision == 0):
+        total_fscore = 0.0
+    else:
+        total_fscore = 2 * total_recall * total_precision / (total_recall + total_precision)
+    return total_recall, total_precision, total_fscore
+
+
+##############################################################################
+
+
+def build_argument_parser():
+    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+
+    parser.add_argument('-t', '--true', action='store', required=True,
+                        help='The Nodes file you want to consider'
+                             ' ground truth.')
+    parser.add_argument('-p', '--prediction', action='store', required=True,
+                        help='The Nodes file you want to consider'
+                             ' the prediction.')
+
+    parser.add_argument('-e', '--export', action='store',
+                        help='If set, will export the problematic Nodes'
+                             ' to this file.')
+
+    parser.add_argument('--analyze_alignment', action='store_true',
+                        help='If set, will check whether the alignment is 1:1,'
+                             ' and print out the irregularities.')
+    parser.add_argument('--analyze_classnames', action='store_true',
+                        help='If set, will check whether the Nodes aligned'
+                             ' to each other have the same class labels'
+                             ' and print out the irregularities.')
+    parser.add_argument('--no_strict_classnames', action='store_true',
+                        help='If set, will not require aligned objects\' classnames'
+                             ' to match before computing pixel-wise overlap'
+                             ' metrics.')
+    parser.add_argument('--log_alignment', action='store_true',
+                        help='Print how the true and predicted objects are'
+                             ' paired.')
+
+    parser.add_argument('--print_fscore_only', action='store_true',
+                        help='If set, only print the total F-score number.'
+                             ' Useful for using in an automated pipeline.')
+
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='Turn on INFO messages.')
+    parser.add_argument('--debug', action='store_true',
+                        help='Turn on DEBUG messages.')
+
+    return parser
+
+
+def main(args):
+    logging.info('Starting main...')
+    _start_time = time.clock()
+
+    # The algorithm:
+    #  - build the cost function(s) for a pair of Nodes
+    #  - align the objects, using the cost function
+
+    # First alignment: try just matching a predicted object to the nearest
+    # true object.
+    # First distance function: proportion of shared pixels.
+    # Rule: if two objects don't share a pixel, they cannot be considered related.
+    # Object classes do not factor into this so far.
+
+    ground_truth_nodes = read_nodes_from_file(args.true)
+    predicted_nodes = read_nodes_from_file(args.prediction)
+
+    _parse_time = time.clock()
+    logging.info('Parsing {0} true and {1} prediction Nodes took {2:.2f} s'
+                 ''.format(len(ground_truth_nodes), len(predicted_nodes), _parse_time - _start_time))
+
+    recall, precision, fscore = compute_recall_precision_fscore(ground_truth_nodes, predicted_nodes)
+
+    _rpf_time = time.clock()
+    logging.info('Computing {0} entries of r/p/f matrices took {1:.2f} s'
+                 ''.format(len(ground_truth_nodes) * len(predicted_nodes), _rpf_time - _parse_time))
+
+    alignment_tp = align_nodes(ground_truth_nodes, predicted_nodes, fscore=fscore)
+    alignment_pt = align_nodes(predicted_nodes, ground_truth_nodes, fscore=fscore.T)
+
+    # Intersect alignments
+    _aln_tp_set = frozenset(alignment_tp)
+    alignment_tp_symmetric = [(t, p) for p, t in alignment_pt
+                              if (t, p) in _aln_tp_set
+                              and (ground_truth_nodes[t].class_name == predicted_nodes[p].class_name)]
+    truth_not_aligned = [t for p, t in alignment_pt
+                         if (t, p) not in alignment_tp_symmetric]
+    n_truth_not_aligned = len(truth_not_aligned)
+    preds_not_aligned = [p for t, p in alignment_tp
+                         if (t, p) not in alignment_tp_symmetric]
+    n_preds_not_aligned = len(preds_not_aligned)
+    n_not_aligned = n_truth_not_aligned + n_preds_not_aligned
+
+    _aln_time = time.clock()
+    logging.info('Computing alignment took {0:.2f} s'
+                 ''.format(_aln_time - _rpf_time))
+
+    # Now compute agreement: precision and recall on pixels
+    # of the aligned Nodes.
+
+    # We apply strict classnames only here, after the Nodes have been
+    # aligned to each other using pixel metrics.
+    strict_classnames = (not args.no_strict_classnames)
+    total_r, total_p, total_f = compute_recall_precision_fscore_given_an_alignment(alignment_tp_symmetric, recall, precision,
+                                                                                   n_not_aligned=n_not_aligned,
+                                                                                   strict_classnames=strict_classnames,
+                                                                                   truths=ground_truth_nodes,
+                                                                                   predictions=predicted_nodes)
+
+    if not args.print_fscore_only:
+        print('Truth objs.:\t{0}'.format(len(ground_truth_nodes)))
+        print('Pred. objs.:\t{0}'.format(len(predicted_nodes)))
+        print('Aligned objs.:\t{0}'.format(len(alignment_tp_symmetric)))
+        print('==============================================')
+        print('Recall:\t\t{0:.3f}\nPrecision:\t{1:.3f}\nF-score:\t{2:.3f}'
+              ''.format(total_r, total_p, total_f))
+        print('')
+    else:
+        print('{0:.3f}'.format(total_f))
+        return
+
+    if args.log_alignment:
+        print('==============================================')
+        print('Alignments:\n{0}'.format('\n'.join([
+            '({0}: {1}) -- ({2}: {3})'.format(ground_truth_nodes[t].id, ground_truth_nodes[t].class_name,
+                                              predicted_nodes[p].id, predicted_nodes[p].class_name)
+            for t, p in alignment_tp_symmetric
+        ])))
+        print('Truth, not aligned:\n{0}'.format('\n'.join(['({0}: {1})'.format(ground_truth_nodes[t].id, ground_truth_nodes[t].class_name)
+                                                           for t in truth_not_aligned])))
+        print(
+            'Preds, not aligned:\n{0}'.format('\n'.join(['({0}: {1})'.format(predicted_nodes[p].id, predicted_nodes[p].class_name)
+                                                         for p in preds_not_aligned])))
+
+    ##########################################################################
+    # Check if the alignment is a pairing -- find truth objects
+    # with more than one prediction aligned to them.
+    if args.analyze_alignment:
+        t_aln_dict = collections.defaultdict(list)
+        for i, j in alignment_tp_symmetric:
+            t_aln_dict[i].append(predicted_nodes[j])
+
+        multiple_truths = [ground_truth_nodes[i] for i in t_aln_dict
+                           if len(t_aln_dict[i]) > 1]
+        multiple_truths_aln_dict = {t: t_aln_dict[t]
+                                    for t in t_aln_dict
+                                    if len(t_aln_dict[t]) > 1}
+
+        print('Truth multi-aligned Node classes:\n{0}'
+              ''.format(pprint.pformat(
+            {(ground_truth_nodes[t].id, ground_truth_nodes[t].class_name): [(p.id, p.class_name)
+                                                  for p in t_aln_dict[t]]
+             for t in multiple_truths_aln_dict})))
+
+    ##########################################################################
+    # Check if the aligned objects have the same classes
+    if args.analyze_classnames:
+        different_classnames_pairs = []
+        for i, j in alignment_tp_symmetric:
+            if ground_truth_nodes[i].class_name != predicted_nodes[j].class_name:
+                different_classnames_pairs.append((ground_truth_nodes[i], predicted_nodes[j]))
+        print('Aligned pairs with different class_names:\n{0}'
+              ''.format('\n'.join(['{0}.{1}\t{2}.{3}'
+                                   ''.format(t.id, t.class_name, p.id, p.class_name)
+                                   for t, p in different_classnames_pairs])))
+
+    _end_time = time.clock()
+    logging.info('analyze_agreement.py done in {0:.3f} s'.format(_end_time - _start_time))
+
+
+if __name__ == '__main__':
+    parser = build_argument_parser()
+    args = parser.parse_args()
+
+    if args.verbose:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
+    if args.debug:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
+
+    main(args)
```

### Comparing `mung-1.1/scripts/analyze_tracking_log.py` & `mung-1.2/scripts/analyze_tracking_log.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,442 +1,442 @@
-"""``analyze_tracking_log.py`` is a script that performs a quick and dirty analysis
-of a MUSCIMarker event log. It is not necessary for using the dataset,
-but you might want it running if you are annotating something with MUSCIMarker.
-
-For an overview of command-line options, call::
-
-  analyze_tracking_log.py -h
-
-What does the script track?
-
-* Number of minutes/hours worked
-* Speed: how much was done in total?
-* Densities: frequency of events (calls) per minute/hour
-
-Visualizations:
-
-* Timing visualization
-
-Also, convert to CSV, to make it grep-able? First: fixed-name cols,
-then: args dict, formatted as key=value,key=value
-
-"""
-import argparse
-import codecs
-import collections
-import itertools
-import json
-import logging
-import operator
-import os
-import pprint
-import time
-
-import matplotlib.pyplot as plt
-import numpy
-from typing import Dict, Tuple
-
-from mung.io import read_nodes_from_file
-
-
-def freqdict(l, sort=True) -> Dict:
-    out = collections.defaultdict(int)
-    for item in l:
-        out[item] += 1
-    if sort:
-        s_out = collections.OrderedDict()
-        for k, v in sorted(list(out.items()), key=operator.itemgetter(1), reverse=True):
-            s_out[k] = v
-        out = s_out
-    return out
-
-
-##############################################################################
-
-def is_annotation_package(path):
-    """Checks that the given path is an annotation package."""
-    if not os.path.isdir(path):
-        return False
-    subdirs = os.listdir(path)
-    if 'source_images' not in subdirs:
-        return False
-    if 'annotations' not in subdirs:
-        return False
-    if 'annotation_logs' not in subdirs:
-        return False
-    return True
-
-
-def logs_from_package(package):
-    """Collects all log file names (with complete paths) from the given package.
-
-    :param package: Path to the annotations package.
-
-    :return: List of filenames (full paths).
-    """
-    logging.info('Collecting log files from package {0}'.format(package))
-    if not os.path.isdir(package):
-        raise OSError('Package {0} not found!'.format(package))
-    log_path = os.path.join(package, 'annotation_logs')
-    if not os.path.isdir(log_path):
-        raise ValueError('Package {0}: annotation_logs not found, probably not a package.'
-                         ''.format(package))
-    # Collect all log days
-    log_days = os.listdir(log_path)
-
-    # Dealing with people who copied the entire .muscimarker-tracking directory
-    # (potentially without the dot, as just "muscimarker-tracking")
-    if len(log_days) == 0:
-        logging.info('No logs in package {0}!'.format(package))
-        return []
-
-    if log_days[-1].endswith('muscimarker-tracking'):
-        log_path = os.path.join(log_path, log_days[-1])
-        log_days = os.listdir(log_path)
-
-    log_files = []
-    for day in log_days:
-
-        # .DS_store and other hidden files
-        if day.startswith('.'):
-            continue
-
-        # Dealing with people who copied only the JSON files
-        if day.endswith('json'):
-            logging.info('Found log file that is not inside a day dir: {0}'
-                         ''.format(day))
-            log_files.append(os.path.join(log_path, day))
-            continue
-
-        if day.endswith('xml'):
-            logging.info('Log file is for some reason XML instead of JSON; copied wrong files???')
-            continue
-
-        day_log_path = os.path.join(log_path, day)
-        day_log_files = [os.path.join(day_log_path, l)
-                         for l in os.listdir(day_log_path)]
-        log_files += day_log_files
-    logging.info('In package {0}: found {1} log files.'
-                 ''.format(package, len(log_files)))
-    logging.debug('In package {0}: log files:\n{1}'
-                  ''.format(package, pprint.pformat(log_files)))
-    return log_files
-
-
-def try_correct_crashed_json(fname):
-    """Attempts to correct an incomplete JSON list file: if MUSCIMarker
-    crashed, the items list would not get correctly closed. We attempt
-    to remove the last comma and add a closing bracket (`]`) on a new
-    line instead, and return the object as a (unicode) string.
-
-    >>> json = '''
-    ... [
-    ...   {'something': 'this', 'something': 'that'},'''
-
-    """
-    with open(fname, 'r') as hdl:
-        lines = [l.rstrip() for l in hdl]
-    if lines[-1][-1] == ',':
-        logging.info('Correcting JSON: found hanging comma!')
-        lines[-1] = lines[-1][:-1]
-        lines.append(']')
-        return '\n'.join(lines)
-
-    else:
-        logging.info('No hanging comma, cannot deal with this situation.')
-        return None
-
-
-def unique_logs(event_logs):
-    """Checks that the event logs are unique using the start event
-    timestamp. Returns a list of unique event logs. If two have the same
-    timestamp, the first one is used.
-
-    For logging purposes, expects a dict of event logs. Keys are log file names,
-    values are the event lists.
-    """
-    unique = collections.OrderedDict()
-    for log_file, l in event_logs.items():
-        if len(l) < 1:
-            logging.info('Got an empty log from file {0}'.format(log_file))
-            continue
-        init_event = l[0]
-        if '-time-' not in init_event:
-            raise ValueError('Got a non-event log JSON list, file {0}! Supposed init event: {1}'
-                             ''.format(log_file, init_event))
-        init_time = init_event['-time-']
-        if init_time in unique:
-            logging.info('Found non-unique event log {0} with timestamp {1} ({2} events)!'
-                         ' Using first ({3} events).'
-                         ''.format(log_file, init_time, len(l), len(unique[init_time])))
-        else:
-            unique[init_time] = l
-    return list(unique.values())
-
-
-##############################################################################
-# Counting results
-
-
-def annotations_from_package(package: str):
-    """Collect all annotation XML files (with complete paths)
-    from the given package."""
-    logging.info('Collecting annotation files from package {0}'.format(package))
-    if not os.path.isdir(package):
-        raise OSError('Package {0} not found!'.format(package))
-    annot_path = os.path.join(package, 'annotations')
-    if not os.path.isdir(annot_path):
-        raise ValueError('Package {0}: annotations not found, probably not a package.'
-                         ''.format(package))
-
-    # Collect all annotations
-    annotation_files = [os.path.join(annot_path, f)
-                        for f in os.listdir(annot_path) if f.endswith('.xml')]
-    return annotation_files
-
-
-def count_nodes(annot_file):
-    return len(read_nodes_from_file(annot_file))
-
-
-def count_nodes_and_relationships(annot_file: str) -> Tuple[int, int]:
-    nodes = read_nodes_from_file(annot_file)
-    n_inlinks = 0
-    for node in nodes:
-        if node.inlinks is not None:
-            n_inlinks += len(node.inlinks)
-    return len(nodes), n_inlinks
-
-
-##############################################################################
-# Visualization
-
-def events_by_time_units(events, seconds_per_unit=60):
-    """Puts the events into bins that correspond to equally spaced
-    intervals of time. The length of time covered by one bin is
-    given by seconds_per_unit."""
-    # Get first event time
-    start_time = min([float(e['-time-']) for e in events])
-
-    # The events do not have to come in-order
-    bins = collections.defaultdict(list)
-    for e in events:
-        t = float(e['-time-'])
-        n_bin = int(t - start_time) // int(seconds_per_unit)
-        bins[n_bin].append(e)
-
-    return bins
-
-
-def plot_events_by_time(events, type_key='-fn-'):
-    """Simple scatterplot visualization.
-
-    All events are expected to have a -fn- component."""
-    fns = [e['-fn-'] for e in events]
-    # Assign numbers to tracked fns
-    fns_by_freq = {f: len([e for e in fns if e == f]) for f in set(fns)}
-    fn_dict = {f: i for i, f in enumerate(sorted(list(fns_by_freq.keys()),
-                                                 reverse=True,
-                                                 key=lambda k: fns_by_freq[k]))}
-
-    min_time = float(events[0]['-time-'])
-
-    dataset = numpy.zeros((len(events), 2))
-    for i, e in enumerate(events):
-        dataset[i][0] = float(e['-time-']) - min_time
-        dataset[i][1] = fn_dict[e[type_key]]
-
-    # Now visualize
-    plt.scatter(dataset[:, 0], dataset[:, 1])
-
-
-def format_as_timeflow_csv(events, delimiter='\t'):
-    """There is a cool offline visualization tool caled TimeFlow,
-    which has a timeline app. It needs a pretty specific CSV format
-    to work, though."""
-    # What we need:
-    #  - ID
-    #  - Date (human?)
-    #  - The common fields:
-    min_second = int(min([float(e['-time-']) for e in events]))
-
-    def format_date(e):
-        # return '-'.join(reversed(time_human.replace(':', '-').split('__')))
-        # time_human = e['-time-human-']
-        time = float(e['-time-'])
-        return str(int(time) - min_second)
-
-    # Collect all events that are in the data.
-    event_fields = freqdict(list(itertools.chain(*[list(e.keys()) for e in events])))
-    output_fields = ['ID', 'Date'] + list(event_fields.keys())
-    n_fields = len(output_fields)
-
-    field2idx = {f: i + 2 for i, f in enumerate(event_fields.keys())}
-    event_table = [['' for _ in range(n_fields)] for _ in events]
-    for i, e in enumerate(events):
-        event_table[i][0] = str(i)
-        event_table[i][1] = format_date(e)  # format_date(e['-time-human-'])
-        for k, v in e.items():
-            event_table[i][field2idx[k]] = v
-
-    # Add labels to event table to get the complete data
-    # that should be formatted as TSV
-    output_data = [output_fields] + event_table
-    output_lines = ['\t'.join(row) for row in output_data]
-    output_string = '\n'.join(output_lines)
-    return output_string
-
-
-##############################################################################
-
-
-def build_argument_parser():
-    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-
-    parser.add_argument('-i', '--inputs', nargs='+', action='store',
-                        help='Log files to be analyzed.')
-    parser.add_argument('-p', '--packages', nargs='+', action='store',
-                        help='Annotation package. If set, will pull'
-                             ' all log files in the package.')
-    parser.add_argument('-a', '--annotator', action='store',
-                        help='Annotator. If set, will pull all log files'
-                             ' from all packages in the given person\'s'
-                             ' annotation directory')
-
-    parser.add_argument('-c', '--count_annotations', action='store_true',
-                        help='If given, will collect annotation files from the'
-                             ' supplied packages (or per-annotator packages)'
-                             ' and compute object/rel counts and efficiency statistics.')
-    parser.add_argument('--no_training', action='store_true',
-                        help='If given, will ignore packages with "training" in their name.')
-
-    parser.add_argument('-v', '--verbose', action='store_true',
-                        help='Turn on INFO messages.')
-    parser.add_argument('--debug', action='store_true',
-                        help='Turn on DEBUG messages.')
-
-    return parser
-
-
-def main(args):
-    logging.info('Starting main...')
-    _start_time = time.clock()
-
-    if args.annotator is not None:
-        logging.info('Collecting annotation packages for annotator {0}'
-                     ''.format(args.annotator))
-        # Collect all packages, incl. training
-        packages = []
-        for d in os.listdir(args.annotator):
-            package_candidate = os.path.join(args.annotator, d)
-            if not is_annotation_package(package_candidate):
-                continue
-            packages.append(package_candidate)
-
-        logging.info('Found: {0} packages'.format(len(packages)))
-
-        args.packages = packages
-
-    if args.packages is not None:
-        logging.info('Collecting log files for {0} packages.'.format(len(args.packages)))
-        log_files = []
-        for package in args.packages:
-            current_log_files = logs_from_package(package)
-            log_files += current_log_files
-
-        logging.info('Found: {0} log files'.format(len(log_files)))
-        args.input = log_files
-
-    log_data_per_file = {}
-    for input_file in args.input:
-        if not os.path.isfile(input_file):
-            raise ValueError('Log file {0} not found!'.format(input_file))
-
-        current_log_data = []
-
-        with codecs.open(input_file, 'r', 'utf-8') as hdl:
-            try:
-                current_log_data = json.load(hdl)
-
-            except ValueError:
-                logging.info('Could not parse JSON file {0}'.format(input_file))
-                logging.info('Attempting to correct file.')
-                corrected = try_correct_crashed_json(input_file)
-                if corrected is not None:
-                    logging.info('Attempting to parse corrected JSON.')
-                    try:
-                        current_log_data = json.loads(corrected)
-                    except ValueError:
-                        logging.warning('Could not even parse corrected JSON, skipping file {0}.'.format(input_file))
-                        # raise
-                    logging.info('Success!')
-                else:
-                    logging.info('Unable to correct JSON, skipping file.')
-
-        log_data_per_file[input_file] = current_log_data
-
-    logging.info('Checking logs for uniqueness. Started with {0} log files.'
-                 ''.format(len(log_data_per_file)))
-    log_data_per_file = unique_logs(log_data_per_file)
-    logging.info('After uniqueness check: {0} logs left.'.format(len(log_data_per_file)))
-
-    log_data = [e for e in itertools.chain(*log_data_per_file)]
-    if len(log_data) == 0:
-        print('Received no log data! Skipping ahead to count annotations.')
-        n_minutes = None
-        n_hours = None
-    else:
-        logging.info('Parsed {0} data items.'.format(len(log_data)))
-        # Your code goes here
-        # raise NotImplementedError()
-
-        # Frequency by -fn-:
-        freq_by_fn = freqdict([l.get('-fn-', None) for l in log_data])
-
-        by_minute = events_by_time_units(log_data)
-        by_minute_freq = {k: len(v) for k, v in list(by_minute.items())}
-        n_minutes = len(by_minute)
-
-        print('# minutes worked: {0}'.format(n_minutes))
-        n_hours = n_minutes / 60.0
-        print('# hours worked: {0:.2f}'.format(n_hours))
-        print('CZK@120: {0:.3f}'.format(n_hours * 120))
-        print('CZK@150: {0:.3f}'.format(n_hours * 150))
-        print('CZK@180: {0:.3f}'.format(n_hours * 180))
-        print('Avg. events per minute: {0}'.format(float(len(log_data)) / n_minutes))
-
-    if args.count_annotations:
-        if args.packages is None:
-            raise ValueError('Cannot count annotations if no packages are given!')
-
-        number_of_nodes = 0
-        number_of_relationships = 0
-        for package in args.packages:
-            annot_files = annotations_from_package(package)
-            for f in annot_files:
-                n_c, n_r = count_nodes_and_relationships(f)
-                number_of_nodes += n_c
-                number_of_relationships += n_r
-
-        print('Total Nodes: {0}'.format(number_of_nodes))
-        print('Total Relationships: {0}'.format(number_of_relationships))
-        if n_minutes is not None:
-            print('Nodes per minute: {0:.2f}'.format(number_of_nodes / float(n_minutes)))
-
-    _end_time = time.clock()
-    logging.info('analyze_tracking_log.py done in {0:.3f} s'.format(_end_time - _start_time))
-
-
-##############################################################################
-
-
-if __name__ == '__main__':
-    parser = build_argument_parser()
-    args = parser.parse_args()
-
-    if args.verbose:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
-    if args.debug:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
-
-    main(args)
+"""``analyze_tracking_log.py`` is a script that performs a quick and dirty analysis
+of a MUSCIMarker event log. It is not necessary for using the dataset,
+but you might want it running if you are annotating something with MUSCIMarker.
+
+For an overview of command-line options, call::
+
+  analyze_tracking_log.py -h
+
+What does the script track?
+
+* Number of minutes/hours worked
+* Speed: how much was done in total?
+* Densities: frequency of events (calls) per minute/hour
+
+Visualizations:
+
+* Timing visualization
+
+Also, convert to CSV, to make it grep-able? First: fixed-name cols,
+then: args dict, formatted as key=value,key=value
+
+"""
+import argparse
+import codecs
+import collections
+import itertools
+import json
+import logging
+import operator
+import os
+import pprint
+import time
+
+import matplotlib.pyplot as plt
+import numpy
+from typing import Dict, Tuple
+
+from mung.io import read_nodes_from_file
+
+
+def freqdict(l, sort=True) -> Dict:
+    out = collections.defaultdict(int)
+    for item in l:
+        out[item] += 1
+    if sort:
+        s_out = collections.OrderedDict()
+        for k, v in sorted(list(out.items()), key=operator.itemgetter(1), reverse=True):
+            s_out[k] = v
+        out = s_out
+    return out
+
+
+##############################################################################
+
+def is_annotation_package(path):
+    """Checks that the given path is an annotation package."""
+    if not os.path.isdir(path):
+        return False
+    subdirs = os.listdir(path)
+    if 'source_images' not in subdirs:
+        return False
+    if 'annotations' not in subdirs:
+        return False
+    if 'annotation_logs' not in subdirs:
+        return False
+    return True
+
+
+def logs_from_package(package):
+    """Collects all log file names (with complete paths) from the given package.
+
+    :param package: Path to the annotations package.
+
+    :return: List of filenames (full paths).
+    """
+    logging.info('Collecting log files from package {0}'.format(package))
+    if not os.path.isdir(package):
+        raise OSError('Package {0} not found!'.format(package))
+    log_path = os.path.join(package, 'annotation_logs')
+    if not os.path.isdir(log_path):
+        raise ValueError('Package {0}: annotation_logs not found, probably not a package.'
+                         ''.format(package))
+    # Collect all log days
+    log_days = os.listdir(log_path)
+
+    # Dealing with people who copied the entire .muscimarker-tracking directory
+    # (potentially without the dot, as just "muscimarker-tracking")
+    if len(log_days) == 0:
+        logging.info('No logs in package {0}!'.format(package))
+        return []
+
+    if log_days[-1].endswith('muscimarker-tracking'):
+        log_path = os.path.join(log_path, log_days[-1])
+        log_days = os.listdir(log_path)
+
+    log_files = []
+    for day in log_days:
+
+        # .DS_store and other hidden files
+        if day.startswith('.'):
+            continue
+
+        # Dealing with people who copied only the JSON files
+        if day.endswith('json'):
+            logging.info('Found log file that is not inside a day dir: {0}'
+                         ''.format(day))
+            log_files.append(os.path.join(log_path, day))
+            continue
+
+        if day.endswith('xml'):
+            logging.info('Log file is for some reason XML instead of JSON; copied wrong files???')
+            continue
+
+        day_log_path = os.path.join(log_path, day)
+        day_log_files = [os.path.join(day_log_path, l)
+                         for l in os.listdir(day_log_path)]
+        log_files += day_log_files
+    logging.info('In package {0}: found {1} log files.'
+                 ''.format(package, len(log_files)))
+    logging.debug('In package {0}: log files:\n{1}'
+                  ''.format(package, pprint.pformat(log_files)))
+    return log_files
+
+
+def try_correct_crashed_json(fname):
+    """Attempts to correct an incomplete JSON list file: if MUSCIMarker
+    crashed, the items list would not get correctly closed. We attempt
+    to remove the last comma and add a closing bracket (`]`) on a new
+    line instead, and return the object as a (unicode) string.
+
+    >>> json = '''
+    ... [
+    ...   {'something': 'this', 'something': 'that'},'''
+
+    """
+    with open(fname, 'r') as hdl:
+        lines = [l.rstrip() for l in hdl]
+    if lines[-1][-1] == ',':
+        logging.info('Correcting JSON: found hanging comma!')
+        lines[-1] = lines[-1][:-1]
+        lines.append(']')
+        return '\n'.join(lines)
+
+    else:
+        logging.info('No hanging comma, cannot deal with this situation.')
+        return None
+
+
+def unique_logs(event_logs):
+    """Checks that the event logs are unique using the start event
+    timestamp. Returns a list of unique event logs. If two have the same
+    timestamp, the first one is used.
+
+    For logging purposes, expects a dict of event logs. Keys are log file names,
+    values are the event lists.
+    """
+    unique = collections.OrderedDict()
+    for log_file, l in event_logs.items():
+        if len(l) < 1:
+            logging.info('Got an empty log from file {0}'.format(log_file))
+            continue
+        init_event = l[0]
+        if '-time-' not in init_event:
+            raise ValueError('Got a non-event log JSON list, file {0}! Supposed init event: {1}'
+                             ''.format(log_file, init_event))
+        init_time = init_event['-time-']
+        if init_time in unique:
+            logging.info('Found non-unique event log {0} with timestamp {1} ({2} events)!'
+                         ' Using first ({3} events).'
+                         ''.format(log_file, init_time, len(l), len(unique[init_time])))
+        else:
+            unique[init_time] = l
+    return list(unique.values())
+
+
+##############################################################################
+# Counting results
+
+
+def annotations_from_package(package: str):
+    """Collect all annotation XML files (with complete paths)
+    from the given package."""
+    logging.info('Collecting annotation files from package {0}'.format(package))
+    if not os.path.isdir(package):
+        raise OSError('Package {0} not found!'.format(package))
+    annot_path = os.path.join(package, 'annotations')
+    if not os.path.isdir(annot_path):
+        raise ValueError('Package {0}: annotations not found, probably not a package.'
+                         ''.format(package))
+
+    # Collect all annotations
+    annotation_files = [os.path.join(annot_path, f)
+                        for f in os.listdir(annot_path) if f.endswith('.xml')]
+    return annotation_files
+
+
+def count_nodes(annot_file):
+    return len(read_nodes_from_file(annot_file))
+
+
+def count_nodes_and_relationships(annot_file: str) -> Tuple[int, int]:
+    nodes = read_nodes_from_file(annot_file)
+    n_inlinks = 0
+    for node in nodes:
+        if node.inlinks is not None:
+            n_inlinks += len(node.inlinks)
+    return len(nodes), n_inlinks
+
+
+##############################################################################
+# Visualization
+
+def events_by_time_units(events, seconds_per_unit=60):
+    """Puts the events into bins that correspond to equally spaced
+    intervals of time. The length of time covered by one bin is
+    given by seconds_per_unit."""
+    # Get first event time
+    start_time = min([float(e['-time-']) for e in events])
+
+    # The events do not have to come in-order
+    bins = collections.defaultdict(list)
+    for e in events:
+        t = float(e['-time-'])
+        n_bin = int(t - start_time) // int(seconds_per_unit)
+        bins[n_bin].append(e)
+
+    return bins
+
+
+def plot_events_by_time(events, type_key='-fn-'):
+    """Simple scatterplot visualization.
+
+    All events are expected to have a -fn- component."""
+    fns = [e['-fn-'] for e in events]
+    # Assign numbers to tracked fns
+    fns_by_freq = {f: len([e for e in fns if e == f]) for f in set(fns)}
+    fn_dict = {f: i for i, f in enumerate(sorted(list(fns_by_freq.keys()),
+                                                 reverse=True,
+                                                 key=lambda k: fns_by_freq[k]))}
+
+    min_time = float(events[0]['-time-'])
+
+    dataset = numpy.zeros((len(events), 2))
+    for i, e in enumerate(events):
+        dataset[i][0] = float(e['-time-']) - min_time
+        dataset[i][1] = fn_dict[e[type_key]]
+
+    # Now visualize
+    plt.scatter(dataset[:, 0], dataset[:, 1])
+
+
+def format_as_timeflow_csv(events, delimiter='\t'):
+    """There is a cool offline visualization tool caled TimeFlow,
+    which has a timeline app. It needs a pretty specific CSV format
+    to work, though."""
+    # What we need:
+    #  - ID
+    #  - Date (human?)
+    #  - The common fields:
+    min_second = int(min([float(e['-time-']) for e in events]))
+
+    def format_date(e):
+        # return '-'.join(reversed(time_human.replace(':', '-').split('__')))
+        # time_human = e['-time-human-']
+        time = float(e['-time-'])
+        return str(int(time) - min_second)
+
+    # Collect all events that are in the data.
+    event_fields = freqdict(list(itertools.chain(*[list(e.keys()) for e in events])))
+    output_fields = ['ID', 'Date'] + list(event_fields.keys())
+    n_fields = len(output_fields)
+
+    field2idx = {f: i + 2 for i, f in enumerate(event_fields.keys())}
+    event_table = [['' for _ in range(n_fields)] for _ in events]
+    for i, e in enumerate(events):
+        event_table[i][0] = str(i)
+        event_table[i][1] = format_date(e)  # format_date(e['-time-human-'])
+        for k, v in e.items():
+            event_table[i][field2idx[k]] = v
+
+    # Add labels to event table to get the complete data
+    # that should be formatted as TSV
+    output_data = [output_fields] + event_table
+    output_lines = ['\t'.join(row) for row in output_data]
+    output_string = '\n'.join(output_lines)
+    return output_string
+
+
+##############################################################################
+
+
+def build_argument_parser():
+    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+
+    parser.add_argument('-i', '--inputs', nargs='+', action='store',
+                        help='Log files to be analyzed.')
+    parser.add_argument('-p', '--packages', nargs='+', action='store',
+                        help='Annotation package. If set, will pull'
+                             ' all log files in the package.')
+    parser.add_argument('-a', '--annotator', action='store',
+                        help='Annotator. If set, will pull all log files'
+                             ' from all packages in the given person\'s'
+                             ' annotation directory')
+
+    parser.add_argument('-c', '--count_annotations', action='store_true',
+                        help='If given, will collect annotation files from the'
+                             ' supplied packages (or per-annotator packages)'
+                             ' and compute object/rel counts and efficiency statistics.')
+    parser.add_argument('--no_training', action='store_true',
+                        help='If given, will ignore packages with "training" in their name.')
+
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='Turn on INFO messages.')
+    parser.add_argument('--debug', action='store_true',
+                        help='Turn on DEBUG messages.')
+
+    return parser
+
+
+def main(args):
+    logging.info('Starting main...')
+    _start_time = time.clock()
+
+    if args.annotator is not None:
+        logging.info('Collecting annotation packages for annotator {0}'
+                     ''.format(args.annotator))
+        # Collect all packages, incl. training
+        packages = []
+        for d in os.listdir(args.annotator):
+            package_candidate = os.path.join(args.annotator, d)
+            if not is_annotation_package(package_candidate):
+                continue
+            packages.append(package_candidate)
+
+        logging.info('Found: {0} packages'.format(len(packages)))
+
+        args.packages = packages
+
+    if args.packages is not None:
+        logging.info('Collecting log files for {0} packages.'.format(len(args.packages)))
+        log_files = []
+        for package in args.packages:
+            current_log_files = logs_from_package(package)
+            log_files += current_log_files
+
+        logging.info('Found: {0} log files'.format(len(log_files)))
+        args.input = log_files
+
+    log_data_per_file = {}
+    for input_file in args.input:
+        if not os.path.isfile(input_file):
+            raise ValueError('Log file {0} not found!'.format(input_file))
+
+        current_log_data = []
+
+        with codecs.open(input_file, 'r', 'utf-8') as hdl:
+            try:
+                current_log_data = json.load(hdl)
+
+            except ValueError:
+                logging.info('Could not parse JSON file {0}'.format(input_file))
+                logging.info('Attempting to correct file.')
+                corrected = try_correct_crashed_json(input_file)
+                if corrected is not None:
+                    logging.info('Attempting to parse corrected JSON.')
+                    try:
+                        current_log_data = json.loads(corrected)
+                    except ValueError:
+                        logging.warning('Could not even parse corrected JSON, skipping file {0}.'.format(input_file))
+                        # raise
+                    logging.info('Success!')
+                else:
+                    logging.info('Unable to correct JSON, skipping file.')
+
+        log_data_per_file[input_file] = current_log_data
+
+    logging.info('Checking logs for uniqueness. Started with {0} log files.'
+                 ''.format(len(log_data_per_file)))
+    log_data_per_file = unique_logs(log_data_per_file)
+    logging.info('After uniqueness check: {0} logs left.'.format(len(log_data_per_file)))
+
+    log_data = [e for e in itertools.chain(*log_data_per_file)]
+    if len(log_data) == 0:
+        print('Received no log data! Skipping ahead to count annotations.')
+        n_minutes = None
+        n_hours = None
+    else:
+        logging.info('Parsed {0} data items.'.format(len(log_data)))
+        # Your code goes here
+        # raise NotImplementedError()
+
+        # Frequency by -fn-:
+        freq_by_fn = freqdict([l.get('-fn-', None) for l in log_data])
+
+        by_minute = events_by_time_units(log_data)
+        by_minute_freq = {k: len(v) for k, v in list(by_minute.items())}
+        n_minutes = len(by_minute)
+
+        print('# minutes worked: {0}'.format(n_minutes))
+        n_hours = n_minutes / 60.0
+        print('# hours worked: {0:.2f}'.format(n_hours))
+        print('CZK@120: {0:.3f}'.format(n_hours * 120))
+        print('CZK@150: {0:.3f}'.format(n_hours * 150))
+        print('CZK@180: {0:.3f}'.format(n_hours * 180))
+        print('Avg. events per minute: {0}'.format(float(len(log_data)) / n_minutes))
+
+    if args.count_annotations:
+        if args.packages is None:
+            raise ValueError('Cannot count annotations if no packages are given!')
+
+        number_of_nodes = 0
+        number_of_relationships = 0
+        for package in args.packages:
+            annot_files = annotations_from_package(package)
+            for f in annot_files:
+                n_c, n_r = count_nodes_and_relationships(f)
+                number_of_nodes += n_c
+                number_of_relationships += n_r
+
+        print('Total Nodes: {0}'.format(number_of_nodes))
+        print('Total Relationships: {0}'.format(number_of_relationships))
+        if n_minutes is not None:
+            print('Nodes per minute: {0:.2f}'.format(number_of_nodes / float(n_minutes)))
+
+    _end_time = time.clock()
+    logging.info('analyze_tracking_log.py done in {0:.3f} s'.format(_end_time - _start_time))
+
+
+##############################################################################
+
+
+if __name__ == '__main__':
+    parser = build_argument_parser()
+    args = parser.parse_args()
+
+    if args.verbose:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
+    if args.debug:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
+
+    main(args)
```

### Comparing `mung-1.1/scripts/baseline_process_symbols.py` & `mung-1.2/scripts/baseline_process_symbols.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,792 +1,788 @@
-"""This is a script that processes a set of symbols in order to obtain the pitch
-recognition baseline. Intended to be used on top of an object detection stage."""
-import argparse
-import collections
-import logging
-import os
-import pickle
-import pprint
-import time
-import traceback
-
-import numpy
-from sklearn.feature_extraction import DictVectorizer
-from typing import List, Dict, Tuple
-
-from mung.grammar import DependencyGrammar
-from mung.graph import find_beams_incoherent_with_stems, NotationGraph
-from mung.graph import find_contained_nodes, remove_contained_nodes
-from mung.graph import find_misdirected_leger_line_edges
-from mung2midi.inference import OnsetsInferenceEngine, MIDIBuilder, PitchInferenceEngine
-from mung.constants import InferenceEngineConstants as _CONST
-from mung.io import parse_node_classes, read_nodes_from_file, export_node_list
-from mung.node import bounding_box_intersection, merge_multiple_nodes, link_nodes, Node
-from mung.stafflines import merge_staffline_segments, build_staff_nodes, \
-    build_staffspace_nodes, \
-    add_staff_relationships
-
-
-def add_key_signatures(nodes: List[Node]) -> List[Node]:
-    """Heuristic for deciding which accidentals are inline,
-    and which should be interpreted as components of a key signature.
-
-    Assumes staffline relationships have already been inferred.
-
-    The heuristic is defined for each staff S as the following:
-
-    * Take the leftmost clef C.
-    * Take the leftmost notehead (incl. grace notes) N.
-    * Take all accidentals A_S that overlap the space between C and N
-      horizontally (including C, not including N), and overlap the staff.
-    * Order A_S left-to-right
-    * Set m = C
-    * Initialize key signature K_S = {}
-    * For each a_S in A_S:
-    * if it is closer to m than to N, then:
-    *   add a_S to K_S,
-    *   set m = a_S
-    * else:
-    *   break
-
-    Note that this modifies the accidentals and staffs in-place: they get inlinks
-    from their respective key signatures.
-    """
-    graph = NotationGraph(nodes)
-
-    new_node_id = max([m.id for m in nodes]) + 1
-
-    key_signatures = []
-
-    staffs = [m for m in nodes if m.class_name == _CONST.STAFF_CLASS_NAME]
-    for s in staffs:
-
-        # Take the leftmost clef C.
-        clefs = graph.parents(s.id, class_filter=_CONST.CLEF_CLASS_NAMES)
-        if len(clefs) == 0:
-            continue
-        leftmost_clef = min(clefs, key=lambda x: x.left)
-
-        # Take the leftmost notehead (incl. grace notes) N.
-        noteheads = graph.parents(s.id, class_filter=_CONST.NOTEHEAD_CLASS_NAMES)
-        if len(noteheads) == 0:
-            continue
-        leftmost_notehead = min(noteheads, key=lambda x: x.left)
-
-        # Take all accidentals A_S that fall between C and N
-        # horizontally, and overlap the staff.
-        all_accidentals = [m for m in nodes
-                           if m.class_name in _CONST.ACCIDENTAL_CLASS_NAMES]
-        relevant_acc_bbox = s.top, leftmost_clef.left, s.bottom, leftmost_notehead.left
-        relevant_accidentals = [m for m in all_accidentals
-                                if bounding_box_intersection(m.bounding_box,
-                                                             relevant_acc_bbox)
-                                is not None]
-
-        # Order A_S left-to-right.
-        ordered_accidentals = sorted(relevant_accidentals,
-                                     key=lambda x: x.left)
-
-        # Set m = C
-        current_lstop = leftmost_clef.right
-        key_signature_accidentals = []
-
-        # Iterate over accidentals; check if they are closer to lstop
-        # than to the first notehead
-        for a in ordered_accidentals:
-            if (a.left - current_lstop) < (leftmost_notehead.left - a.right):
-                key_signature_accidentals.append(a)
-                current_lstop = a.right
-            else:
-                break
-
-        # Build key signature and connect it to staff
-        if len(key_signature_accidentals) > 0:
-            key_signature_class_names = list(_CONST.KEY_SIGNATURE_CLASS_NAMES)[0]
-            # Note: there might be spurious links from the accidentals
-            # to notheads, if they were mis-interpreted during parsing.
-            # This actually might not matter; needs testing.
-            key_signature = merge_multiple_nodes(
-                key_signature_accidentals,
-                class_name=key_signature_class_names,
-                id_=new_node_id)
-            new_node_id += 1
-            link_nodes(key_signature, s)
-            for a in key_signature_accidentals:
-                link_nodes(key_signature, a)
-
-            key_signatures.append(key_signature)
-
-    logging.info('Adding {} key signatures'.format(len(key_signatures)))
-    return nodes + key_signatures
-
-
-##############################################################################
-# Feature extraction
-
-class PairwiseClassificationFeatureExtractor(object):
-    def __init__(self, vectorizer=None):
-        """Initialize the feature extractor.
-
-        :param vectorizer: A DictVectorizer() from scikit-learn.
-            Used to convert feature dicts to the vectors that
-            the edge classifier of the parser will expect.
-            If None, will create a new DictVectorizer. (This is useful
-            for training; you can then pickle the entire extractor
-            and make sure the feature extraction works for the classifier
-            at runtime.)
-        """
-        if vectorizer is None:
-            vectorizer = DictVectorizer()
-        self.vectorizer = vectorizer
-
-    def __call__(self, *args, **kwargs):
-        """The call is per item (in this case, Node pair)."""
-        fd = self.get_features_relative_bbox_and_clsname(*args, **kwargs)
-        # Compensate for the vecotrizer "target", which we don't have here (by :-1)
-        item_features = self.vectorizer.transform(fd).toarray()[0, :-1]
-        return item_features
-
-    def get_features_relative_bbox_and_clsname(self, c_from: Node, c_to: Node):
-        """Extract a feature vector from the given pair of Nodes.
-        Does *NOT* convert the class names to integers.
-
-        Features: bbox(c_to) - bbox(c_from), class_name(c_from), class_name(c_to)
-        Target: 1 if there is a link from u to v
-
-        Returns a dict that works as input to ``self.vectorizer``.
-        """
-        target = 0
-        if c_from.document == c_to.document:
-            if c_to.id in c_from.outlinks:
-                target = 1
-        features = (c_to.top - c_from.top,
-                    c_to.left - c_from.left,
-                    c_to.bottom - c_from.bottom,
-                    c_to.right - c_from.right,
-                    c_from.class_name,
-                    c_to.class_name,
-                    target)
-        dt, dl, db, dr, cu, cv, tgt = features
-        # Normalizing clsnames
-        if cu.startswith('letter'):
-            cu = 'letter'
-        if cu.startswith('numeral'):
-            cu = 'numeral'
-        if cv.startswith('letter'):
-            cv = 'letter'
-        if cv.startswith('numeral'):
-            cv = 'numeral'
-        feature_dict = {'dt': dt,
-                        'dl': dl,
-                        'db': db,
-                        'dr': dr,
-                        'cls_from': cu,
-                        'cls_to': cv,
-                        'target': tgt}
-        return feature_dict
-
-    def get_features_distance_relative_bbox_and_clsname(self, from_node: Node,
-                                                        to_node: Node) -> Dict:
-        """Extract a feature vector from the given pair of Nodes.
-        Does *NOT* convert the class names to integers.
-
-        Features: bbox(c_to) - bbox(c_from), class_name(c_from), class_name(c_to)
-        Target: 1 if there is a link from u to v
-
-        Returns a tuple.
-        """
-        target = 0
-        if from_node.document == to_node.document:
-            if to_node.id in from_node.outlinks:
-                target = 1
-        distance = from_node.distance_to(to_node)
-        features = (distance,
-                    to_node.top - from_node.top,
-                    to_node.left - from_node.left,
-                    to_node.bottom - from_node.bottom,
-                    to_node.right - from_node.right,
-                    from_node.class_name,
-                    to_node.class_name,
-                    target)
-        dist, dt, dl, db, dr, cu, cv, tgt = features
-        if cu.startswith('letter'):
-            cu = 'letter'
-        if cu.startswith('numeral'):
-            cu = 'numeral'
-        if cv.startswith('letter'):
-            cv = 'letter'
-        if cv.startswith('numeral'):
-            cv = 'numeral'
-        feature_dict = {'dist': dist,
-                        'dt': dt,
-                        'dl': dl,
-                        'db': db,
-                        'dr': dr,
-                        'cls_from': cu,
-                        'cls_to': cv,
-                        'target': tgt}
-        return feature_dict
-
-
-##############################################################################
-# Edge classifier
-
-
-class PairwiseClassificationParser(object):
-    """This parser applies a simple classifier that takes the bounding
-    boxes of two Nodes and their classes and returns whether there
-    is an edge or not."""
-    MAXIMUM_DISTANCE_THRESHOLD = 200
-
-    def __init__(self, grammar: DependencyGrammar, classifier,
-                 feature_extractor: PairwiseClassificationFeatureExtractor):
-        self.grammar = grammar
-        self.classifier = classifier
-        self.extractor = feature_extractor
-
-    def parse(self, nodes: List[Node]):
-
-        # Ensure the same docname for all Nodes,
-        # since we later compute their distances.
-        # The correct docname gets set on export anyway.
-        pairs, features = self.extract_all_pairs(nodes)
-
-        logging.info(
-            'Clf.Parse: {0} object pairs from {1} objects'.format(len(pairs), len(nodes)))
-
-        preds = self.classifier.predict(features)
-
-        edges = []
-        for idx, (c_from, c_to) in enumerate(pairs):
-            if preds[idx] != 0:
-                edges.append((c_from.id, c_to.id))
-
-        edges = self.__apply_trivial_fixes(nodes, edges)
-        return edges
-
-    def __apply_trivial_fixes(self, nodes: List[Node], edges: List[Tuple[int, int]]):
-        edges = self.__only_one_stem_per_notehead(nodes, edges)
-        edges = self.__every_full_notehead_has_a_stem(nodes, edges)
-
-        return edges
-
-    def __only_one_stem_per_notehead(self, nodes: List[Node], edges: List[Tuple[int, int]]):
-        node_id_to_node_mapping = {n.id: n for n in nodes}  # type: Dict[int, Node]
-
-        # Collect stems per notehead
-        stems_per_notehead = collections.defaultdict(list)
-        stem_objids = set()
-        for from_id, to_id in edges:
-            from_node = node_id_to_node_mapping[from_id]
-            to_node = node_id_to_node_mapping[to_id]
-            if (from_node.class_name in _CONST.NOTEHEAD_CLASS_NAMES) and \
-                    (to_node.class_name == 'stem'):
-                stems_per_notehead[from_id].append(to_id)
-                stem_objids.add(to_id)
-
-        # Pick the closest one (by minimum distance)
-        closest_stems_per_notehead = dict()
-        for n_objid in stems_per_notehead:
-            n = node_id_to_node_mapping[n_objid]
-            stems = [node_id_to_node_mapping[objid] for objid in stems_per_notehead[n_objid]]
-            closest_stem = min(stems, key=lambda s: n.distance_to(s))
-            closest_stems_per_notehead[n_objid] = closest_stem.id
-
-        # Filter the edges
-        edges = [(f_objid, t_objid) for f_objid, t_objid in edges
-                 if (f_objid not in closest_stems_per_notehead) or
-                 (t_objid not in stem_objids) or
-                 (closest_stems_per_notehead[f_objid] == t_objid)]
-
-        return edges
-
-    def __every_full_notehead_has_a_stem(self, nodes: List[Node], edges):
-        node_id_to_node_mapping = {c.id: c for c in nodes}  # type: Dict[int, Node]
-
-        # Collect stems per notehead
-        notehead_objids = set([c.id for c in nodes if c.class_name == 'noteheadFull'])
-        stem_objids = set([c.id for c in nodes if c.class_name == 'stem'])
-
-        noteheads_with_stem_objids = set()
-        stems_with_notehead_objids = set()
-        for f, t in edges:
-            if node_id_to_node_mapping[f].class_name == 'noteheadFull':
-                if node_id_to_node_mapping[t].class_name == 'stem':
-                    noteheads_with_stem_objids.add(f)
-                    stems_with_notehead_objids.add(t)
-
-        noteheads_without_stems = {n: node_id_to_node_mapping[n] for n in notehead_objids
-                                   if n not in noteheads_with_stem_objids}
-        stems_without_noteheads = {n: node_id_to_node_mapping[n] for n in stem_objids
-                                   if n not in stems_with_notehead_objids}
-
-        # To each notehead, assign the closest stem that is not yet taken.
-        closest_stem_per_notehead = {objid: min(stems_without_noteheads,
-                                                key=lambda x: node_id_to_node_mapping[
-                                                    x].distance_to(n))
-                                     for objid, n in list(noteheads_without_stems.items())}
-
-        # Filter edges that are too long
-        _n_before_filter = len(closest_stem_per_notehead)
-        closest_stem_threshold_distance = 80
-        closest_stem_per_notehead = {n_objid: s_objid
-                                     for n_objid, s_objid in list(closest_stem_per_notehead.items())
-                                     if node_id_to_node_mapping[n_objid].distance_to(
-                node_id_to_node_mapping[s_objid]) < closest_stem_threshold_distance}
-
-        return edges + list(closest_stem_per_notehead.items())
-
-    def extract_all_pairs(self, nodes: List[Node]):
-        pairs = []
-        features = []
-        for u in nodes:
-            for v in nodes:
-                if u.id == v.id:
-                    continue
-                distance = u.distance_to(v)
-                if distance < self.MAXIMUM_DISTANCE_THRESHOLD:
-                    pairs.append((u, v))
-                    f = self.extractor(u, v)
-                    features.append(f)
-
-        # logging.info('Parsing features: {0}'.format(features[0]))
-        features = numpy.array(features)
-        # logging.info('Parsing features: {0}/{1}'.format(features.shape, features))
-        return pairs, features
-
-    def is_edge(self, c_from, c_to) -> bool:
-        features = self.extractor(c_from, c_to)
-        result = self.classifier.predict(features)
-        return result
-
-    def set_grammar(self, grammar: DependencyGrammar):
-        self.grammar = grammar
-
-
-def do_parse(nodes: List[Node], parser: PairwiseClassificationParser) -> List[Node]:
-    non_staff_nodes = [node for node in nodes if node.class_name not in _CONST.STAFF_CLASS_NAMES]
-    edges = parser.parse(non_staff_nodes)
-
-    # Add edges
-    id_to_node_mapping = {node.id: node for node in nodes}
-    for f, t in edges:
-        cf, ct = id_to_node_mapping[f], id_to_node_mapping[t]
-        if t not in cf.outlinks:
-            if f not in ct.inlinks:
-                cf.outlinks.append(t)
-                ct.inlinks.append(f)
-
-    return nodes
-
-
-##############################################################################
-# Staffline building
-
-def process_stafflines(nodes: List[Node],
-                       do_build_staffs: bool = True,
-                       do_build_staffspaces: bool = True,
-                       do_add_staff_relationships: bool = True) -> List[Node]:
-    """Merges staffline fragments into stafflines. Can group them into staffs,
-    add staffspaces, and add the various obligatory relationships of other
-    objects to the staff objects. Required before attempting to export MIDI."""
-    if len([c for c in nodes if c.class_name == 'staff']) > 0:
-        logging.warning('Some stafflines have already been processed. Reprocessing'
-                        ' is not certain to work.')
-
-    try:
-        new_nodes = merge_staffline_segments(nodes)
-    except ValueError as e:
-        logging.warning('Model: Staffline merge failed:\n\t\t'
-                        '{0}'.format(e.message))
-        raise
-
-    try:
-        if do_build_staffs:
-            staffs = build_staff_nodes(new_nodes)
-            new_nodes = new_nodes + staffs
-    except Exception as e:
-        logging.warning('Building staffline Nodes from merged segments failed:'
-                        ' {0}'.format(e.message))
-        raise
-
-    try:
-        if do_build_staffspaces:
-            staffspaces = build_staffspace_nodes(new_nodes)
-            new_nodes = new_nodes + staffspaces
-    except Exception as e:
-        logging.warning('Building staffspace Nodes from stafflines failed:'
-                        ' {0}'.format(e.message))
-        raise
-
-    try:
-        if do_add_staff_relationships:
-            new_nodes = add_staff_relationships(new_nodes)
-    except Exception as e:
-        logging.warning('Adding staff relationships failed:'
-                        ' {0}'.format(e.message))
-        raise
-
-    return new_nodes
-
-
-def find_wrong_edges(nodes: List[Node], grammar: DependencyGrammar) -> List[Tuple[int, int]]:
-    id_to_node_mapping = {node.id: node for node in nodes}
-    graph = NotationGraph(nodes)
-
-    incoherent_beam_pairs = find_beams_incoherent_with_stems(nodes)
-    # Switching off misdirected leger lines: there is something wrong with them
-    misdirected_leger_lines = find_misdirected_leger_line_edges(nodes)
-
-    wrong_edges = [(n.id, b.id)
-                   for n, b in incoherent_beam_pairs + misdirected_leger_lines]
-
-    disallowed_symbol_class_pairs = [(f, t) for f, t in graph.edges
-                                     if not grammar.validate_edge(id_to_node_mapping[f].class_name,
-                                                                  id_to_node_mapping[t].class_name)]
-    wrong_edges += disallowed_symbol_class_pairs
-    return wrong_edges
-
-
-def find_very_small_nodes(nodes: List[Node], bbox_threshold=40, mask_threshold=35) -> List[int]:
-    very_small_nodes = []
-
-    for c in nodes:
-        total_masked_area = c.mask.sum()
-        total_bbox_area = c.width * c.height
-        if total_bbox_area < bbox_threshold:
-            very_small_nodes.append(c)
-        elif total_masked_area < mask_threshold:
-            very_small_nodes.append(c)
-
-    return list(set([c.id for c in very_small_nodes]))
-
-
-def infer_precedence_edges(nodes: List[Node], factor_by_staff=True) -> List[Tuple[int, int]]:
-    """Returns a list of (from_objid, to_objid) parirs. They
-    then need to be added to the Nodes as precedence edges."""
-    id_to_node_mapping = {c.id: c for c in nodes}
-    relevant_class_names = set(list(_CONST.NONGRACE_NOTEHEAD_CLASS_NAMES)
-                               + list(_CONST.REST_CLASS_NAMES))
-    precedence_nodes = [c for c in nodes
-                        if c.class_name in relevant_class_names]
-    logging.info('_infer_precedence: {0} total prec. Nodes'
-                 ''.format(len(precedence_nodes)))
-
-    # Group the objects according to the staff they are related to
-    # and infer precedence on these subgroups.
-    if factor_by_staff:
-        staffs = [c for c in nodes
-                  if c.class_name == _CONST.STAFF_CLASS_NAME]
-        logging.info('_infer_precedence: got {0} staffs'.format(len(staffs)))
-        staff_objids = {c.id: i for i, c in enumerate(staffs)}
-        precedence_nodes_per_staff = [[] for _ in staffs]
-        # All Nodes relevant for precedence have a relationship
-        # to a staff.
-        for c in precedence_nodes:
-            for o in c.outlinks:
-                if o in staff_objids:
-                    precedence_nodes_per_staff[staff_objids[o]].append(c)
-
-        logging.info('Precedence groups: {0}'
-                     ''.format(precedence_nodes_per_staff))
-        prec_edges = []
-        for precedence_nodes_group in precedence_nodes_per_staff:
-            group_prec_edges = infer_precedence_edges(precedence_nodes_group,
-                                                      factor_by_staff=False)
-            prec_edges.extend(group_prec_edges)
-        return prec_edges
-
-    if len(precedence_nodes) <= 1:
-        logging.info('EdgeListView._infer_precedence: less than 2'
-                     ' timed Nodes selected, no precedence'
-                     ' edges to infer.')
-        return []
-
-    # Group into equivalence if noteheads share stems
-    _stems_to_noteheads_map = collections.defaultdict(list)
-    for c in precedence_nodes:
-        for o in c.outlinks:
-            if o not in id_to_node_mapping:
-                logging.warning('Dangling outlink: {} --> {}'.format(c.id, o))
-                continue
-            c_o = id_to_node_mapping[o]
-            if c_o.class_name == 'stem':
-                _stems_to_noteheads_map[c_o.id].append(c.id)
-
-    _prec_equiv_objids = []
-    _stemmed_noteheads_objids = []
-    for _stem_objid, _stem_notehead_objids in list(_stems_to_noteheads_map.items()):
-        _stemmed_noteheads_objids = _stemmed_noteheads_objids \
-                                    + _stem_notehead_objids
-        _prec_equiv_objids.append(_stem_notehead_objids)
-    for c in precedence_nodes:
-        if c.id not in _stemmed_noteheads_objids:
-            _prec_equiv_objids.append([c.id])
-
-    equiv_objs = [[id_to_node_mapping[objid] for objid in equiv_objids]
-                  for equiv_objids in _prec_equiv_objids]
-
-    # Order the equivalence classes left to right
-    sorted_equiv_objs = sorted(equiv_objs,
-                               key=lambda eo: min([o.left for o in eo]))
-
-    edges = []
-    for i in range(len(sorted_equiv_objs) - 1):
-        fr_objs = sorted_equiv_objs[i]
-        to_objs = sorted_equiv_objs[i + 1]
-        for f in fr_objs:
-            for t in to_objs:
-                edges.append((f.id, t.id))
-
-    return edges
-
-
-def add_precedence_edges(nodes: List[Node], edges: List[Tuple[int, int]]) -> List[Node]:
-    """Adds precedence edges to Nodes."""
-    # Ensure unique
-    edges = set(edges)
-    id_to_node_mapping = {c.id: c for c in nodes}
-
-    for f, t in edges:
-        cf, ct = id_to_node_mapping[f], id_to_node_mapping[t]
-
-        if cf.data is None:
-            cf.data = dict()
-        if 'precedence_outlinks' not in cf.data:
-            cf.data['precedence_outlinks'] = []
-        cf.data['precedence_outlinks'].append(t)
-
-        if ct.data is None:
-            ct.data = dict()
-        if 'precedence_inlinks' not in ct.data:
-            ct.data['precedence_inlinks'] = []
-        ct.data['precedence_inlinks'].append(f)
-
-    return nodes
-
-
-def build_midi(nodes: List[Node], selected_nodes: List[Node] = None,
-               retain_pitches: bool = True,
-               retain_durations: bool = True,
-               retain_onsets: bool = True,
-               tempo: int = 180):
-    """Attempts to export a MIDI file from the current graph. Assumes that
-    all the staff objects and their relations have been correctly established,
-    and that the correct precedence graph is available.
-
-    :param retain_pitches: If set, will record the pitch information
-        in pitched objects.
-
-    :param retain_durations: If set, will record the duration information
-        in objects to which it applies.
-
-    :returns: A single-track ``midiutil.MidiFile.MIDIFile`` object. It can be
-        written to a stream using its ``mf.writeFile()`` method."""
-    id_to_node_mapping = {c.id: c for c in nodes}
-
-    pitch_inference_engine = PitchInferenceEngine()
-    time_inference_engine = OnsetsInferenceEngine(nodes=nodes)
-
-    try:
-        logging.info('Running pitch inference.')
-        pitches, pitch_names = pitch_inference_engine.infer_pitches(nodes,
-                                                                    with_names=True)
-    except Exception as e:
-        logging.warning('Model: Pitch inference failed!')
-        logging.exception(traceback.format_exc(e))
-        raise
-
-    if retain_pitches:
-        for objid in pitches:
-            c = id_to_node_mapping[objid]
-            pitch_step, pitch_octave = pitch_names[objid]
-            c.data['midi_pitch_code'] = pitches[objid]
-            c.data['normalized_pitch_step'] = pitch_step
-            c.data['pitch_octave'] = pitch_octave
-
-    try:
-        logging.info('Running durations inference.')
-        durations = time_inference_engine.durations(nodes)
-    except Exception as e:
-        logging.warning('Model: Duration inference failed!')
-        logging.exception(traceback.format_exc(e))
-        raise
-
-    if retain_durations:
-        for objid in durations:
-            c = id_to_node_mapping[objid]
-            c.data['duration_beats'] = durations[objid]
-
-    try:
-        logging.info('Running onsets inference.')
-        onsets = time_inference_engine.onsets(nodes)
-    except Exception as e:
-        logging.warning('Model: Onset inference failed!')
-        logging.exception(traceback.format_exc(e))
-        raise
-
-    if retain_onsets:
-        for objid in onsets:
-            c = id_to_node_mapping[objid]
-            c.data['onset_beats'] = onsets[objid]
-
-    # Process ties
-    durations, onsets = time_inference_engine.process_ties(nodes, durations, onsets)
-
-    # Prepare selection subset
-    if selected_nodes is None:
-        selected_nodes = nodes
-    ids_of_selected_nodes = [c.id for c in selected_nodes]
-
-    # Build the MIDI data
-    midi_builder = MIDIBuilder()
-    mf = midi_builder.build_midi(
-        pitches=pitches, durations=durations, onsets=onsets,
-        selection=ids_of_selected_nodes, tempo=tempo)
-
-    return mf
-
-
-def build_argument_parser():
-    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-
-    parser.add_argument('-i', '--input_mung', action='store', required=True,
-                        help='Read the input MuNG to this'
-                             ' file.')
-    parser.add_argument('-o', '--output_mung', action='store', required=True,
-                        help='Write the resulting MuNG to this'
-                             ' file.')
-
-    parser.add_argument('--mlclasses', action='store', required=True,
-                        help='Read the NodeClass list from this XML.')
-    parser.add_argument('--grammar', action='store', required=True,
-                        help='Read the grammar file that specifies the allowed edge node'
-                             ' class pairs.')
-    parser.add_argument('--parser', action='store', required=True,
-                        help='Read the pickled feature extractor for parser classifier.')
-    parser.add_argument('--vectorizer', action='store', required=True,
-                        help='Read the pickled parser classifier.')
-
-    parser.add_argument('--add_key_signatures', action='store_true',
-                        help='Attempt to add key signatures. Algorithm is'
-                             ' very basic: for each staff, gather all accidentals'
-                             ' intersecting that staff. From the left, find the'
-                             ' first notehead on a staff that is not contained in'
-                             ' anything, and the last clef before'
-                             ' this notehead. (...) [TESTING]')
-    parser.add_argument('--filter_contained', action='store_true',
-                        help='Remove objects that are fully contained within another.'
-                             ' This should be applied *after* parsing non-staff'
-                             ' edges, but *before* inferring staffs.')
-
-    parser.add_argument('-v', '--verbose', action='store_true',
-                        help='Turn on INFO messages.')
-    parser.add_argument('--debug', action='store_true',
-                        help='Turn on DEBUG messages.')
-
-    return parser
-
-
-def main(args):
-    logging.info('Starting main...')
-    _start_time = time.clock()
-
-    ###############################################################
-    # Preparation: loading the parsing apparatus
-
-    with open(args.vectorizer) as hdl:
-        vectorizer = pickle.load(hdl)
-    feature_extractor = PairwiseClassificationFeatureExtractor(vectorizer=vectorizer)
-
-    with open(args.parser) as hdl:
-        classifier = pickle.load(hdl)
-
-    mlclass_list = parse_node_classes(args.mlclasses)
-    mlclasses = {m.name for m in mlclass_list}
-
-    grammar = DependencyGrammar(grammar_filename=args.grammar, alphabet=mlclasses)
-
-    parser = PairwiseClassificationParser(grammar=grammar,
-                                          classifier=classifier,
-                                          feature_extractor=feature_extractor)
-
-    #################################################################
-    logging.info('Load graph')
-    nodes = read_nodes_from_file(args.input_mung)
-
-    logging.info('Filter very small')
-    very_small_nodes = find_very_small_nodes(nodes,
-                                             bbox_threshold=40,
-                                             mask_threshold=35)
-    very_small_nodes = set(very_small_nodes)
-    nodes = [c for c in nodes if c not in very_small_nodes]
-
-    logging.info('Parsing')
-    nodes = do_parse(nodes, parser=parser)
-
-    # Filter contained here.
-    if args.filter_contained:
-        logging.info('Finding contained Nodes...')
-        contained = find_contained_nodes(nodes,
-                                         mask_threshold=0.95)
-        NEVER_DISCARD_CLASSES = ['key_signature', 'time_signature']
-        contained = [c for c in contained if c.class_name not in NEVER_DISCARD_CLASSES]
-
-        _contained_counts = collections.defaultdict(int)
-        for c in contained:
-            _contained_counts[c.class_name] += 1
-        logging.info('Found {} contained Nodes'.format(len(contained)))
-        logging.info('Contained counts:\n{0}'.format(pprint.pformat(dict(_contained_counts))))
-        nodes = remove_contained_nodes(nodes,
-                                       contained)
-        logging.info('Removed contained Nodes: {}...'.format([m.id for m in contained]))
-
-    logging.info('Inferring staffline & staff objects, staff relationships')
-    nodes = process_stafflines(nodes)
-
-    if args.add_key_signatures:
-        nodes = add_key_signatures(nodes)
-
-    logging.info('Filter invalid edges')
-    graph = NotationGraph(nodes)
-    # Operatng on the graph changes the Nodes
-    #  -- the graph only keeps a pointer
-    wrong_edges = find_wrong_edges(nodes, grammar)
-    for f, t in wrong_edges:
-        graph.remove_edge(f, t)
-
-    logging.info('Add precedence relationships, factored only by staff')
-    prec_edges = infer_precedence_edges(nodes)
-    nodes = add_precedence_edges(nodes, prec_edges)
-
-    logging.info('Ensuring MIDI can be built')
-    mf = build_midi(nodes,
-                    retain_pitches=True,
-                    retain_durations=True,
-                    retain_onsets=True,
-                    tempo=180)
-
-    logging.info('Save output')
-    docname = os.path.splitext(os.path.basename(args.output_mung))[0]
-    xml = export_node_list(nodes,
-                           document=docname,
-                           dataset='FNOMR_results')
-    with open(args.output_mung, 'w') as out_stream:
-        out_stream.write(xml)
-        out_stream.write('\n')
-
-    _end_time = time.clock()
-    logging.info('baseline_process_symbols.py done in {0:.3f} s'.format(_end_time - _start_time))
-
-
-if __name__ == '__main__':
-    parser = build_argument_parser()
-    args = parser.parse_args()
-
-    if args.verbose:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
-    if args.debug:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
-
-    main(args)
+"""This is a script that processes a set of symbols in order to obtain the pitch
+recognition baseline. Intended to be used on top of an object detection stage."""
+import argparse
+import collections
+import logging
+import os
+import pickle
+import pprint
+import time
+import traceback
+from typing import List, Dict, Tuple
+
+import numpy
+from mung.constants import InferenceEngineConstants as _CONST
+from mung.grammar import DependencyGrammar
+from mung.graph import find_beams_incoherent_with_stems, NotationGraph
+from mung.graph import find_contained_nodes, remove_contained_nodes
+from mung.graph import find_misdirected_leger_line_edges
+from mung.io import parse_node_classes, read_nodes_from_file, export_node_list
+from mung.node import bounding_box_intersection, merge_multiple_nodes, link_nodes, Node
+from mung.stafflines import merge_staffline_segments, build_staff_nodes, \
+    build_staffspace_nodes, \
+    add_staff_relationships
+from mung2midi.inference import OnsetsInferenceEngine, PitchInferenceEngine
+from sklearn.feature_extraction import DictVectorizer
+
+
+def add_key_signatures(nodes: List[Node]) -> List[Node]:
+    """Heuristic for deciding which accidentals are inline,
+    and which should be interpreted as components of a key signature.
+
+    Assumes staffline relationships have already been inferred.
+
+    The heuristic is defined for each staff S as the following:
+
+    * Take the leftmost clef C.
+    * Take the leftmost notehead (incl. grace notes) N.
+    * Take all accidentals A_S that overlap the space between C and N
+      horizontally (including C, not including N), and overlap the staff.
+    * Order A_S left-to-right
+    * Set m = C
+    * Initialize key signature K_S = {}
+    * For each a_S in A_S:
+    * if it is closer to m than to N, then:
+    *   add a_S to K_S,
+    *   set m = a_S
+    * else:
+    *   break
+
+    Note that this modifies the accidentals and staffs in-place: they get inlinks
+    from their respective key signatures.
+    """
+    graph = NotationGraph(nodes)
+
+    new_node_id = max([m.id for m in nodes]) + 1
+
+    key_signatures = []
+
+    staffs = [m for m in nodes if m.class_name == _CONST.STAFF]
+    for s in staffs:
+
+        # Take the leftmost clef C.
+        clefs = graph.parents(s.id, class_filter=_CONST.CLEF_CLASS_NAMES)
+        if len(clefs) == 0:
+            continue
+        leftmost_clef = min(clefs, key=lambda x: x.left)
+
+        # Take the leftmost notehead (incl. grace notes) N.
+        noteheads = graph.parents(s.id, class_filter=_CONST.NOTEHEAD_CLASS_NAMES)
+        if len(noteheads) == 0:
+            continue
+        leftmost_notehead = min(noteheads, key=lambda x: x.left)
+
+        # Take all accidentals A_S that fall between C and N
+        # horizontally, and overlap the staff.
+        all_accidentals = [m for m in nodes
+                           if m.class_name in _CONST.ACCIDENTAL_CLASS_NAMES]
+        relevant_acc_bbox = s.top, leftmost_clef.left, s.bottom, leftmost_notehead.left
+        relevant_accidentals = [m for m in all_accidentals
+                                if bounding_box_intersection(m.bounding_box,
+                                                             relevant_acc_bbox)
+                                is not None]
+
+        # Order A_S left-to-right.
+        ordered_accidentals = sorted(relevant_accidentals,
+                                     key=lambda x: x.left)
+
+        # Set m = C
+        current_lstop = leftmost_clef.right
+        key_signature_accidentals = []
+
+        # Iterate over accidentals; check if they are closer to lstop
+        # than to the first notehead
+        for a in ordered_accidentals:
+            if (a.left - current_lstop) < (leftmost_notehead.left - a.right):
+                key_signature_accidentals.append(a)
+                current_lstop = a.right
+            else:
+                break
+
+        # Build key signature and connect it to staff
+        if len(key_signature_accidentals) > 0:
+            key_signature_class_names = list(_CONST.KEY_SIGNATURE)[0]
+            # Note: there might be spurious links from the accidentals
+            # to notheads, if they were mis-interpreted during parsing.
+            # This actually might not matter; needs testing.
+            key_signature = merge_multiple_nodes(
+                key_signature_accidentals,
+                class_name=key_signature_class_names,
+                id_=new_node_id)
+            new_node_id += 1
+            link_nodes(key_signature, s)
+            for a in key_signature_accidentals:
+                link_nodes(key_signature, a)
+
+            key_signatures.append(key_signature)
+
+    logging.info('Adding {} key signatures'.format(len(key_signatures)))
+    return nodes + key_signatures
+
+
+##############################################################################
+# Feature extraction
+
+class PairwiseClassificationFeatureExtractor(object):
+    def __init__(self, vectorizer=None):
+        """Initialize the feature extractor.
+
+        :param vectorizer: A DictVectorizer() from scikit-learn.
+            Used to convert feature dicts to the vectors that
+            the edge classifier of the parser will expect.
+            If None, will create a new DictVectorizer. (This is useful
+            for training; you can then pickle the entire extractor
+            and make sure the feature extraction works for the classifier
+            at runtime.)
+        """
+        if vectorizer is None:
+            vectorizer = DictVectorizer()
+        self.vectorizer = vectorizer
+
+    def __call__(self, *args, **kwargs):
+        """The call is per item (in this case, Node pair)."""
+        fd = self.get_features_relative_bbox_and_clsname(*args, **kwargs)
+        # Compensate for the vecotrizer "target", which we don't have here (by :-1)
+        item_features = self.vectorizer.transform(fd).toarray()[0, :-1]
+        return item_features
+
+    def get_features_relative_bbox_and_clsname(self, c_from: Node, c_to: Node):
+        """Extract a feature vector from the given pair of Nodes.
+        Does *NOT* convert the class names to integers.
+
+        Features: bbox(c_to) - bbox(c_from), class_name(c_from), class_name(c_to)
+        Target: 1 if there is a link from u to v
+
+        Returns a dict that works as input to ``self.vectorizer``.
+        """
+        target = 0
+        if c_from.document == c_to.document:
+            if c_to.id in c_from.outlinks:
+                target = 1
+        features = (c_to.top - c_from.top,
+                    c_to.left - c_from.left,
+                    c_to.bottom - c_from.bottom,
+                    c_to.right - c_from.right,
+                    c_from.class_name,
+                    c_to.class_name,
+                    target)
+        dt, dl, db, dr, cu, cv, tgt = features
+        # Normalizing clsnames
+        if cu.startswith('letter'):
+            cu = 'letter'
+        if cu.startswith('numeral'):
+            cu = 'numeral'
+        if cv.startswith('letter'):
+            cv = 'letter'
+        if cv.startswith('numeral'):
+            cv = 'numeral'
+        feature_dict = {'dt': dt,
+                        'dl': dl,
+                        'db': db,
+                        'dr': dr,
+                        'cls_from': cu,
+                        'cls_to': cv,
+                        'target': tgt}
+        return feature_dict
+
+    def get_features_distance_relative_bbox_and_clsname(self, from_node: Node,
+                                                        to_node: Node) -> Dict:
+        """Extract a feature vector from the given pair of Nodes.
+        Does *NOT* convert the class names to integers.
+
+        Features: bbox(c_to) - bbox(c_from), class_name(c_from), class_name(c_to)
+        Target: 1 if there is a link from u to v
+
+        Returns a tuple.
+        """
+        target = 0
+        if from_node.document == to_node.document:
+            if to_node.id in from_node.outlinks:
+                target = 1
+        distance = from_node.distance_to(to_node)
+        features = (distance,
+                    to_node.top - from_node.top,
+                    to_node.left - from_node.left,
+                    to_node.bottom - from_node.bottom,
+                    to_node.right - from_node.right,
+                    from_node.class_name,
+                    to_node.class_name,
+                    target)
+        dist, dt, dl, db, dr, cu, cv, tgt = features
+        if cu.startswith('letter'):
+            cu = 'letter'
+        if cu.startswith('numeral'):
+            cu = 'numeral'
+        if cv.startswith('letter'):
+            cv = 'letter'
+        if cv.startswith('numeral'):
+            cv = 'numeral'
+        feature_dict = {'dist': dist,
+                        'dt': dt,
+                        'dl': dl,
+                        'db': db,
+                        'dr': dr,
+                        'cls_from': cu,
+                        'cls_to': cv,
+                        'target': tgt}
+        return feature_dict
+
+
+##############################################################################
+# Edge classifier
+
+
+class PairwiseClassificationParser(object):
+    """This parser applies a simple classifier that takes the bounding
+    boxes of two Nodes and their classes and returns whether there
+    is an edge or not."""
+    MAXIMUM_DISTANCE_THRESHOLD = 200
+
+    def __init__(self, grammar: DependencyGrammar, classifier,
+                 feature_extractor: PairwiseClassificationFeatureExtractor):
+        self.grammar = grammar
+        self.classifier = classifier
+        self.extractor = feature_extractor
+
+    def parse(self, nodes: List[Node]):
+
+        # Ensure the same docname for all Nodes,
+        # since we later compute their distances.
+        # The correct docname gets set on export anyway.
+        pairs, features = self.extract_all_pairs(nodes)
+
+        logging.info(
+            'Clf.Parse: {0} object pairs from {1} objects'.format(len(pairs), len(nodes)))
+
+        preds = self.classifier.predict(features)
+
+        edges = []
+        for idx, (c_from, c_to) in enumerate(pairs):
+            if preds[idx] != 0:
+                edges.append((c_from.id, c_to.id))
+
+        edges = self.__apply_trivial_fixes(nodes, edges)
+        return edges
+
+    def __apply_trivial_fixes(self, nodes: List[Node], edges: List[Tuple[int, int]]):
+        edges = self.__only_one_stem_per_notehead(nodes, edges)
+        edges = self.__every_full_notehead_has_a_stem(nodes, edges)
+
+        return edges
+
+    def __only_one_stem_per_notehead(self, nodes: List[Node], edges: List[Tuple[int, int]]):
+        node_id_to_node_mapping = {n.id: n for n in nodes}  # type: Dict[int, Node]
+
+        # Collect stems per notehead
+        stems_per_notehead = collections.defaultdict(list)
+        stem_objids = set()
+        for from_id, to_id in edges:
+            from_node = node_id_to_node_mapping[from_id]
+            to_node = node_id_to_node_mapping[to_id]
+            if (from_node.class_name in _CONST.NOTEHEAD_CLASS_NAMES) and \
+                    (to_node.class_name == 'stem'):
+                stems_per_notehead[from_id].append(to_id)
+                stem_objids.add(to_id)
+
+        # Pick the closest one (by minimum distance)
+        closest_stems_per_notehead = dict()
+        for n_objid in stems_per_notehead:
+            n = node_id_to_node_mapping[n_objid]
+            stems = [node_id_to_node_mapping[objid] for objid in stems_per_notehead[n_objid]]
+            closest_stem = min(stems, key=lambda s: n.distance_to(s))
+            closest_stems_per_notehead[n_objid] = closest_stem.id
+
+        # Filter the edges
+        edges = [(f_objid, t_objid) for f_objid, t_objid in edges
+                 if (f_objid not in closest_stems_per_notehead) or
+                 (t_objid not in stem_objids) or
+                 (closest_stems_per_notehead[f_objid] == t_objid)]
+
+        return edges
+
+    def __every_full_notehead_has_a_stem(self, nodes: List[Node], edges):
+        node_id_to_node_mapping = {c.id: c for c in nodes}  # type: Dict[int, Node]
+
+        # Collect stems per notehead
+        notehead_objids = set([c.id for c in nodes if c.class_name == 'noteheadFull'])
+        stem_objids = set([c.id for c in nodes if c.class_name == 'stem'])
+
+        noteheads_with_stem_objids = set()
+        stems_with_notehead_objids = set()
+        for f, t in edges:
+            if node_id_to_node_mapping[f].class_name == 'noteheadFull':
+                if node_id_to_node_mapping[t].class_name == 'stem':
+                    noteheads_with_stem_objids.add(f)
+                    stems_with_notehead_objids.add(t)
+
+        noteheads_without_stems = {n: node_id_to_node_mapping[n] for n in notehead_objids
+                                   if n not in noteheads_with_stem_objids}
+        stems_without_noteheads = {n: node_id_to_node_mapping[n] for n in stem_objids
+                                   if n not in stems_with_notehead_objids}
+
+        # To each notehead, assign the closest stem that is not yet taken.
+        closest_stem_per_notehead = {objid: min(stems_without_noteheads,
+                                                key=lambda x: node_id_to_node_mapping[
+                                                    x].distance_to(n))
+                                     for objid, n in list(noteheads_without_stems.items())}
+
+        # Filter edges that are too long
+        _n_before_filter = len(closest_stem_per_notehead)
+        closest_stem_threshold_distance = 80
+        closest_stem_per_notehead = {n_objid: s_objid
+                                     for n_objid, s_objid in list(closest_stem_per_notehead.items())
+                                     if node_id_to_node_mapping[n_objid].distance_to(
+                node_id_to_node_mapping[s_objid]) < closest_stem_threshold_distance}
+
+        return edges + list(closest_stem_per_notehead.items())
+
+    def extract_all_pairs(self, nodes: List[Node]):
+        pairs = []
+        features = []
+        for u in nodes:
+            for v in nodes:
+                if u.id == v.id:
+                    continue
+                distance = u.distance_to(v)
+                if distance < self.MAXIMUM_DISTANCE_THRESHOLD:
+                    pairs.append((u, v))
+                    f = self.extractor(u, v)
+                    features.append(f)
+
+        # logging.info('Parsing features: {0}'.format(features[0]))
+        features = numpy.array(features)
+        # logging.info('Parsing features: {0}/{1}'.format(features.shape, features))
+        return pairs, features
+
+    def is_edge(self, c_from, c_to) -> bool:
+        features = self.extractor(c_from, c_to)
+        result = self.classifier.predict(features)
+        return result
+
+    def set_grammar(self, grammar: DependencyGrammar):
+        self.grammar = grammar
+
+
+def do_parse(nodes: List[Node], parser: PairwiseClassificationParser) -> List[Node]:
+    non_staff_nodes = [node for node in nodes if node.class_name not in _CONST.STAFF_CLASSES]
+    edges = parser.parse(non_staff_nodes)
+
+    # Add edges
+    id_to_node_mapping = {node.id: node for node in nodes}
+    for f, t in edges:
+        cf, ct = id_to_node_mapping[f], id_to_node_mapping[t]
+        if t not in cf.outlinks:
+            if f not in ct.inlinks:
+                cf.outlinks.append(t)
+                ct.inlinks.append(f)
+
+    return nodes
+
+
+##############################################################################
+# Staffline building
+
+def process_stafflines(nodes: List[Node],
+                       do_build_staffs: bool = True,
+                       do_build_staffspaces: bool = True,
+                       do_add_staff_relationships: bool = True) -> List[Node]:
+    """Merges staffline fragments into stafflines. Can group them into staffs,
+    add staffspaces, and add the various obligatory relationships of other
+    objects to the staff objects. Required before attempting to export MIDI."""
+    if len([c for c in nodes if c.class_name == 'staff']) > 0:
+        logging.warning('Some stafflines have already been processed. Reprocessing'
+                        ' is not certain to work.')
+
+    try:
+        new_nodes = merge_staffline_segments(nodes)
+    except ValueError as e:
+        logging.warning('Model: Staffline merge failed:\n\t\t'
+                        '{0}'.format(e.message))
+        raise
+
+    try:
+        if do_build_staffs:
+            staffs = build_staff_nodes(new_nodes)
+            new_nodes = new_nodes + staffs
+    except Exception as e:
+        logging.warning('Building staffline Nodes from merged segments failed:'
+                        ' {0}'.format(e.message))
+        raise
+
+    try:
+        if do_build_staffspaces:
+            staffspaces = build_staffspace_nodes(new_nodes)
+            new_nodes = new_nodes + staffspaces
+    except Exception as e:
+        logging.warning('Building staffspace Nodes from stafflines failed:'
+                        ' {0}'.format(e.message))
+        raise
+
+    try:
+        if do_add_staff_relationships:
+            new_nodes = add_staff_relationships(new_nodes)
+    except Exception as e:
+        logging.warning('Adding staff relationships failed:'
+                        ' {0}'.format(e.message))
+        raise
+
+    return new_nodes
+
+
+def find_wrong_edges(nodes: List[Node], grammar: DependencyGrammar) -> List[Tuple[int, int]]:
+    id_to_node_mapping = {node.id: node for node in nodes}
+    graph = NotationGraph(nodes)
+
+    incoherent_beam_pairs = find_beams_incoherent_with_stems(nodes)
+    # Switching off misdirected leger lines: there is something wrong with them
+    misdirected_leger_lines = find_misdirected_leger_line_edges(nodes)
+
+    wrong_edges = [(n.id, b.id)
+                   for n, b in incoherent_beam_pairs + misdirected_leger_lines]
+
+    disallowed_symbol_class_pairs = [(f, t) for f, t in graph.edges
+                                     if not grammar.validate_edge(id_to_node_mapping[f].class_name,
+                                                                  id_to_node_mapping[t].class_name)]
+    wrong_edges += disallowed_symbol_class_pairs
+    return wrong_edges
+
+
+def find_very_small_nodes(nodes: List[Node], bbox_threshold=40, mask_threshold=35) -> List[int]:
+    very_small_nodes = []
+
+    for c in nodes:
+        total_masked_area = c.mask.sum()
+        total_bbox_area = c.width * c.height
+        if total_bbox_area < bbox_threshold:
+            very_small_nodes.append(c)
+        elif total_masked_area < mask_threshold:
+            very_small_nodes.append(c)
+
+    return list(set([c.id for c in very_small_nodes]))
+
+
+def infer_precedence_edges(nodes: List[Node], factor_by_staff=True) -> List[Tuple[int, int]]:
+    """Returns a list of (from_objid, to_objid) parirs. They
+    then need to be added to the Nodes as precedence edges."""
+    id_to_node_mapping = {c.id: c for c in nodes}
+    relevant_class_names = set(list(_CONST.NONGRACE_NOTEHEAD_CLASS_NAMES)
+                               + list(_CONST.REST_CLASS_NAMES))
+    precedence_nodes = [c for c in nodes
+                        if c.class_name in relevant_class_names]
+    logging.info('_infer_precedence: {0} total prec. Nodes'
+                 ''.format(len(precedence_nodes)))
+
+    # Group the objects according to the staff they are related to
+    # and infer precedence on these subgroups.
+    if factor_by_staff:
+        staffs = [c for c in nodes
+                  if c.class_name == _CONST.STAFF]
+        logging.info('_infer_precedence: got {0} staffs'.format(len(staffs)))
+        staff_objids = {c.id: i for i, c in enumerate(staffs)}
+        precedence_nodes_per_staff = [[] for _ in staffs]
+        # All Nodes relevant for precedence have a relationship
+        # to a staff.
+        for c in precedence_nodes:
+            for o in c.outlinks:
+                if o in staff_objids:
+                    precedence_nodes_per_staff[staff_objids[o]].append(c)
+
+        logging.info('Precedence groups: {0}'
+                     ''.format(precedence_nodes_per_staff))
+        prec_edges = []
+        for precedence_nodes_group in precedence_nodes_per_staff:
+            group_prec_edges = infer_precedence_edges(precedence_nodes_group,
+                                                      factor_by_staff=False)
+            prec_edges.extend(group_prec_edges)
+        return prec_edges
+
+    if len(precedence_nodes) <= 1:
+        logging.info('EdgeListView._infer_precedence: less than 2'
+                     ' timed Nodes selected, no precedence'
+                     ' edges to infer.')
+        return []
+
+    # Group into equivalence if noteheads share stems
+    _stems_to_noteheads_map = collections.defaultdict(list)
+    for c in precedence_nodes:
+        for o in c.outlinks:
+            if o not in id_to_node_mapping:
+                logging.warning('Dangling outlink: {} --> {}'.format(c.id, o))
+                continue
+            c_o = id_to_node_mapping[o]
+            if c_o.class_name == 'stem':
+                _stems_to_noteheads_map[c_o.id].append(c.id)
+
+    _prec_equiv_objids = []
+    _stemmed_noteheads_objids = []
+    for _stem_objid, _stem_notehead_objids in list(_stems_to_noteheads_map.items()):
+        _stemmed_noteheads_objids = _stemmed_noteheads_objids \
+                                    + _stem_notehead_objids
+        _prec_equiv_objids.append(_stem_notehead_objids)
+    for c in precedence_nodes:
+        if c.id not in _stemmed_noteheads_objids:
+            _prec_equiv_objids.append([c.id])
+
+    equiv_objs = [[id_to_node_mapping[objid] for objid in equiv_objids]
+                  for equiv_objids in _prec_equiv_objids]
+
+    # Order the equivalence classes left to right
+    sorted_equiv_objs = sorted(equiv_objs,
+                               key=lambda eo: min([o.left for o in eo]))
+
+    edges = []
+    for i in range(len(sorted_equiv_objs) - 1):
+        fr_objs = sorted_equiv_objs[i]
+        to_objs = sorted_equiv_objs[i + 1]
+        for f in fr_objs:
+            for t in to_objs:
+                edges.append((f.id, t.id))
+
+    return edges
+
+
+def add_precedence_edges(nodes: List[Node], edges: List[Tuple[int, int]]) -> List[Node]:
+    """Adds precedence edges to Nodes."""
+    # Ensure unique
+    edges = set(edges)
+    id_to_node_mapping = {c.id: c for c in nodes}
+
+    for f, t in edges:
+        cf, ct = id_to_node_mapping[f], id_to_node_mapping[t]
+
+        if cf.data is None:
+            cf.data = dict()
+        if 'precedence_outlinks' not in cf.data:
+            cf.data['precedence_outlinks'] = []
+        cf.data['precedence_outlinks'].append(t)
+
+        if ct.data is None:
+            ct.data = dict()
+        if 'precedence_inlinks' not in ct.data:
+            ct.data['precedence_inlinks'] = []
+        ct.data['precedence_inlinks'].append(f)
+
+    return nodes
+
+
+def build_midi(nodes: List[Node], selected_nodes: List[Node] = None,
+               retain_pitches: bool = True,
+               retain_durations: bool = True,
+               retain_onsets: bool = True,
+               tempo: int = 180):
+    """Attempts to export a MIDI file from the current graph. Assumes that
+    all the staff objects and their relations have been correctly established,
+    and that the correct precedence graph is available.
+
+    :param retain_pitches: If set, will record the pitch information
+        in pitched objects.
+
+    :param retain_durations: If set, will record the duration information
+        in objects to which it applies.
+
+    :returns: A single-track ``midiutil.MidiFile.MIDIFile`` object. It can be
+        written to a stream using its ``mf.writeFile()`` method."""
+    id_to_node_mapping = {c.id: c for c in nodes}
+
+    pitch_inference_engine = PitchInferenceEngine()
+    time_inference_engine = OnsetsInferenceEngine(nodes=nodes)
+
+    try:
+        logging.info('Running pitch inference.')
+        pitches, pitch_names = pitch_inference_engine.infer_pitches(nodes,
+                                                                    with_names=True)
+    except Exception as e:
+        logging.warning('Model: Pitch inference failed!')
+        logging.exception(traceback.format_exc(e))
+        raise
+
+    if retain_pitches:
+        for objid in pitches:
+            c = id_to_node_mapping[objid]
+            pitch_step, pitch_octave = pitch_names[objid]
+            c.data['midi_pitch_code'] = pitches[objid]
+            c.data['normalized_pitch_step'] = pitch_step
+            c.data['pitch_octave'] = pitch_octave
+
+    try:
+        logging.info('Running durations inference.')
+        durations = time_inference_engine.durations(nodes)
+    except Exception as e:
+        logging.warning('Model: Duration inference failed!')
+        logging.exception(traceback.format_exc(e))
+        raise
+
+    if retain_durations:
+        for objid in durations:
+            c = id_to_node_mapping[objid]
+            c.data['duration_beats'] = durations[objid]
+
+    try:
+        logging.info('Running onsets inference.')
+        onsets = time_inference_engine.onsets(nodes)
+    except Exception as e:
+        logging.warning('Model: Onset inference failed!')
+        logging.exception(traceback.format_exc(e))
+        raise
+
+    if retain_onsets:
+        for objid in onsets:
+            c = id_to_node_mapping[objid]
+            c.data['onset_beats'] = onsets[objid]
+
+    # Process ties
+    durations, onsets = time_inference_engine.process_ties(nodes, durations, onsets)
+
+    # Prepare selection subset
+    if selected_nodes is None:
+        selected_nodes = nodes
+    ids_of_selected_nodes = [c.id for c in selected_nodes]
+
+    # Build the MIDI data
+    mf = build_midi(pitches=pitches, durations=durations, onsets=onsets, selection=ids_of_selected_nodes, tempo=tempo)
+
+    return mf
+
+
+def build_argument_parser():
+    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+
+    parser.add_argument('-i', '--input_mung', action='store', required=True,
+                        help='Read the input MuNG to this'
+                             ' file.')
+    parser.add_argument('-o', '--output_mung', action='store', required=True,
+                        help='Write the resulting MuNG to this'
+                             ' file.')
+
+    parser.add_argument('--mlclasses', action='store', required=True,
+                        help='Read the NodeClass list from this XML.')
+    parser.add_argument('--grammar', action='store', required=True,
+                        help='Read the grammar file that specifies the allowed edge node'
+                             ' class pairs.')
+    parser.add_argument('--parser', action='store', required=True,
+                        help='Read the pickled feature extractor for parser classifier.')
+    parser.add_argument('--vectorizer', action='store', required=True,
+                        help='Read the pickled parser classifier.')
+
+    parser.add_argument('--add_key_signatures', action='store_true',
+                        help='Attempt to add key signatures. Algorithm is'
+                             ' very basic: for each staff, gather all accidentals'
+                             ' intersecting that staff. From the left, find the'
+                             ' first notehead on a staff that is not contained in'
+                             ' anything, and the last clef before'
+                             ' this notehead. (...) [TESTING]')
+    parser.add_argument('--filter_contained', action='store_true',
+                        help='Remove objects that are fully contained within another.'
+                             ' This should be applied *after* parsing non-staff'
+                             ' edges, but *before* inferring staffs.')
+
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='Turn on INFO messages.')
+    parser.add_argument('--debug', action='store_true',
+                        help='Turn on DEBUG messages.')
+
+    return parser
+
+
+def main(args):
+    logging.info('Starting main...')
+    _start_time = time.clock()
+
+    ###############################################################
+    # Preparation: loading the parsing apparatus
+
+    with open(args.vectorizer) as hdl:
+        vectorizer = pickle.load(hdl)
+    feature_extractor = PairwiseClassificationFeatureExtractor(vectorizer=vectorizer)
+
+    with open(args.parser) as hdl:
+        classifier = pickle.load(hdl)
+
+    mlclass_list = parse_node_classes(args.mlclasses)
+    mlclasses = {m.name for m in mlclass_list}
+
+    grammar = DependencyGrammar(grammar_filename=args.grammar, alphabet=mlclasses)
+
+    parser = PairwiseClassificationParser(grammar=grammar,
+                                          classifier=classifier,
+                                          feature_extractor=feature_extractor)
+
+    #################################################################
+    logging.info('Load graph')
+    nodes = read_nodes_from_file(args.input_mung)
+
+    logging.info('Filter very small')
+    very_small_nodes = find_very_small_nodes(nodes,
+                                             bbox_threshold=40,
+                                             mask_threshold=35)
+    very_small_nodes = set(very_small_nodes)
+    nodes = [c for c in nodes if c not in very_small_nodes]
+
+    logging.info('Parsing')
+    nodes = do_parse(nodes, parser=parser)
+
+    # Filter contained here.
+    if args.filter_contained:
+        logging.info('Finding contained Nodes...')
+        contained = find_contained_nodes(nodes,
+                                         mask_threshold=0.95)
+        NEVER_DISCARD_CLASSES = ['key_signature', 'time_signature']
+        contained = [c for c in contained if c.class_name not in NEVER_DISCARD_CLASSES]
+
+        _contained_counts = collections.defaultdict(int)
+        for c in contained:
+            _contained_counts[c.class_name] += 1
+        logging.info('Found {} contained Nodes'.format(len(contained)))
+        logging.info('Contained counts:\n{0}'.format(pprint.pformat(dict(_contained_counts))))
+        nodes = remove_contained_nodes(nodes,
+                                       contained)
+        logging.info('Removed contained Nodes: {}...'.format([m.id for m in contained]))
+
+    logging.info('Inferring staffline & staff objects, staff relationships')
+    nodes = process_stafflines(nodes)
+
+    if args.add_key_signatures:
+        nodes = add_key_signatures(nodes)
+
+    logging.info('Filter invalid edges')
+    graph = NotationGraph(nodes)
+    # Operatng on the graph changes the Nodes
+    #  -- the graph only keeps a pointer
+    wrong_edges = find_wrong_edges(nodes, grammar)
+    for f, t in wrong_edges:
+        graph.remove_edge(f, t)
+
+    logging.info('Add precedence relationships, factored only by staff')
+    prec_edges = infer_precedence_edges(nodes)
+    nodes = add_precedence_edges(nodes, prec_edges)
+
+    logging.info('Ensuring MIDI can be built')
+    mf = build_midi(nodes,
+                    retain_pitches=True,
+                    retain_durations=True,
+                    retain_onsets=True,
+                    tempo=180)
+
+    logging.info('Save output')
+    docname = os.path.splitext(os.path.basename(args.output_mung))[0]
+    xml = export_node_list(nodes,
+                           document=docname,
+                           dataset='FNOMR_results')
+    with open(args.output_mung, 'w') as out_stream:
+        out_stream.write(xml)
+        out_stream.write('\n')
+
+    _end_time = time.clock()
+    logging.info('baseline_process_symbols.py done in {0:.3f} s'.format(_end_time - _start_time))
+
+
+if __name__ == '__main__':
+    parser = build_argument_parser()
+    args = parser.parse_args()
+
+    if args.verbose:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
+    if args.debug:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
+
+    main(args)
```

### Comparing `mung-1.1/scripts/infer_pitches.py` & `mung-1.2/scripts/infer_pitches.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-#!/usr/bin/env python
-"""This is a script that takes the full-grown notation graph
-and recovers for each notehead the pitch to which it corresponds.
-
-Assumptions
------------
-
-* Clefs are used in a standard way: G-clef on 4th, C-clef on 3rd, F-clef
-  on 2nd staffline.
-* Key signatures are used in a standard way, so that we can rely on counting
-  the accidentals.
-* Accidentals are valid up until the end of the bar.
-
-We are currently NOT processing any transpositions.
-
-Representation
---------------
-
-Notes are not noteheads. Pitch is associated with a note, and it is derived
-from the notehead's subgraph. The current goal of this exercise is obtaining
-MIDI, so we discard in effect information about what is e.g. a G-sharp
-and A-flat.
-
-"""
-import argparse
-import logging
-import os
-import time
-
-from mung2midi.inference import PitchInferenceEngine, OnsetsInferenceEngine, MIDIBuilder
-from mung.io import read_nodes_from_file, export_node_list
-
-
-def build_argument_parser():
-    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-
-    parser.add_argument('-a', '--annot', action='store', required=True,
-                        help='The annotation file for which the staffline and staff'
-                             ' Node relationships should be added.')
-    parser.add_argument('-e', '--export', action='store',
-                        help='A filename to which the output NodeList'
-                             ' should be saved. If not given, will print to'
-                             ' stdout.')
-    parser.add_argument('-m', '--midi', action='store',
-                        help='A filename to which to export the MIDI file'
-                             ' for the given score.')
-
-    parser.add_argument('-v', '--verbose', action='store_true',
-                        help='Turn on INFO messages.')
-    parser.add_argument('--debug', action='store_true',
-                        help='Turn on DEBUG messages.')
-    return parser
-
-
-##############################################################################
-
-
-def main(args):
-    logging.info('Starting main...')
-    _start_time = time.clock()
-
-    # Your code goes here
-    if not os.path.isfile(args.annot):
-        raise ValueError('Annotation file {0} not found!'
-                         ''.format(args.annot))
-    nodes = read_nodes_from_file(args.annot)
-
-    pitch_inference_engine = PitchInferenceEngine()
-    time_inference_engine = OnsetsInferenceEngine(nodes=nodes)
-
-    logging.info('Running pitch inference.')
-    pitches, pitch_names = pitch_inference_engine.infer_pitches(nodes, with_names=True)
-
-    # Export
-    logging.info('Adding pitch information to <Data> attributes.')
-    for node in nodes:
-        if node.id in pitches:
-            midi_pitch_code = pitches[node.id]
-            pitch_step, pitch_octave = pitch_names[node.id]
-            if node.data is None:
-                node.data = dict()
-            node.data['midi_pitch_code'] = midi_pitch_code
-            node.data['normalized_pitch_step'] = pitch_step
-            node.data['pitch_octave'] = pitch_octave
-
-    logging.info('Adding duration info to <Data> attributes.')
-    durations = time_inference_engine.durations(nodes)
-    logging.info('Total durations: {0}'.format(len(durations)))
-    for node in nodes:
-        if node.id in durations:
-            node.data['duration_beats'] = durations[node.id]
-
-    logging.info('Some durations: {0}'.format(sorted(durations.items())[:10]))
-
-    logging.info('Adding onset info to <Data> attributes.')
-    onsets = time_inference_engine.onsets(nodes)
-    logging.info('Total onsets: {0}'.format(len(onsets)))
-    for node in nodes:
-        if node.id in onsets:
-            node.data['onset_beats'] = onsets[node.id]
-
-    if args.export is not None:
-        with open(args.export, 'w') as hdl:
-            hdl.write(export_node_list(nodes))
-            hdl.write('\n')
-    else:
-        print(export_node_list(nodes))
-
-    if args.midi is not None:
-        midi_builder = MIDIBuilder()
-        mf = midi_builder.build_midi(pitches, durations, onsets)
-        with open(args.midi, 'wb') as hdl:
-            mf.writeFile(hdl)
-
-    _end_time = time.clock()
-    logging.info('infer_pitches.py done in {0:.3f} s'.format(_end_time - _start_time))
-
-
-if __name__ == '__main__':
-    parser = build_argument_parser()
-    args = parser.parse_args()
-
-    if args.verbose:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
-    if args.debug:
-        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
-
-    main(args)
+#!/usr/bin/env python
+"""This is a script that takes the full-grown notation graph
+and recovers for each notehead the pitch to which it corresponds.
+
+Assumptions
+-----------
+
+* Clefs are used in a standard way: G-clef on 4th, C-clef on 3rd, F-clef
+  on 2nd staffline.
+* Key signatures are used in a standard way, so that we can rely on counting
+  the accidentals.
+* Accidentals are valid up until the end of the bar.
+
+We are currently NOT processing any transpositions.
+
+Representation
+--------------
+
+Notes are not noteheads. Pitch is associated with a note, and it is derived
+from the notehead's subgraph. The current goal of this exercise is obtaining
+MIDI, so we discard in effect information about what is e.g. a G-sharp
+and A-flat.
+
+"""
+import argparse
+import logging
+import os
+import time
+
+from mung2midi.run_inference import build_midi
+from mung2midi.inference import PitchInferenceEngine, OnsetsInferenceEngine
+from mung.io import read_nodes_from_file, export_node_list
+
+
+def build_argument_parser():
+    parser = argparse.ArgumentParser(description=__doc__, add_help=True,
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+
+    parser.add_argument('-a', '--annot', action='store', required=True,
+                        help='The annotation file for which the staffline and staff'
+                             ' Node relationships should be added.')
+    parser.add_argument('-e', '--export', action='store',
+                        help='A filename to which the output NodeList'
+                             ' should be saved. If not given, will print to'
+                             ' stdout.')
+    parser.add_argument('-m', '--midi', action='store',
+                        help='A filename to which to export the MIDI file'
+                             ' for the given score.')
+
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='Turn on INFO messages.')
+    parser.add_argument('--debug', action='store_true',
+                        help='Turn on DEBUG messages.')
+    return parser
+
+
+##############################################################################
+
+
+def main(args):
+    logging.info('Starting main...')
+    _start_time = time.clock()
+
+    # Your code goes here
+    if not os.path.isfile(args.annot):
+        raise ValueError('Annotation file {0} not found!'
+                         ''.format(args.annot))
+    nodes = read_nodes_from_file(args.annot)
+
+    pitch_inference_engine = PitchInferenceEngine()
+    time_inference_engine = OnsetsInferenceEngine(nodes=nodes)
+
+    logging.info('Running pitch inference.')
+    pitches, pitch_names = pitch_inference_engine.infer_pitches(nodes, with_names=True)
+
+    # Export
+    logging.info('Adding pitch information to <Data> attributes.')
+    for node in nodes:
+        if node.id in pitches:
+            midi_pitch_code = pitches[node.id]
+            pitch_step, pitch_octave = pitch_names[node.id]
+            if node.data is None:
+                node.data = dict()
+            node.data['midi_pitch_code'] = midi_pitch_code
+            node.data['normalized_pitch_step'] = pitch_step
+            node.data['pitch_octave'] = pitch_octave
+
+    logging.info('Adding duration info to <Data> attributes.')
+    durations = time_inference_engine.durations(nodes)
+    logging.info('Total durations: {0}'.format(len(durations)))
+    for node in nodes:
+        if node.id in durations:
+            node.data['duration_beats'] = durations[node.id]
+
+    logging.info('Some durations: {0}'.format(sorted(durations.items())[:10]))
+
+    logging.info('Adding onset info to <Data> attributes.')
+    onsets = time_inference_engine.onsets(nodes)
+    logging.info('Total onsets: {0}'.format(len(onsets)))
+    for node in nodes:
+        if node.id in onsets:
+            node.data['onset_beats'] = onsets[node.id]
+
+    if args.export is not None:
+        with open(args.export, 'w') as hdl:
+            hdl.write(export_node_list(nodes))
+            hdl.write('\n')
+    else:
+        print(export_node_list(nodes))
+
+    if args.midi is not None:
+        mf = build_midi(pitches, durations, onsets)
+        with open(args.midi, 'wb') as hdl:
+            mf.writeFile(hdl)
+
+    _end_time = time.clock()
+    logging.info('infer_pitches.py done in {0:.3f} s'.format(_end_time - _start_time))
+
+
+if __name__ == '__main__':
+    parser = build_argument_parser()
+    args = parser.parse_args()
+
+    if args.verbose:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
+    if args.debug:
+        logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG)
+
+    main(args)
```

### Comparing `mung-1.1/setup.py` & `mung-1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,77 @@
-from setuptools import setup
-import io
-import logging
-import os
-
-import mung
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-
-def read(*filenames, **kwargs):
-    encoding = kwargs.get('encoding', 'utf-8')
-    sep = kwargs.get('sep', '\n')
-    buf = []
-    for filename in filenames:
-        with io.open(filename, encoding=encoding) as f:
-            buf.append(f.read())
-    return sep.join(buf)
-
-
-def get_long_description():
-    readme = os.path.join(here, 'README.md')
-    changes = os.path.join(here, 'CHANGES.md')
-
-    if os.path.isfile(readme) and os.path.isfile(changes):
-        long_description = read(readme, changes)
-    else:
-        logging.warning('Could not find README.md and CHANGES.md file'
-                        ' in directory {0}. Contents:'
-                        ' {1}'.format(here, os.listdir(here)))
-        long_description = 'Tools for the Music Notation Graph representation of' \
-                           ' music notation, used primarily for optical music' \
-                           ' recognition. The MUSCIMA++ dataset uses this data' \
-                           ' model. Supports export to MIDI. [README.md and' \
-                           ' CHANGES.md not found]'
-    return long_description
-
-
-setup(
-    name='mung',
-    version=mung.__version__,
-    url='https://mung.readthedocs.io',
-    license='MIT Software License',
-    author='Jan Hajič jr. and Alexander Pacha',
-    install_requires=['numpy>=1.11.1',
-                      'lxml>=3.6.4'],
-    author_email='alexander.pacha@tuwien.ac.at',
-    description='Tools for the Music Notation Graph representation of music notation, used primarily for optical music recognition.',
-    long_description=get_long_description(),
-    long_description_content_type="text/markdown",
-    packages=['mung', 'mung2midi'],
-    include_package_data=True,
-    scripts=['scripts/add_staff_relationships.py',
-             'scripts/add_staffline_symbols.py',
-             'scripts/analyze_agreement.py',
-             'scripts/analyze_annotations.py',
-             'scripts/analyze_tracking_log.py',
-             'scripts/baseline_process_symbols.py',
-             'scripts/get_images_from_muscima.py',
-             'scripts/infer_pitches.py',
-             'scripts/strip_staffline_symbols.py',
-             ],
-    platforms='any',
-    test_suite='test.test_mung',
-    classifiers=[
-        'Programming Language :: Python',
-        'Development Status :: 4 - Beta',
-        'Natural Language :: English',
-        'Environment :: Web Environment',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
-    ],
-)
+from setuptools import setup
+import io
+import logging
+import os
+
+import mung
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+
+def read(*filenames, **kwargs):
+    encoding = kwargs.get('encoding', 'utf-8')
+    sep = kwargs.get('sep', '\n')
+    buf = []
+    for filename in filenames:
+        with io.open(filename, encoding=encoding) as f:
+            buf.append(f.read())
+    return sep.join(buf)
+
+
+def get_long_description():
+    readme = os.path.join(here, 'README.md')
+    changes = os.path.join(here, 'CHANGES.md')
+
+    if os.path.isfile(readme) and os.path.isfile(changes):
+        long_description = read(readme, changes)
+    else:
+        logging.warning(
+            'Could not find README.md and CHANGES.md file'
+            ' in directory {0}. Contents:'
+            ' {1}'.format(here, os.listdir(here))
+            )
+        long_description = 'Tools for the Music Notation Graph representation of' \
+                           ' music notation, used primarily for optical music' \
+                           ' recognition. The MUSCIMA++ dataset uses this data' \
+                           ' model. Supports export to MIDI. [README.md and' \
+                           ' CHANGES.md not found]'
+    return long_description
+
+
+setup(
+    name='mung',
+    version=mung.__version__,
+    url='https://mung.readthedocs.io',
+    license='MIT Software License',
+    author='Jan Hajič jr. and Alexander Pacha',
+    install_requires=['numpy', 'lxml', 'scikit-image'],
+    author_email='alexander.pacha@tuwien.ac.at',
+    description='Tools for the Music Notation Graph representation of music notation, used primarily for optical '
+                'music recognition.',
+    long_description=get_long_description(),
+    long_description_content_type="text/markdown",
+    packages=['mung', 'mung2midi'],
+    include_package_data=True,
+    scripts=['scripts/add_staff_relationships.py',
+             'scripts/add_staffline_symbols.py',
+             'scripts/analyze_agreement.py',
+             'scripts/analyze_annotations.py',
+             'scripts/analyze_tracking_log.py',
+             'scripts/baseline_process_symbols.py',
+             'scripts/get_images_from_muscima.py',
+             'scripts/infer_pitches.py',
+             'scripts/strip_staffline_symbols.py',
+             ],
+    platforms='any',
+    test_suite='test.test_mung',
+    classifiers=[
+        'Programming Language :: Python',
+        'Development Status :: 4 - Beta',
+        'Natural Language :: English',
+        'Environment :: Web Environment',
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
+    ],
+)
```

### Comparing `mung-1.1/test/test_grammar.py` & `mung-1.2/test/test_grammar.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from mung.grammar import DependencyGrammar
-from mung.io import parse_node_classes
-
-import os
-import unittest
-
-
-class GrammarTest(unittest.TestCase):
-    def test_parse_grammar(self):
-        filepath = os.path.dirname(
-            os.path.dirname(__file__)) + u'/test/test_data/mff-muscima-classes-annot.deprules'
-        node_classes_path = os.path.dirname(
-            os.path.dirname(__file__)) + u'/test/test_data/mff-muscima-classes-annot.xml'
-        node_classes = parse_node_classes(node_classes_path)
-        node_classes_dict = {node_class.name for node_class in node_classes}
-        dependency_graph = DependencyGrammar(grammar_filename=filepath, alphabet=node_classes_dict)
-        self.assertEqual(646, len(dependency_graph.rules))
-
-
-if __name__ == '__main__':
-    unittest.main()
+from mung.grammar import DependencyGrammar
+from mung.io import parse_node_classes
+
+import os
+import unittest
+
+
+class GrammarTest(unittest.TestCase):
+    def test_parse_grammar(self):
+        filepath = os.path.dirname(
+            os.path.dirname(__file__)) + u'/test/test_data/mff-muscima-classes-annot.deprules'
+        node_classes_path = os.path.dirname(
+            os.path.dirname(__file__)) + u'/test/test_data/mff-muscima-classes-annot.xml'
+        node_classes = parse_node_classes(node_classes_path)
+        node_classes_dict = {node_class.name for node_class in node_classes}
+        dependency_graph = DependencyGrammar(grammar_filename=filepath, alphabet=node_classes_dict)
+        self.assertEqual(646, len(dependency_graph.rules))
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `mung-1.1/test/test_node.py` & `mung-1.2/test/test_node.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import os
-import unittest
-
-from mung.io import read_nodes_from_file, export_node_list
-from mung.node import Node
-
-
-class NodeTest(unittest.TestCase):
-    def test_bbox_to_integer_bounds(self):
-        # Arrange
-        expected = (44, 18, 56, 93)
-        expected2 = (44, 18, 56, 93)
-
-        # Act
-        actual = Node.round_bounding_box_to_integer(44.2, 18.9, 55.1, 92.99)
-        actual2 = Node.round_bounding_box_to_integer(44, 18, 56, 92.99)
-
-        # Assert
-        self.assertEqual(actual, expected)
-        self.assertEqual(actual2, expected2)
-
-    def test_overlaps(self):
-        # Arrange
-        node = Node(0, 'test', 10, 100, height=20, width=10)
-
-        # Act and Assert
-        self.assertEqual(node.bounding_box, (10, 100, 30, 110))
-
-        self.assertTrue(node.overlaps((10, 100, 30, 110)))  # Exact match
-
-        self.assertFalse(node.overlaps((0, 100, 8, 110)))  # Row mismatch
-        self.assertFalse(node.overlaps((10, 0, 30, 89)))  # Column mismatch
-        self.assertFalse(node.overlaps((0, 0, 8, 89)))  # Total mismatch
-
-        self.assertTrue(node.overlaps((9, 99, 31, 111)))  # Encompasses Node
-        self.assertTrue(node.overlaps((11, 101, 29, 109)))  # Within Node
-        self.assertTrue(node.overlaps((9, 101, 31, 109)))  # Encompass horz., within vert.
-        self.assertTrue(node.overlaps((11, 99, 29, 111)))  # Encompasses vert., within horz.
-        self.assertTrue(node.overlaps((11, 101, 31, 111)))  # Corner within: top left
-        self.assertTrue(node.overlaps((11, 99, 31, 109)))  # Corner within: top right
-        self.assertTrue(node.overlaps((9, 101, 29, 111)))  # Corner within: bottom left
-        self.assertTrue(node.overlaps((9, 99, 29, 109)))  # Corner within: bottom right
-
-    def test_read_nodes_from_file(self):
-        test_data_dir = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'test', 'test_data')
-        clfile = os.path.join(test_data_dir, '01_basic.xml')
-        nodes = read_nodes_from_file(clfile)
-        self.assertEqual(len(nodes), 48)
-
-    def test_read_nodes_from_file_with_data(self):
-        test_data_dir = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'test', 'test_data')
-        file = os.path.join(test_data_dir, '01_basic_binary.xml')
-        nodes = read_nodes_from_file(file)
-        self.assertEqual("G", nodes[0].data['pitch_step'])
-        self.assertEqual(79, nodes[0].data['midi_pitch_code'])
-        self.assertEqual([8, 17], nodes[0].data['precedence_outlinks'])
-
-
-if __name__ == '__main__':
-    unittest.main()
+import os
+import unittest
+
+from mung.io import read_nodes_from_file, export_node_list
+from mung.node import Node
+
+
+class NodeTest(unittest.TestCase):
+    def test_bbox_to_integer_bounds(self):
+        # Arrange
+        expected = (44, 18, 56, 93)
+        expected2 = (44, 18, 56, 93)
+
+        # Act
+        actual = Node.round_bounding_box_to_integer(44.2, 18.9, 55.1, 92.99)
+        actual2 = Node.round_bounding_box_to_integer(44, 18, 56, 92.99)
+
+        # Assert
+        self.assertEqual(actual, expected)
+        self.assertEqual(actual2, expected2)
+
+    def test_overlaps(self):
+        # Arrange
+        node = Node(0, 'test', 10, 100, height=20, width=10)
+
+        # Act and Assert
+        self.assertEqual(node.bounding_box, (10, 100, 30, 110))
+
+        self.assertTrue(node.overlaps((10, 100, 30, 110)))  # Exact match
+
+        self.assertFalse(node.overlaps((0, 100, 8, 110)))  # Row mismatch
+        self.assertFalse(node.overlaps((10, 0, 30, 89)))  # Column mismatch
+        self.assertFalse(node.overlaps((0, 0, 8, 89)))  # Total mismatch
+
+        self.assertTrue(node.overlaps((9, 99, 31, 111)))  # Encompasses Node
+        self.assertTrue(node.overlaps((11, 101, 29, 109)))  # Within Node
+        self.assertTrue(node.overlaps((9, 101, 31, 109)))  # Encompass horz., within vert.
+        self.assertTrue(node.overlaps((11, 99, 29, 111)))  # Encompasses vert., within horz.
+        self.assertTrue(node.overlaps((11, 101, 31, 111)))  # Corner within: top left
+        self.assertTrue(node.overlaps((11, 99, 31, 109)))  # Corner within: top right
+        self.assertTrue(node.overlaps((9, 101, 29, 111)))  # Corner within: bottom left
+        self.assertTrue(node.overlaps((9, 99, 29, 109)))  # Corner within: bottom right
+
+    def test_read_nodes_from_file(self):
+        test_data_dir = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'test', 'test_data')
+        clfile = os.path.join(test_data_dir, '01_basic.xml')
+        nodes = read_nodes_from_file(clfile)
+        self.assertEqual(len(nodes), 48)
+
+    def test_read_nodes_from_file_with_data(self):
+        test_data_dir = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'test', 'test_data')
+        file = os.path.join(test_data_dir, '01_basic_binary_2.0.xml')
+        nodes = read_nodes_from_file(file)
+        self.assertEqual("G", nodes[0].data['pitch_step'])
+        self.assertEqual(79, nodes[0].data['midi_pitch_code'])
+        self.assertEqual([8, 17], nodes[0].data['precedence_outlinks'])
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `mung-1.1/test/test_node_class.py` & `mung-1.2/test/test_node_class.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-import unittest
-
-from mung.io import parse_node_classes
-from mung.node_class import NodeClass
-
-
-class NodeClassTest(unittest.TestCase):
-    def test_note_class_to_string(self):
-        # Arrange
-        expected = """<NodeClass>
-    <Id>1</Id>
-    <Name>noteheadFull</Name>
-    <GroupName>primitives</GroupName>
-    <Color>#FF6689</Color>
-</NodeClass>"""
-        node_class = NodeClass(1, "noteheadFull", "primitives", "#FF6689")
-
-        # Act
-        actual = str(node_class)
-
-        # Assert
-        self.assertEqual(actual, expected)
-
-    def test_node_class_parsing(self):
-        # Arrange
-        expected_number_of_classes = 163
-
-        # Act
-        node_classes = parse_node_classes("test/test_data/mff-muscima-classes-annot.xml")
-
-        # Assert
-        self.assertEqual(len(node_classes), expected_number_of_classes)
-        self.assertEqual(node_classes[0].name, "noteheadFull")
-
-
-if __name__ == '__main__':
-    unittest.main()
+import os
+import unittest
+
+from mung.io import parse_node_classes
+from mung.node_class import NodeClass
+
+
+class NodeClassTest(unittest.TestCase):
+    def test_note_class_to_string(self):
+        # Arrange
+        expected = """<NodeClass>
+    <Id>1</Id>
+    <Name>noteheadFull</Name>
+    <GroupName>primitives</GroupName>
+    <Color>#FF6689</Color>
+</NodeClass>"""
+        node_class = NodeClass(1, "noteheadFull", "primitives", "#FF6689")
+
+        # Act
+        actual = str(node_class)
+
+        # Assert
+        self.assertEqual(actual, expected)
+
+    def test_node_class_parsing(self):
+        # Arrange
+        expected_number_of_classes = 163
+
+        # Act
+        test_data_dir = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'test', 'test_data')
+        classes_file = os.path.join(test_data_dir, 'mff-muscima-classes-annot.xml')
+
+        node_classes = parse_node_classes(classes_file)
+
+        # Assert
+        self.assertEqual(len(node_classes), expected_number_of_classes)
+        self.assertEqual(node_classes[0].name, "noteheadFull")
+
+
+if __name__ == '__main__':
+    unittest.main()
```

