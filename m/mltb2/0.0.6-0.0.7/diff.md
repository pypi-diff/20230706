# Comparing `tmp/mltb2-0.0.6.tar.gz` & `tmp/mltb2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltb2-0.0.6.tar", last modified: Sun Jun 25 05:59:46 2023, max compression
+gzip compressed data, was "mltb2-0.0.7.tar", last modified: Thu Jul  6 20:19:41 2023, max compression
```

## Comparing `mltb2-0.0.6.tar` & `mltb2-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:46.000000 mltb2-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-25 05:59:34.000000 mltb2-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-25 05:59:34.000000 mltb2-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-25 05:59:46.000000 mltb2-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-25 05:59:34.000000 mltb2-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-25 05:59:34.000000 mltb2-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-25 05:59:46.000000 mltb2-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-25 05:59:34.000000 mltb2-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:46.000000 mltb2-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:19:41.479008 mltb2-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-06 20:19:31.000000 mltb2-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:19:31.000000 mltb2-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-06 20:19:41.479008 mltb2-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-06 20:19:31.000000 mltb2-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:19:41.475008 mltb2-0.0.7/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:19:41.475008 mltb2-0.0.7/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-06 20:19:31.000000 mltb2-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 20:19:41.479008 mltb2-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-06 20:19:31.000000 mltb2-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:19:41.479008 mltb2-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_transformers.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mltb2-0.0.6/LICENSE` & `mltb2-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/PKG-INFO` & `mltb2-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.6
+Version: 0.0.7
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
 Project-URL: Source Code, https://github.com/telekom/mltb2
 Keywords: optuna deep-learning ml ai machine-learning hyperparameter-optimization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: files
 Provides-Extra: fasttext
 Provides-Extra: optuna
 Provides-Extra: plot
 Provides-Extra: somajo
 Provides-Extra: transformers
```

### Comparing `mltb2-0.0.6/README.md` & `mltb2-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/mltb2/fasttext.py` & `mltb2-0.0.7/mltb2/fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/mltb2/files.py` & `mltb2-0.0.7/mltb2/files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/mltb2/optuna.py` & `mltb2-0.0.7/mltb2/optuna.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,28 +111,24 @@
         n_warmup_steps: Pruning is disabled until the trial reaches or exceeds the given number
             of steps.
     """
 
     def __init__(self, alpha: float = 0.1, n_warmup_steps: int = 4) -> None:
         # input value check
         if n_warmup_steps < 0:
-            raise ValueError(
-                "'n_warmup_steps' must not be negative! n_warmup_steps: {}".format(n_warmup_steps)
-            )
+            raise ValueError("'n_warmup_steps' must not be negative! n_warmup_steps: {}".format(n_warmup_steps))
         if alpha >= 1:
             raise ValueError("'alpha' must be smaller than 1! {}".format(alpha))
         if alpha <= 0:
             raise ValueError("'alpha' must be greater than 0! {}".format(alpha))
 
         self.n_warmup_steps = n_warmup_steps
         self.alpha = alpha
 
-    def prune(
-        self, study: optuna.study.Study, trial: optuna.trial.FrozenTrial
-    ) -> bool:  # noqa: D102
+    def prune(self, study: optuna.study.Study, trial: optuna.trial.FrozenTrial) -> bool:  # noqa: D102
         # get best tial - best trial is not available for first trial
         best_trial = None
         try:
             best_trial = study.best_trial
         except ValueError:
             pass
 
@@ -148,31 +144,29 @@
                 best_trial_intermediate_values = list(best_trial.intermediate_values.values())
                 best_trial_mean = np.mean(best_trial_intermediate_values)
 
                 _logger.debug("trial_mean: %s", trial_mean)
                 _logger.debug("best_trial_intermediate_values: %s", best_trial_intermediate_values)
                 _logger.debug("best_trial_mean: %s", best_trial_mean)
 
-                if (
-                    trial_mean < best_trial_mean and study.direction == StudyDirection.MAXIMIZE
-                ) or (trial_mean > best_trial_mean and study.direction == StudyDirection.MINIMIZE):
+                if (trial_mean < best_trial_mean and study.direction == StudyDirection.MAXIMIZE) or (
+                    trial_mean > best_trial_mean and study.direction == StudyDirection.MINIMIZE
+                ):
                     pvalue = stats.ttest_ind(
                         trial_intermediate_values,
                         best_trial_intermediate_values,
                     ).pvalue
 
                     _logger.debug("pvalue: %s", pvalue)
 
                     if pvalue < self.alpha:
                         _logger.info("We prune this trial. pvalue: %s", pvalue)
 
                         return True
 
                 else:
-                    _logger.debug(
-                        "This trial is better than best trial - we do not check for pruning."
-                    )
+                    _logger.debug("This trial is better than best trial - we do not check for pruning.")
 
             else:
                 _logger.debug("This trial did not reach n_warmup_steps - we do no checks.")
 
         return False
```

### Comparing `mltb2-0.0.6/mltb2/plot.py` & `mltb2-0.0.7/mltb2/plot.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/mltb2/somajo.py` & `mltb2-0.0.7/mltb2/somajo.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,107 +6,136 @@
 
 This module is based on `SoMaJo <https://github.com/tsproisl/SoMaJo>`_.
 Use pip to install the necessary dependencies for this module:
 ``pip install mltb2[somajo]``
 """
 
 
