# Comparing `tmp/miditok-2.1.0.tar.gz` & `tmp/miditok-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miditok-2.1.0.tar", last modified: Mon Jul  3 14:48:10 2023, max compression
+gzip compressed data, was "miditok-2.1.1.tar", last modified: Thu Jul  6 13:22:48 2023, max compression
```

## Comparing `miditok-2.1.0.tar` & `miditok-2.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.472050 miditok-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 14:48:00.000000 miditok-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-03 14:48:10.472050 miditok-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-03 14:48:00.000000 miditok-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.468050 miditok-2.1.0/miditok/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.468050 miditok-2.1.0/miditok/data_augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/data_augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/data_augmentation/data_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    73357 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/midi_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.472050 miditok-2.1.0/miditok/tokenizations/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/cp_word.py
--rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/midi_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/mmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/mumidi.py
--rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/octuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/octuple_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/remi.py
--rw-r--r--   0 runner    (1001) docker     (123)    26784 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/remi_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/tsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.472050 miditok-2.1.0/miditok/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.468050 miditok-2.1.0/miditok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:48:10.472050 miditok-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 14:48:00.000000 miditok-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.472050 miditok-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_multitrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_one_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_saving_loading_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/tests_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 13:22:37.000000 miditok-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-06 13:22:48.044588 miditok-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-06 13:22:37.000000 miditok-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.040588 miditok-2.1.1/miditok/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/miditok/data_augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/data_augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/data_augmentation/data_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73315 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/midi_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/miditok/tokenizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22611 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/cp_word.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/midi_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/mmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/mumidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20743 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/octuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/octuple_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/remi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26784 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/remi_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/tsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/miditok/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/miditok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:22:48.044588 miditok-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-06 13:22:37.000000 miditok-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_multitrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_one_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_saving_loading_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/tests_utils.py
```

### Comparing `miditok-2.1.0/LICENSE` & `miditok-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/PKG-INFO` & `miditok-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.1.0
+Version: 2.1.1
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `miditok-2.1.0/README.md` & `miditok-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/miditok/classes.py` & `miditok-2.1.1/miditok/classes.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/miditok/constants.py` & `miditok-2.1.1/miditok/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Constants for data encoding
 
 """
 
-CURRENT_VERSION_PACKAGE = "2.1.0"  # used when saving the config of a tokenizer
+CURRENT_VERSION_PACKAGE = "2.1.1"  # used when saving the config of a tokenizer
 
 MIDI_FILES_EXTENSIONS = [".mid", ".midi", ".MID", ".MIDI"]
 
 # Starting id of chr() method for BPE, as the 5 (0 to 4 included) firsts are ignored by 🤗tokenize
 # We also skip the 32nd (0x20) (space) as it causes issues when loading a BPE model with spaces in merged
 # Issue for reference: https://github.com/huggingface/tokenizers/issues/566
 # List of unicode characters: https://www.fileformat.info/info/charset/UTF-8/list.htm
```

### Comparing `miditok-2.1.0/miditok/data_augmentation/data_augmentation.py` & `miditok-2.1.1/miditok/data_augmentation/data_augmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,18 @@
                 dur_directions,
                 ids=ids,
             )
             augmented_tokens: Dict[
                 Tuple[int, int, int], List[Union[int, List[int]]]
             ] = {}
             for track, (_, is_drum) in zip(ids, programs):
