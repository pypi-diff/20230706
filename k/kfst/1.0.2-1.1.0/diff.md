# Comparing `tmp/kfst-1.0.2.tar.gz` & `tmp/kfst-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfst-1.0.2.tar", last modified: Wed Jul  5 23:46:04 2023, max compression
+gzip compressed data, was "kfst-1.1.0.tar", last modified: Thu Jul  6 21:09:07 2023, max compression
```

## Comparing `kfst-1.0.2.tar` & `kfst-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-05 23:46:04.701924 kfst-1.0.2/
--rw-r--r--   0 iikka      (501) staff       (20)     7653 2023-07-05 12:46:55.000000 kfst-1.0.2/LICENSE
--rw-r--r--   0 iikka      (501) staff       (20)     1853 2023-07-05 23:46:04.701962 kfst-1.0.2/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)     1221 2023-07-05 12:46:53.000000 kfst-1.0.2/README.md
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-05 23:46:04.701309 kfst-1.0.2/kfst/
--rw-r--r--   0 iikka      (501) staff       (20)      742 2023-07-05 14:15:18.000000 kfst-1.0.2/kfst/__init__.py
--rw-r--r--   0 iikka      (501) staff       (20)    11303 2023-07-05 23:44:27.000000 kfst-1.0.2/kfst/transducer.py
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-05 23:46:04.701841 kfst-1.0.2/kfst.egg-info/
--rw-r--r--   0 iikka      (501) staff       (20)     1853 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)      217 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/SOURCES.txt
--rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/dependency_links.txt
--rw-r--r--   0 iikka      (501) staff       (20)       11 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/requires.txt
--rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/top_level.txt
--rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:15.000000 kfst-1.0.2/pyproject.toml
--rw-r--r--   0 iikka      (501) staff       (20)      756 2023-07-05 23:46:04.702140 kfst-1.0.2/setup.cfg
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:09:07.316405 kfst-1.1.0/
+-rw-r--r--   0 iikka      (501) staff       (20)     7653 2023-07-05 12:46:55.000000 kfst-1.1.0/LICENSE
+-rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-06 21:09:07.316444 kfst-1.1.0/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)     1456 2023-07-06 13:42:57.000000 kfst-1.1.0/README.md
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:09:07.315817 kfst-1.1.0/kfst/
+-rw-r--r--   0 iikka      (501) staff       (20)      742 2023-07-05 14:15:18.000000 kfst-1.1.0/kfst/__init__.py
+-rw-r--r--   0 iikka      (501) staff       (20)      495 2023-07-06 13:08:58.000000 kfst-1.1.0/kfst/convert.py
+-rw-r--r--   0 iikka      (501) staff       (20)    17180 2023-07-06 20:44:56.000000 kfst-1.1.0/kfst/transducer.py
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:09:07.316330 kfst-1.1.0/kfst.egg-info/
+-rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)      233 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/SOURCES.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/dependency_links.txt
+-rw-r--r--   0 iikka      (501) staff       (20)       11 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/requires.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/top_level.txt
+-rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:15.000000 kfst-1.1.0/pyproject.toml
+-rw-r--r--   0 iikka      (501) staff       (20)      708 2023-07-06 21:09:07.316630 kfst-1.1.0/setup.cfg
```

### Comparing `kfst-1.0.2/LICENSE` & `kfst-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kfst-1.0.2/PKG-INFO` & `kfst-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: kfst
-Version: 1.0.2
-Summary: A pure-python finite state transducer library with support for AT&T files and flag diacritics
+Version: 1.1.0
+Summary: A pure-python finite state transducer library
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU LGPLv3 or later
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KFST
 