+from abc import ABC
 from dataclasses import dataclass, field
-from typing import List, Set
+from typing import Container, Iterable, List, Optional, Set
 
 from somajo import SoMaJo
 from tqdm import tqdm
 
 
 @dataclass
-class SoMaJoSentenceSplitter:
-    """Use SoMaJo to split text into sentences.
+class SoMaJoBaseClass(ABC):
+    """Base Class for SoMaJo tools.
 
     Args:
         language: The language. ``de_CMC`` for German or ``en_PTB`` for English.
-        show_progress_bar: Show a progressbar during processing.
+
+    Note:
+        This class is an abstract base class. It should not be used directly.
     """
 
     language: str
     somajo: SoMaJo = field(init=False, repr=False)
-    show_progress_bar: bool = False
 
     def __post_init__(self):
         """Do post init."""
         self.somajo = SoMaJo(self.language)
 
-    # see https://github.com/tsproisl/SoMaJo/issues/17
-    @staticmethod
-    def detokenize(tokens) -> str:
-        """Convert SoMaJo tokens to sentence (string).
 
-        Args:
-            tokens: The tokens to be de-tokenized.
-        Returns:
-            The de-tokenized sentence.
-        """
-        result_list = []
-        for token in tokens:
-            if token.original_spelling is not None:
-                result_list.append(token.original_spelling)
-            else:
-                result_list.append(token.text)
-
-            if token.space_after:
-                result_list.append(" ")
-        result = "".join(result_list)
-        result = result.strip()
-        return result
+def detokenize(tokens) -> str:
+    """Convert SoMaJo tokens to sentence (string).
+
+    Args:
+        tokens: The tokens to be de-tokenized.
+    Returns:
+        The de-tokenized sentence.
+
+    See Also:
+        `How do I split sentences but not words? <https://github.com/tsproisl/SoMaJo/issues/17>`_
+    """
+    result_list = []
+    for token in tokens:
+        if token.original_spelling is not None:
+            result_list.append(token.original_spelling)
+        else:
+            result_list.append(token.text)
+
+        if token.space_after:
+            result_list.append(" ")
+    result = "".join(result_list)
+    result = result.strip()
+    return result
+
+
+def extract_token_class_set(sentences: Iterable, keep_token_classes: Optional[Container[str]] = None) -> Set[str]:
+    """Extract token from sentences by token class.
+
+    Args:
+        sentences: The sentences from which to extract.
+        keep_token_classes: The token classes to keep. If ``None`` all will be kept.
+    Returns:
+        The set of extracted token texts.
+    """
+    result = set()
+    for sentence in sentences:
+        for token in sentence:
+            if keep_token_classes is None:
+                result.add(token.text)
+            elif token.token_class in keep_token_classes:
+                result.add(token.text)
+            # else ignore
+    return result
+
+
+@dataclass
+class SoMaJoSentenceSplitter(SoMaJoBaseClass):
+    """Use SoMaJo to split text into sentences.
+
+    Args:
+        language: The language. ``de_CMC`` for German or ``en_PTB`` for English.
+        show_progress_bar: Show a progressbar during processing.
+    """
+
+    show_progress_bar: bool = False
 
     def __call__(self, text: str) -> List[str]:
         """Split the text into a list of sentences.
 
         Args:
             text: The text to be split.
         Returns:
             The list of sentence splits.
         """
         sentences = self.somajo.tokenize_text([text])
 
         result = []
 
         for sentence in tqdm(sentences, disable=not self.show_progress_bar):
-            sentence_string = self.detokenize(sentence)
+            sentence_string = detokenize(sentence)
             result.append(sentence_string)
 
         return result
 
 
 @dataclass
-class JaccardSimilarity:
+class JaccardSimilarity(SoMaJoBaseClass):
     """Calculate the `jaccard similarity <https://en.wikipedia.org/wiki/Jaccard_index>`_.
 
     Args:
         language: The language. ``de_CMC`` for German or ``en_PTB`` for English.
     """
 
-    language: str
-    somajo: SoMaJo = field(init=False, repr=False)
-
-    def __post_init__(self):
-        """Do post init."""
-        self.somajo = SoMaJo(self.language)
-
     def get_token_set(self, text: str) -> Set[str]:
         """Get token set for text.
 
         Args:
             text: The text to be tokenized into a set.
         Returns:
             The set of tokens (words).
         """
         sentences = self.somajo.tokenize_text([text])
-        tokens = [t.text.lower() for sentence in sentences for t in sentence]
-        # TODO: add option to filter tokens
-        token_set = set(tokens)
+        token_set = extract_token_class_set(sentences)  # TODO: filter tokens
+        token_set = {t.lower() for t in token_set}
+
         return token_set
 
     def __call__(self, text1: str, text2: str) -> float:
         """Calculate the jaccard similarity for two texts.
 
         Args:
             text1: Text one.