-                if is_drum:  # we dont augment drums
+                # we dont augment drums
+                if not tokenizer.unique_track and is_drum:
+                    continue
+                elif tokenizer.unique_track and all(p[1] for p in programs):
                     continue
                 corrected_offsets = deepcopy(offsets)
                 vel_dim = int(128 / len(tokenizer.velocities))
                 corrected_offsets[1] = [
                     int(off / vel_dim) for off in corrected_offsets[1]
                 ]
                 aug = data_augmentation_tokens(
@@ -109,20 +112,21 @@
                     if tokenizer.unique_track:
                         augmented_tokens[aug_offsets] = seq
                         continue
                     try:
                         augmented_tokens[aug_offsets].append(seq)
                     except KeyError:
                         augmented_tokens[aug_offsets] = [seq]
-            for i, (track, (_, is_drum)) in enumerate(
-                zip(ids, programs)
-            ):  # adding drums to all already augmented
-                if is_drum:
-                    for aug_offsets in augmented_tokens:
-                        augmented_tokens[aug_offsets].insert(i, track)
+            if not tokenizer.unique_track:
+                for i, (track, (_, is_drum)) in enumerate(
+                    zip(ids, programs)
+                ):  # adding drums to all already augmented
+                    if is_drum:
+                        for aug_offsets in augmented_tokens:
+                            augmented_tokens[aug_offsets].insert(i, track)
 
             # Save augmented tracks as json
             for aug_offsets, tracks_seq in augmented_tokens.items():
                 if len(tracks_seq) == 0:
                     continue
                 suffix = "§" + "_".join(
                     [
@@ -134,14 +138,16 @@
                 saving_path = (
                     file_path.parent if out_path is None else out_path
                 ) / f"{file_path.stem}{suffix}.json"
                 tokenizer.save_tokens(tracks_seq, saving_path, programs)
                 nb_augmentations += 1
                 nb_tracks_augmented += len(tracks_seq)
             if copy_original_in_new_location and out_path is not None:
+                if tokenizer.unique_track:
+                    ids = ids[0]
                 tokenizer.save_tokens(
                     ids, out_path / f"{file_path.stem}.json", programs
                 )
 
         else:  # as midi
             try:
                 midi = MidiFile(file_path)
@@ -444,14 +450,25 @@
         if not tokenizer.is_multi_voc:
             pitch_tokens = np.array(
                 tokenizer.token_ids_of_type("Pitch")
                 + tokenizer.token_ids_of_type("NoteOn")
             )
             note_off_tokens = np.array(tokenizer.token_ids_of_type("NoteOff"))
             mask_pitch = np.isin(tokens, pitch_tokens)
+            # If applicable, removes drum notes from the mask
+            if tokenizer.unique_track:
+                for idx, is_note in enumerate(mask_pitch):
+                    if (
+                        is_note
+                        and idx > 0
+                        and tokenizer[tokens[idx - 1]] == "Program_-1"
+                    ):
+                        mask_pitch[idx] = False
+                        if len(note_off_tokens) > 0:
+                            note_off_tokens[idx] = False
         else:
             pitch_tokens = np.array(tokenizer.token_ids_of_type("Pitch", pitch_voc_idx))
             mask_pitch = np.full_like(tokens, 0, dtype=np.bool_)
             mask_pitch[:, pitch_voc_idx] = np.isin(
                 tokens[:, pitch_voc_idx], pitch_tokens
             )
```

### Comparing `miditok-2.1.0/miditok/midi_tokenizer.py` & `miditok-2.1.1/miditok/midi_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1021,17 +1021,15 @@
             iterator = []  # list of lists of one string (bytes)
             for file_path in tqdm(tokens_paths, desc="Loading token files"):
                 sample = self.load_tokens(file_path)
                 bytes_ = self._ids_to_bytes(
                     sample["ids"], as_one_str=True
                 )  # list of str (bytes)
                 iterator += (
-                    [[byte_] for byte_ in bytes_]
-                    if not self.unique_track
-                    else [[bytes_]]
+                    [[byte_] for byte_ in bytes_] if not self.unique_track else [bytes_]
                 )
 
             # This doesn't seem to work, the trainer pre-processes the sequences, but then no word remains
             """def it_gen():
                 for file_path_ in tqdm(tokens_paths, desc="Loading token files"):
                     sample_ = self.load_tokens(file_path_)
                     yield self._ids_to_bytes(sample_["ids"], as_one_str=True)
```

### Comparing `miditok-2.1.0/miditok/tokenizations/cp_word.py` & `miditok-2.1.1/miditok/tokenizations/cp_word.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,16 @@
         vocab[4] += [
             f'Duration_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
         # PROGRAM
         if self.config.use_programs:
             vocab += [
-                ["Ignore_None"] + [f"Program_{program}" for program in range(-1, 128)]
+                ["Ignore_None"]
+                + [f"Program_{program}" for program in self.config.programs]
             ]
 
         # CHORD
         if self.config.use_chords:
             vocab += [["Ignore_None"] + self._create_chords_tokens()]
 
         # REST
```

### Comparing `miditok-2.1.0/miditok/tokenizations/midi_like.py` & `miditok-2.1.1/miditok/tokenizations/midi_like.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 
         # TEMPO
         if self.config.use_tempos:
             vocab += [f"Tempo_{i}" for i in self.tempos]
 
         # PROGRAM
         if self.config.use_programs:
-            vocab += [f"Program_{program}" for program in range(-1, 128)]
+            vocab += [f"Program_{program}" for program in self.config.programs]
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
         NOTE: Program type is not referenced here, you can add it manually by
```

### Comparing `miditok-2.1.0/miditok/tokenizations/mmm.py` & `miditok-2.1.1/miditok/tokenizations/mmm.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/miditok/tokenizations/mumidi.py` & `miditok-2.1.1/miditok/tokenizations/mumidi.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/miditok/tokenizations/octuple.py` & `miditok-2.1.1/miditok/tokenizations/octuple.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 
         ticks_per_bar = time_division * time_sig[0]
         time_sig_changes = [TimeSignature(*time_sig, 0)]
 
         current_time_sig_tick = 0
         current_time_sig_bar = 0
 
-        tracks = dict([(n, []) for n in range(-1, 128)])
+        tracks = dict([(n, []) for n in self.config.programs])
         for time_step in tokens:
             if any(tok.split("_")[1] == "None" for tok in time_step[:6]):
                 continue  # Either padding, mask: error of prediction or end of sequence anyway
 
             # Note attributes
             pitch = int(time_step[0].split("_")[1])
             vel = int(time_step[1].split("_")[1])
```

### Comparing `miditok-2.1.0/miditok/tokenizations/octuple_mono.py` & `miditok-2.1.1/miditok/tokenizations/octuple_mono.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/miditok/tokenizations/remi.py` & `miditok-2.1.1/miditok/tokenizations/remi.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,15 @@
 
         # TEMPO
         if self.config.use_tempos:
             vocab += [f"Tempo_{i}" for i in self.tempos]
 
         # PROGRAM
         if self.config.use_programs:
-            vocab += [f"Program_{program}" for program in range(-1, 128)]
+            vocab += [f"Program_{program}" for program in self.config.programs]
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
         NOTE: Program type is not referenced here, you can add it manually by
```

### Comparing `miditok-2.1.0/miditok/tokenizations/remi_plus.py` & `miditok-2.1.1/miditok/tokenizations/remi_plus.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/miditok/tokenizations/structured.py` & `miditok-2.1.1/miditok/tokenizations/structured.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         vocab.append("TimeShift_0.0.1")  # for a time shift of 0
         vocab += [
             f'TimeShift_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
         # PROGRAM
         if self.config.use_programs:
-            vocab += [f"Program_{program}" for program in range(-1, 128)]
+            vocab += [f"Program_{program}" for program in self.config.programs]
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
         NOTE: Program type is not referenced here, you can add it manually by
```

### Comparing `miditok-2.1.0/miditok/tokenizations/tsd.py` & `miditok-2.1.1/miditok/tokenizations/tsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 
         # TEMPO
         if self.config.use_tempos:
             vocab += [f"Tempo_{i}" for i in self.tempos]
 
         # PROGRAM
         if self.config.use_programs:
-            vocab += [f"Program_{program}" for program in range(-1, 128)]
+            vocab += [f"Program_{program}" for program in self.config.programs]
 
         # TIME SIGNATURE
         if self.config.use_time_signatures:
             vocab += [f"TimeSig_{i[0]}/{i[1]}" for i in self.time_signatures]
 
         return vocab
```

### Comparing `miditok-2.1.0/miditok/utils/utils.py` & `miditok-2.1.1/miditok/utils/utils.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/miditok.egg-info/PKG-INFO` & `miditok-2.1.1/miditok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.1.0
+Version: 2.1.1
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `miditok-2.1.0/miditok.egg-info/SOURCES.txt` & `miditok-2.1.1/miditok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/setup.py` & `miditok-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="miditok",
     author="Nathan Fradet",
     url="https://github.com/Natooz/MidiTok",
     packages=find_packages(exclude=("tests",)),
-    version="2.1.0",
+    version="2.1.1",
     license="MIT",
     description="A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         "artificial intelligence",
         "deep learning",
```

### Comparing `miditok-2.1.0/tests/test_bpe.py` & `miditok-2.1.1/tests/test_bpe.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/tests/test_methods.py` & `miditok-2.1.1/tests/test_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,18 +210,22 @@
             if tokenizer.unique_track:
                 original_tokens, aug_tokens = [original_tokens], [aug_tokens]
             for original_track, aug_track, (_, is_drum) in zip(
                 original_tokens, aug_tokens, original_programs
             ):
                 if is_drum:
                     continue
-                for original_token, aug_token in zip(original_track, aug_track):
+                for idx, (original_token, aug_token) in enumerate(zip(original_track, aug_track)):
                     if not tokenizer.is_multi_voc:
                         if original_token in pitch_tokens:
-                            assert aug_token == original_token + offsets[0]
+                            pitch_offset = offsets[0]
+                            # no offset for drum pitches
+                            if tokenizer.unique_track and idx > 0 and tokenizer[original_track[idx - 1]] == "Program_-1":
+                                pitch_offset = 0
+                            assert aug_token == original_token + pitch_offset
                         elif original_token in vel_tokens:
                             assert aug_token in [
                                 original_token + offsets[1],
                                 tok_vel_min,
                                 tok_vel_max,
                             ]
                         elif (
```

### Comparing `miditok-2.1.0/tests/test_multitrack.py` & `miditok-2.1.1/tests/test_multitrack.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/tests/test_one_track.py` & `miditok-2.1.1/tests/test_one_track.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/tests/test_saving_loading_config.py` & `miditok-2.1.1/tests/test_saving_loading_config.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/tests/test_utils.py` & `miditok-2.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.0/tests/tests_utils.py` & `miditok-2.1.1/tests/tests_utils.py`

 * *Files identical despite different names*