-KFST is a finite state transducer library written in pure Python. It supports reading transducers from [AT&T tabular format](https://github.com/hfst/hfst/blob/master/doc/transducer-representations-formats.rst) files. In addition to standard features, it also supports flag diacritics.
+KFST is a finite state transducer library written in pure Python. It supports reading transducers from [AT&T tabular format](https://github.com/hfst/hfst/blob/master/doc/transducer-representations-formats.rst) files and its own binary format.
+In addition to standard features, it also supports flag diacritics.
 
 The intended use case is to use KFST in environments in which native libraries like HFST cannot be installed.
 
 ## Installation
 
 KFST is available on PyPI and can be installed with pip:
 
@@ -31,24 +32,29 @@
 ## Usage
 
 In this example, we assume that you have a transducer stored in the file `my-transducer.att`.
 You can easily create such file using the HFST toolkit:
 
 ```sh
 hfst-fst2txt -f att my-transducer.hfst > my-transducer.att
+
+# if you want a kfst file:
+python -m kfst.convert my-transducer.att my-transducer.kfst
 ```
 
 ### Reading transducers
 
-Transducers can be read from AT&T tabular format files using the `read_att` function:
+Transducers can be read from AT&T tabular format files using the `read_att_file` function, and the KFST binary format using the `read_kfst_file` function:
 
 ```python
 from kfst import FST
 
 fst = FST.read_att_file("my-transducer.att")
+# or
+fst = FST.read_kfst_file("my-transducer.kfst")
 ```
 
 ### Using the transducer
 
 To run the transducer, use the `lookup` method, which returns a list of tuples of the form `(output, weight)` sorted by weight:
 
 ```python
```

### Comparing `kfst-1.0.2/README.md` & `kfst-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # KFST
 
-KFST is a finite state transducer library written in pure Python. It supports reading transducers from [AT&T tabular format](https://github.com/hfst/hfst/blob/master/doc/transducer-representations-formats.rst) files. In addition to standard features, it also supports flag diacritics.
+KFST is a finite state transducer library written in pure Python. It supports reading transducers from [AT&T tabular format](https://github.com/hfst/hfst/blob/master/doc/transducer-representations-formats.rst) files and its own binary format.
+In addition to standard features, it also supports flag diacritics.
 
 The intended use case is to use KFST in environments in which native libraries like HFST cannot be installed.
 
 ## Installation
 
 KFST is available on PyPI and can be installed with pip:
 
@@ -15,24 +16,29 @@
 ## Usage
 
 In this example, we assume that you have a transducer stored in the file `my-transducer.att`.
 You can easily create such file using the HFST toolkit:
 
 ```sh
 hfst-fst2txt -f att my-transducer.hfst > my-transducer.att
+
+# if you want a kfst file:
+python -m kfst.convert my-transducer.att my-transducer.kfst
 ```
 
 ### Reading transducers
 
-Transducers can be read from AT&T tabular format files using the `read_att` function:
+Transducers can be read from AT&T tabular format files using the `read_att_file` function, and the KFST binary format using the `read_kfst_file` function:
 
 ```python
 from kfst import FST
 
 fst = FST.read_att_file("my-transducer.att")
+# or
+fst = FST.read_kfst_file("my-transducer.kfst")
 ```
 
 ### Using the transducer
 
 To run the transducer, use the `lookup` method, which returns a list of tuples of the form `(output, weight)` sorted by weight:
 
 ```python
```

### Comparing `kfst-1.0.2/kfst/__init__.py` & `kfst-1.1.0/kfst/__init__.py`

 * *Files identical despite different names*

### Comparing `kfst-1.0.2/kfst/transducer.py` & `kfst-1.1.0/kfst/transducer.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with KFST. If not, see <https://www.gnu.org/licenses/>. 
 
 import argparse
+import lzma
 import re
+import struct
 from collections import defaultdict
 from pathlib import Path
 from typing import NamedTuple
 
 from frozendict import frozendict
 
 
@@ -36,15 +38,15 @@
 
 
 class FST(NamedTuple):
     """
     Represents a finite state transducer
     """
     final_states: dict[int, float]
-    rules: defaultdict[int, defaultdict[str, list[tuple[int, str, int]]]]
+    rules: defaultdict[int, defaultdict[str, list[tuple[int, str, float]]]]
     symbols: set[str]
     debug: bool = False
 
     @staticmethod
     def from_att_file(att_file: str | Path, debug: bool = False) -> "FST":
         """
         Parses a transducer in A&AT format and returns an FST object.
@@ -97,14 +99,107 @@
                 fst.symbols.add(fields[3])
 
             else:
                 raise RuntimeError("Cannot parse line:", line)
 
         return fst
 
+    @staticmethod
+    def from_kfst_file(kfst_file: str | Path, debug: bool = False) -> "FST":
+        """
+        Parses a transducer in the KFST binary format and returns an FST object.
+        The input must be the path to the .kfst file.
+
+        If you already have the content of the .kfst file, use FST.from_kfst_bytes() instead.
+
+        If you use HFST, .kfst files can be created using the command:
+        ```sh
+        python -m kfst.convert file.hfst file.kfst
+        ```
+        """
+        if not isinstance(kfst_file, Path):
+            kfst_file = Path(kfst_file)
+
+        kfst_bytes = kfst_file.read_bytes()
+        return FST.from_kfst_bytes(kfst_bytes, debug=debug)
+
+    @staticmethod
+    def from_kfst_bytes(kfst_bytes: bytes, debug: bool = False) -> "FST":
+        """
+        Parses a transducer in the KFST binary format and returns an FST object.
+
+        Note that the input must be the content of the .kfst file, not the path to the file.
+        For that, use FST.from_kfst_file() instead.
+        """
+
+        fst = FST(
+            final_states={},
+            rules=defaultdict(lambda: defaultdict(list)),
+            symbols=set(),
+            debug=debug,
+        )
+
+        reader = KFSTReader(kfst_bytes)
+        reader.read_into(fst)
+        
+        return fst
+
+    def to_kfst_file(self, path: str | Path):
+        """
+        Encodes the FST in the KFST binary format and writes it to the given path.
+        """
+        if not isinstance(path, Path):
+            path = Path(path)
+
+        path.write_bytes(self.to_kfst_bytes())
+        
+    def to_kfst_bytes(self) -> bytes:
+        """
+        Encodes the FST in the KFST binary format.
+        """
+
+        is_weighted = any(weight != 0 for weight in self.final_states.values()) or any(weight != 0 for state in self.rules.values() for transitions in state.values() for _, _, weight in transitions)
+
+        assert len(self.symbols) <= 2**16, "Too many symbols"
+
+        num_rules = sum(len(transitions) for state in self.rules.values() for transitions in state.values())
+
+        assert num_rules <= 2**32, "Too many rules"
+        assert len(self.final_states) <= 2**32, "Too many final states"
+
+        buffer = bytes()
+        buffer += b"KFST"
+        buffer += struct.pack("!H", 0) # version
+        buffer += struct.pack("!HII?", len(self.symbols), num_rules, len(self.final_states), is_weighted) # header
+
+        # Write symbols
+        symbols_list = sorted(self.symbols)
+        for symbol in symbols_list:
+            buffer += symbol.encode("utf-8") + b"\x00"
+
+        state_bytes = []
+        
+        # Write states
+        for from_state, transitions in self.rules.items():
+            for input_symbol, transitions_list in transitions.items():
+                for to_state, output_symbol, weight in transitions_list:
+                    state_bytes.append(struct.pack("!IIHH", from_state, to_state, symbols_list.index(input_symbol), symbols_list.index(output_symbol)))
+                    if is_weighted:
+                        state_bytes.append(struct.pack("!d", weight))
+        
+        # Write final states
+        for state, weight in self.final_states.items():
+            state_bytes.append(struct.pack("!I", state))
+            if is_weighted:
+                state_bytes.append(struct.pack("!d", weight))
+        
+        data = b"".join(state_bytes)
+        buffer += lzma.compress(data)
+        return buffer
+
     def split_to_symbols(self, text: str) -> list[str] | None:
         """
         Splits a given string into a list of symbols.
         For each position in the string, greedily selects the longest symbol that matches.
 
         Returns None if the string cannot be split into symbols.
         """
@@ -182,14 +277,15 @@
         Runs the FST on the given input symbols, starting from the given state (by default 0).
         Yields a tuple of (output_symbols, path_weight) for each successful path.
         
         Otherwise same as run_fst, but operates on strings instead of symbol lists, filters out duplicate outputs and sorts the results by weight.
         """
 
         input_symbols = self.split_to_symbols(input)
+        assert input_symbols is not None, "Input cannot be split into symbols"
         results = self.run_fst(input_symbols, state=state)
         results = sorted(results, key=lambda x: x[1])
         already_seen = set()
         for os, w in results:
             o = "".join(os)
             if o not in already_seen:
                 yield o, w
@@ -278,25 +374,94 @@
         return False
 
     def _is_epsilon(self, symbol: str) -> bool:
         # flag diacritics are treated like epsilon symbols
         return symbol == "@0@" or symbol == "@_EPSILON_SYMBOL_@" or self._is_flag(symbol)
     
     def _is_flag(self, symbol: str) -> bool:
-        return re.match(r"^@[PNDRCU]\.", symbol)
+        return bool(re.match(r"^@[PNDRCU]\.", symbol))
+
+
+class KFSTReader:
+
+    def __init__(self, buffer):
+        self.buffer = buffer
+        self.pointer = 0
+
+    def read_into(self, fst: FST):
+        # Validate signature
+        assert self.buffer[:4] == b"KFST"
+        self.pointer += 4
+
+        # Parse version
+        (version,) = self.unpack_and_advance("!H")
+
+        assert version == 0, "Unsupported KFST binary file version"
+
+        # Parse header
+        num_symbols, num_states, num_final_states, is_weighted = self.unpack_and_advance("!HII?")
+
+        # Parse symbols
+        symbols_list = []
+        for _ in range(num_symbols):
+            symbol = self.read_null_terminated_string()
+            symbol_string = symbol.decode("utf-8")
+            fst.symbols.add(symbol_string)
+            symbols_list.append(symbol_string)
+        
+        lzma_data = self.buffer[self.pointer:]
+        self.buffer = lzma.decompress(lzma_data)
+        self.pointer = 0
+        
+        # Parse states
+        for _ in range(num_states):
+            from_state, to_state, input_symbol, output_symbol = self.unpack_and_advance("!IIHH")
+            weight = 0
+
+            if is_weighted:
+                (weight,) = self.unpack_and_advance("!d")
+
+            fst.rules[from_state][symbols_list[input_symbol]].append((to_state, symbols_list[output_symbol], weight))
+        
+        # Parse final states
+        for _ in range(num_final_states):
+            (state,) = self.unpack_and_advance("!I")
+            weight = 0
+            if is_weighted:
+                (weight,) = self.unpack_and_advance("!d")
+            
+            fst.final_states[state] = weight
+
+    def unpack_and_advance(self, format: str):
+        size = struct.calcsize(format)
+        ans = struct.unpack(format, self.buffer[self.pointer:self.pointer+size])
+        self.pointer += size
+        return ans
+
+    def read_null_terminated_string(self) -> bytes:
+        i = self.buffer[self.pointer:].find(b"\x00")
+        string = self.buffer[self.pointer:self.pointer+i]
+        self.pointer += i + 1
+        return string
 
 
 def main():
     parser = argparse.ArgumentParser(description="Finite State Transducer interpreter written in Python")
-    parser.add_argument("att_file", type=Path, help="FST in AT&T format")
+    parser.add_argument("fst_file", type=Path, help="FST in AT&T or KFST format")
     parser.add_argument("-d", action="store_true", help="enable debug mode")
     parser.add_argument("-s", action="store_true", help="print symbols in transducer and exit")
+    parser.add_argument("-f", choices=["att", "kfst", "auto"], default="auto", help="force input format")
     args = parser.parse_args()
 
-    fst = FST.from_att_file(args.att_file, debug=args.d)
+    if args.fst_file.suffix == ".kfst" if args.f == "auto" else args.f == "kfst":
+        fst =  FST.from_kfst_file(args.fst_file, debug=args.d)
+    
+    else:
+        fst = FST.from_att_file(args.fst_file, debug=args.d)
+    
     if args.s:
         print(sorted(fst.symbols))
         return
 
     if args.d:
         print(sorted(fst.symbols))
         print(fst.final_states)
```

### Comparing `kfst-1.0.2/kfst.egg-info/PKG-INFO` & `kfst-1.1.0/kfst.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: kfst
-Version: 1.0.2
-Summary: A pure-python finite state transducer library with support for AT&T files and flag diacritics
+Version: 1.1.0
+Summary: A pure-python finite state transducer library
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU LGPLv3 or later
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KFST
 
-KFST is a finite state transducer library written in pure Python. It supports reading transducers from [AT&T tabular format](https://github.com/hfst/hfst/blob/master/doc/transducer-representations-formats.rst) files. In addition to standard features, it also supports flag diacritics.
+KFST is a finite state transducer library written in pure Python. It supports reading transducers from [AT&T tabular format](https://github.com/hfst/hfst/blob/master/doc/transducer-representations-formats.rst) files and its own binary format.
+In addition to standard features, it also supports flag diacritics.
 
 The intended use case is to use KFST in environments in which native libraries like HFST cannot be installed.
 
 ## Installation
 
 KFST is available on PyPI and can be installed with pip:
 
@@ -31,24 +32,29 @@
 ## Usage
 
 In this example, we assume that you have a transducer stored in the file `my-transducer.att`.
 You can easily create such file using the HFST toolkit:
 
 ```sh
 hfst-fst2txt -f att my-transducer.hfst > my-transducer.att
+
+# if you want a kfst file:
+python -m kfst.convert my-transducer.att my-transducer.kfst
 ```
 
 ### Reading transducers
 
-Transducers can be read from AT&T tabular format files using the `read_att` function:
+Transducers can be read from AT&T tabular format files using the `read_att_file` function, and the KFST binary format using the `read_kfst_file` function:
 
 ```python
 from kfst import FST
 
 fst = FST.read_att_file("my-transducer.att")
+# or
+fst = FST.read_kfst_file("my-transducer.kfst")
 ```
 
 ### Using the transducer
 
 To run the transducer, use the `lookup` method, which returns a list of tuples of the form `(output, weight)` sorted by weight:
 
 ```python
```

### Comparing `kfst-1.0.2/setup.cfg` & `kfst-1.1.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = kfst
-version = 1.0.2
+version = 1.1.0
 author = Iikka Hauhio
 author_email = iikka.hauhio@helsinki.fi
-description = A pure-python finite state transducer library with support for AT&T files and flag diacritics
+description = A pure-python finite state transducer library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv3 or later
 license_files = 
 	LICENSE
 url = https://github.com/fergusq/fst-python
 project_urls =
```