@@ -116,7 +145,28 @@
         """
         token_set1 = self.get_token_set(text1)
         token_set2 = self.get_token_set(text2)
         intersection = token_set1.intersection(token_set2)
         union = token_set1.union(token_set2)
         jaccard_similarity = float(len(intersection)) / len(union)
         return jaccard_similarity
+
+
+@dataclass
+class TokenExtractor(SoMaJoBaseClass):
+    """Extract tokens from text.
+
+    Args:
+        language: The language. ``de_CMC`` for German or ``en_PTB`` for English.
+    """
+
+    def extract_url_set(self, text: str) -> Set[str]:
+        """Extract URLs from text.
+
+        Args:
+            text: the text
+        Returns:
+            Set of extracted links.
+        """
+        sentences = self.somajo.tokenize_text([text])
+        result = extract_token_class_set(sentences, keep_token_classes="URL")
+        return result
```

### Comparing `mltb2-0.0.6/mltb2/somajo_transformers.py` & `mltb2-0.0.7/mltb2/somajo_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,15 @@
         counts = self.transformers_token_counter(sentences)
 
         assert len(sentences) == len(counts)  # type: ignore
 
         result_splits: List[str] = []
         current_sentences: List[str] = []
         current_count: int = 0
-        for sentence, count in zip(
-            tqdm(sentences, disable=not self.show_progress_bar), counts  # type: ignore
-        ):
+        for sentence, count in zip(tqdm(sentences, disable=not self.show_progress_bar), counts):  # type: ignore
             if count > self.max_token:
                 if self.ignore_overly_long_sentences:
                     continue
                 else:
                     raise ValueError("No sentence may be longer than 'max_token'.")
             if current_count + count <= self.max_token:
                 current_count += count
```

### Comparing `mltb2-0.0.6/mltb2/transformers.py` & `mltb2-0.0.7/mltb2/transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/mltb2.egg-info/PKG-INFO` & `mltb2-0.0.7/mltb2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.6
+Version: 0.0.7
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
 Project-URL: Source Code, https://github.com/telekom/mltb2
 Keywords: optuna deep-learning ml ai machine-learning hyperparameter-optimization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: files
 Provides-Extra: fasttext
 Provides-Extra: optuna
 Provides-Extra: plot
 Provides-Extra: somajo
 Provides-Extra: transformers
```

### Comparing `mltb2-0.0.6/mltb2.egg-info/SOURCES.txt` & `mltb2-0.0.7/mltb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/pyproject.toml` & `mltb2-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.black]
-line-length = 99
-target-version = ["py37"]
+line-length = 119
+target-version = ["py38"]
 
 [tool.isort]
 profile = "black"
 lines_after_imports = 2
-line_length = 99
+line_length = 119
 
 [tool.pylint."MASTER"]
 load-plugins = "pylintfileheader"
 file-header = "(# Copyright \\(c\\) \\d{4} .*\\n)*# This software is distributed under the terms of the MIT license\\n# which is available at https://opensource.org/licenses/MIT\\n\\n"
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
```

### Comparing `mltb2-0.0.6/setup.py` & `mltb2-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,15 @@
         "pylintfileheader",
     ],
     "testing": ["pytest", "packaging"],
     "doc": ["sphinx", "sphinx_rtd_theme", "sphinx_copybutton"],
 }
 
 # add "all"
-extras_require["all"] = {
-    package_name for value in extras_require.values() for package_name in value
-}
+extras_require["all"] = {package_name for value in extras_require.values() for package_name in value}
 
 
 def get_version():
     """Read version from ``__init__.py``."""
     version_filepath = os.path.join(os.path.dirname(__file__), project_name, "__init__.py")
     with open(version_filepath) as f:
         for line in f:
@@ -86,28 +84,27 @@
         "Bug Tracker": source_code + "/issues",
         "Documentation": "https://telekom.github.io/mltb2/",
         "Source Code": source_code,
         # "Contributing": source_code + "/blob/main/CONTRIBUTING.md",
         # "Code of Conduct": source_code + "/blob/main/CODE_OF_CONDUCT.md",
     },
     packages=setuptools.find_packages(),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=install_requires,
     extras_require=extras_require,
     keywords=keywords,
     classifiers=[
         "Development Status :: 3 - Alpha",
         # "Development Status :: 4 - Beta",
         # "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         # "Intended Audience :: Education",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Mathematics",
```

### Comparing `mltb2-0.0.6/tests/test_fasttext.py` & `mltb2-0.0.7/tests/test_fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/tests/test_files.py` & `mltb2-0.0.7/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/tests/test_optuna.py` & `mltb2-0.0.7/tests/test_optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/tests/test_somajo_transformers.py` & `mltb2-0.0.7/tests/test_somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.6/tests/test_transformers.py` & `mltb2-0.0.7/tests/test_transformers.py`

 * *Files identical despite different names*

