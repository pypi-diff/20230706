# Comparing `tmp/bioviper-0.1.2.tar.gz` & `tmp/bioviper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioviper-0.1.2.tar", last modified: Tue Aug  2 13:23:57 2022, max compression
+gzip compressed data, was "bioviper-0.2.0.tar", last modified: Thu Jul  6 01:16:10 2023, max compression
```

## Comparing `bioviper-0.1.2.tar` & `bioviper-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sam        (504) staff       (20)        0 2022-08-02 13:23:57.530356 bioviper-0.1.2/
--rw-r--r--   0 sam        (504) staff       (20)     1066 2022-01-23 14:04:12.000000 bioviper-0.1.2/LICENSE
--rw-r--r--   0 sam        (504) staff       (20)     7737 2022-08-02 13:23:57.530193 bioviper-0.1.2/PKG-INFO
--rw-r--r--   0 sam        (504) staff       (20)     5942 2022-07-27 22:26:41.000000 bioviper-0.1.2/README.md
-drwxr-xr-x   0 sam        (504) staff       (20)        0 2022-08-02 13:23:57.523450 bioviper-0.1.2/bioviper/
--rw-r--r--   0 sam        (504) staff       (20)      318 2022-08-02 13:23:23.000000 bioviper-0.1.2/bioviper/__init__.py
--rw-r--r--   0 sam        (504) staff       (20)     3251 2022-04-05 15:36:59.000000 bioviper-0.1.2/bioviper/hmmer_tools.py
--rw-r--r--   0 sam        (504) staff       (20)    37426 2022-08-02 13:19:25.000000 bioviper-0.1.2/bioviper/msa.py
--rw-r--r--   0 sam        (504) staff       (20)     8056 2022-08-02 13:04:54.000000 bioviper-0.1.2/bioviper/pdb.py
--rw-r--r--   0 sam        (504) staff       (20)     7444 2022-03-13 02:05:19.000000 bioviper-0.1.2/bioviper/phylo.py
-drwxr-xr-x   0 sam        (504) staff       (20)        0 2022-08-02 13:23:57.529944 bioviper-0.1.2/bioviper.egg-info/
--rw-r--r--   0 sam        (504) staff       (20)     7737 2022-08-02 13:23:57.000000 bioviper-0.1.2/bioviper.egg-info/PKG-INFO
--rw-r--r--   0 sam        (504) staff       (20)      264 2022-08-02 13:23:57.000000 bioviper-0.1.2/bioviper.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (504) staff       (20)        1 2022-08-02 13:23:57.000000 bioviper-0.1.2/bioviper.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (504) staff       (20)        9 2022-08-02 13:23:57.000000 bioviper-0.1.2/bioviper.egg-info/top_level.txt
--rw-r--r--   0 sam        (504) staff       (20)      776 2022-08-02 13:23:35.000000 bioviper-0.1.2/pyproject.toml
--rw-r--r--   0 sam        (504) staff       (20)       38 2022-08-02 13:23:57.530416 bioviper-0.1.2/setup.cfg
--rw-r--r--   0 sam        (504) staff       (20)      360 2022-08-02 13:23:28.000000 bioviper-0.1.2/setup.py
+drwxr-xr-x   0 sam        (504) staff       (20)        0 2023-07-06 01:16:10.120206 bioviper-0.2.0/
+-rw-r--r--   0 sam        (504) staff       (20)     1066 2022-01-23 14:04:12.000000 bioviper-0.2.0/LICENSE
+-rw-r--r--   0 sam        (504) staff       (20)     7556 2023-07-06 01:16:10.120043 bioviper-0.2.0/PKG-INFO
+-rw-r--r--   0 sam        (504) staff       (20)     5761 2022-08-29 15:33:39.000000 bioviper-0.2.0/README.md
+drwxr-xr-x   0 sam        (504) staff       (20)        0 2023-07-06 01:16:10.115079 bioviper-0.2.0/bioviper/
+-rw-r--r--   0 sam        (504) staff       (20)      318 2022-08-02 14:33:15.000000 bioviper-0.2.0/bioviper/__init__.py
+-rw-r--r--   0 sam        (504) staff       (20)     3251 2022-08-02 14:44:01.000000 bioviper-0.2.0/bioviper/hmmer_tools.py
+-rw-r--r--   0 sam        (504) staff       (20)    39448 2023-07-05 22:15:43.000000 bioviper-0.2.0/bioviper/msa.py
+-rw-r--r--   0 sam        (504) staff       (20)    13678 2023-03-09 21:38:54.000000 bioviper-0.2.0/bioviper/pdb.py
+-rw-r--r--   0 sam        (504) staff       (20)    23855 2023-05-24 14:04:29.000000 bioviper-0.2.0/bioviper/phylo.py
+drwxr-xr-x   0 sam        (504) staff       (20)        0 2023-07-06 01:16:10.119818 bioviper-0.2.0/bioviper.egg-info/
+-rw-r--r--   0 sam        (504) staff       (20)     7556 2023-07-06 01:16:10.000000 bioviper-0.2.0/bioviper.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (504) staff       (20)      264 2023-07-06 01:16:10.000000 bioviper-0.2.0/bioviper.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (504) staff       (20)        1 2023-07-06 01:16:10.000000 bioviper-0.2.0/bioviper.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (504) staff       (20)        9 2023-07-06 01:16:10.000000 bioviper-0.2.0/bioviper.egg-info/top_level.txt
+-rw-r--r--   0 sam        (504) staff       (20)      776 2023-07-05 22:28:14.000000 bioviper-0.2.0/pyproject.toml
+-rw-r--r--   0 sam        (504) staff       (20)       38 2023-07-06 01:16:10.120255 bioviper-0.2.0/setup.cfg
+-rw-r--r--   0 sam        (504) staff       (20)      360 2023-07-05 22:27:04.000000 bioviper-0.2.0/setup.py
```

### Comparing `bioviper-0.1.2/LICENSE` & `bioviper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioviper-0.1.2/PKG-INFO` & `bioviper-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioviper
-Version: 0.1.2
+Version: 0.2.0
 Summary: Enhancements to Biopython for working with biological data
 Author: Sam Berry
 Author-email: Sam Berry <sberry@g.harvard.edu>
 License: MIT License
         
         Copyright (c) 2022 Sam Berry
         
@@ -43,27 +43,21 @@
 
 The core of this code is a set of three new classes: a MultipleSequenceAlignment class, a SequenceArray class (for unaligned sequences) and a ProteinStructure class.
 
 I am working on a set of Jupyter notebooks that should explain the basic usage of these objects.
 
 ## Installation
 
-On Mac/Linux, I would recommend cloning or downloading this repository and then installing it into a conda environment. You can create a conda environment, let's called it "evo," assuming you have conda installed with:
+bioviper is now on PyPI and can be installed with pip or conda install. However, for the last development version which may have some bugs fixed or new funcitonality being tested, I recommend using
 
 ```
-conda create -n evo pip numpy pandas Biopython
+pip install git+https://github.com/samberry19/bioviper/
 ```
 
-Then navigate to the folder alignment_tools and type:
-
-```
-conda install .
-```
-
-I have no idea how to do this on Windows, but let me know if you install it and how and I can add it here :)
+for the time being.
 
 ## Basics
 
 To load an alignment from a file:
 
 ```
 msa = readAlignment("alignment.fa", format="fasta")
```

### Comparing `bioviper-0.1.2/README.md` & `bioviper-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,27 +6,21 @@
 
 The core of this code is a set of three new classes: a MultipleSequenceAlignment class, a SequenceArray class (for unaligned sequences) and a ProteinStructure class.
 
 I am working on a set of Jupyter notebooks that should explain the basic usage of these objects.
 
 ## Installation
 
-On Mac/Linux, I would recommend cloning or downloading this repository and then installing it into a conda environment. You can create a conda environment, let's called it "evo," assuming you have conda installed with:
+bioviper is now on PyPI and can be installed with pip or conda install. However, for the last development version which may have some bugs fixed or new funcitonality being tested, I recommend using
 
 ```
-conda create -n evo pip numpy pandas Biopython
+pip install git+https://github.com/samberry19/bioviper/
 ```
 
-Then navigate to the folder alignment_tools and type:
-
-```
-conda install .
-```
-
-I have no idea how to do this on Windows, but let me know if you install it and how and I can add it here :)
+for the time being.
 
 ## Basics
 
 To load an alignment from a file:
 
 ```
 msa = readAlignment("alignment.fa", format="fasta")
```

### Comparing `bioviper-0.1.2/bioviper/hmmer_tools.py` & `bioviper-0.2.0/bioviper/hmmer_tools.py`

 * *Files identical despite different names*

### Comparing `bioviper-0.1.2/bioviper/msa.py` & `bioviper-0.2.0/bioviper/msa.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,32 @@
 from Bio.Align import _aligners
 from Bio.Align import substitution_matrices
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord,_RestrictedDict
 from Bio.Align import MultipleSeqAlignment
 
 from .pdb import readPDB
+from .phylo import readTree, Tree
 
 # Otherwise we get some annoying pandas warnings
 import warnings
 warnings.simplefilter("ignore", UserWarning)
 
 from copy import copy,deepcopy
 
 alphabet = '-ACDEFGHIKLMNPQRSTVWY'
 
 def readAlignment(alignment_file, format="fasta", calc_frequencies=False):
 
+    '''
+    Read in an alignment in a format accepted by biopython. Arguments:
+        -alignment_file: the path to the alignment you want to load
+        -format: 
+    '''
+
     msa = MultipleSequenceAlignment(AlignIO.read(alignment_file, format=format))
 
     if calc_frequencies==True:
         msa.calc_frequencies()
         msa.calc_coverage()
 
     return msa
@@ -105,15 +112,18 @@
 
         # Annotations about each column of the alignment
         if column_annotations is None:
             column_annotations = {}
         # Handle this via the property set function which will validate it
         self.column_annotations = column_annotations
 
+        #Useful for indexing
         self.N, self.L = self.matrix.shape
+        id_to_index = pd.DataFrame(zip(self.ids, np.arange(self.N)), columns=("id", "index")).set_index("id")
+        self.id_to_index = id_to_index
 
         self.coverage = None
         self.frequencies = None
         self.tree = None
         self.numeric_matrix = None
         self.fij = None
         self._pseudocount = 0
@@ -149,15 +159,15 @@
 
         ds = []
 
         for rec in self._records:
             s = Seq(str(rec.seq).replace('-','').replace('.','').upper())
             ds.append(SeqRecord(s, id = rec.id, name=rec.name, description=rec.description))
 
-        return ds
+        return SequenceArray(ds)
 
 
     def sequence_lengths(self):
 
         W = (self.matrix!='-')&(self.matrix!='.')
         return np.sum(W,axis=1)
 
@@ -187,14 +197,15 @@
 
         frequencies = pd.DataFrame(frequencies, columns=list(alphabet))
 
         frequencies.sequence_weights = self.sequence_weights
 
         if type(pos_indices) != type(None):
             frequencies.index = pos_indices
+            
         elif first_pos != 0:
             frequencies.index = np.arange(first_index, self.L + first_index)
 
         if store:
             self.frequencies = frequencies
 
         return frequencies
@@ -217,19 +228,20 @@
         if numeric:
             df = pd.DataFrame.from_records(self.as_numeric(), index=self.ids)
         else:
             df = pd.DataFrame.from_records(self.matrix, index=self.ids)
 
         return df
 
-    def one_hot_encoding(self):
+    def one_hot_encode(self, dim=1):
 
-        '''Generate a one-hot encoded pandas dataframe, e.g. for dimensionality reduction.'''
+        '''Generate a one-hot encoded pandas dataframe, e.g. for dimensionality reduction. If dim=1, will be N x L*20, if dim=2, will be N x L x 20'''
+
+        return np.array([one_hot_encode(seq, dim=dim) for seq in self.as_numeric()])
 
-        return pd.get_dummies(self.upper().as_df())
 
     def calc_pair_frequencies(self, pseudocount=0):
 
         if type(self.numeric_matrix) == type(None):
             self.as_numeric()
 
         X = [[[] for i in range(self.L)] for i in range(self.L)]
@@ -353,15 +365,15 @@
     def set_ids(self, ids):
 
         """Reset all IDs in place to a new list. Will both change self.ids and the .id attribute
            of each individual sequence record."""
 
         if len(ids) == self.N:
             self.ids = ids
-            for n,record in enumerate(self._records):
+            for n,seq in enumerate(self._records):
                 seq.id = ids[n]
         else:
             raise ValueError('ERROR: cannot use id list of length', len(ids), 'for an alignment with', self.N, 'sequences')
 
 
     def modify_ids(melf, func):
 
@@ -372,47 +384,72 @@
 
         for seq in self._records:
             seq.id = func(seq.id)
             ids.append(seq.id)
 
         self.ids = np.array(ids)
 
+    def pos_covariance(self):
+
+        '''Get the 4D position by position covariance matrix, considering one-hot encoded sequences'''
+
+        return np.cov(self.one_hot_encoding(full=True).T).reshape((sampler.alignment.L, sampler.alignment.L, 21, 21))
+
+    def seq_covariance(self):
+
+        '''Get the covariance matrix across sequences'''
+
+        return np.cov(np.array(self.one_hot_encoding()))
 
     def __getitem__(self, index):
         """Access part of the alignment. Indexes like a 2D numpy array and returns
         another MultipleSequenceAlignment object unless:
             1) you ask for a single row, when you get a SeqRecord object
             2) you ask for a single column, when you get a numpy array
             3) you ask for a single row AND a single column, when you get a single letter as a string."""
 
         if isinstance(index, int):
             return self._records[index]
 
         elif isinstance(index, slice):
-            return self.__getitem__(np.arange(self.L)[index])
+            return self.__getitem__(np.arange(self.N)[index])
 
+        # if you pass an array as the index
         elif isinstance(index, np.ndarray):
-            ids = self.ids[index]; names = self.names[index]
-            descs = list(np.array(self.descriptions)[index])
 
-            if type(self.tree) != type(None):
+            # if the first item is an integer, float or boolean
+            if isinstance(index[0], (int, np.int64, float, np.float64, bool, np.bool_)):
 
-                if type(index[0])==np.bool_:
-                    branches = [self._records[k] for k in np.where(index)[0]]
-                else:
-                    branches = [self._records[k] for k in index]
+                ids = self.ids[index]; names = self.names[index]
+                descs = list(np.array(self.descriptions)[index])
+
+                # taking the appropriate branches of the tree if you have an attached tree
+                if type(self.tree) != type(None):
 
-                new_msa = MultipleSequenceAlignment(self.matrix[index], ids=ids,
-                    names=names, descriptions=descs,_tree_branches=branches)
-                new_msa.tree = self.tree
+                    if type(index[0])==np.bool_:
+                        branches = [self._records[k] for k in np.where(index)[0]]
+                    else:
+                        branches = [self._records[k] for k in index]
 
-                return new_msa
+                    new_msa = MultipleSequenceAlignment(self.matrix[index], ids=ids,
+                        names=names, descriptions=descs,_tree_branches=branches)
+                    new_msa.tree = self.tree
+
+                    return new_msa
 
+                else:
+                    return MultipleSequenceAlignment(self.matrix[index], ids=ids, names=names, descriptions=descs)
+
+            # if they're not floats/integers/boolean 
             else:
-                return MultipleSequenceAlignment(self.matrix[index], ids=ids, names=names, descriptions=descs)
+
+                return self.__getitem__(np.array(self.id_to_index.loc[index]["index"]))
+
+        elif isinstance(index, list):
+            return self.__getitem__(np.array(id))
 
         elif isinstance(index, str):
             return self.__getitem__(np.where(self.ids==index)[0])[0]
 
         elif len(index) != 2:
              raise TypeError("Invalid index type.")
 
@@ -537,66 +574,76 @@
 
     def attach_tree(self, tree, format='newick', prune_unmatched=False):
 
         """Attach a precalculated tree to the alignment. See documentation for how usage.
             As of now, IDs in the tree must exactly match IDs in the alignment."""
 
         if type(tree)==str:
-            tree = Phylo.read(tree, format)
+            tree = readTree(tree, format)
+
+        if isinstance(tree, (Phylo.Newick.Tree, Phylo.PhyloXML.Phylogeny)):
+            tree = Tree(tree)
 
         self.tree = deepcopy(tree)
 
-        for term in self.tree.get_terminals():
+        for leaf in self.tree.leaves:
+
             try:
-                n = list(self.ids).index(term.name)
+                n = list(self.ids).index(leaf.name)
+
             except:
-                ns = [n for n,i in enumerate(self.ids) if term.name in i]
+
+                ns = [n for n,i in enumerate(self.ids) if leaf.name in i]
                 if len(ns) == 0:
-                    print("Terminal name", term.name, "not in alignment - will not be attached!")
+                    print("Terminal name", leaf.name, "not in alignment - will not be attached!")
                     n = -1
+
                 elif len(ns) == 1:
                     n = n[0]
+
                 else:
-                    print("Ambiguity with terminal time", term.name, "in alignment", len(ns), "times!")
+                    print("Ambiguity with terminal time", leaf.name, "in alignment", len(ns), "times!")
                     n = -1
 
             if n > -1:
-                self._records[n].branch = term
-                term.seq = self._records[n].seq
-                term.nseq = n
+                self._records[n].branch = leaf
+                leaf.seq = self._records[n].seq
+                leaf.nseq = n
+
             elif prune_unmatched:
-                self.tree.prune(term)
+                self.tree.prune(leaf)
 
     def set_sequence_weights(self, weights):
 
         self.sequence_weights = np.array(weights)
         for n,record in enumerate(self._records):
             record.weight = weights[n]
 
     def get_index(self, id):
 
         """Return the index of a particular sequence id. Should work for partial IDs;
             for indices that appear multiple times it will return an array, and for missing
             indices it will return None."""
 
 
-        if id in self.ids:
-            return list(self.ids).index(id)
+        try:
+            # pandas indexing here is by far the fastest way to do this
+            return self.id_to_index.loc[id].iloc[0]
 
-        else:
+        except:
 
             a = self.search_id(id)
             if type(a)==type(None):
                 return None
 
             elif type(a) == SeqRecord:
                 return self.get_index(a.id)
 
             else:
-                return array([self.get_index(seq.id) for seq in a])
+                return np.array([self.get_index(seq.id) for seq in a])
 
     def fix_tree(self):
 
         """This updates the current attached tree to (1) make sure that the number matching is correct
         and (2) remove any nodes that are not present in the alignment.
 
         Technically, it makes a copy of the original tree and re-attaches it before modifying.
@@ -611,40 +658,22 @@
             branches = [record.branch for record in self._records]
 
             for term in self.tree.get_terminals():
                 if tree not in branches:
                     self.tree.prune(branch)
 
 
-    def subset_by_ids(self, ids, sort=True):
-
-        if sort:
+    def subset_by_ids(self, ids, sort=False, match_order=True):
 
-            '''Sort both lists and search - orders of magnitude faster for
-                    very large alignments.'''
-
-            sorted_ali = self.__getitem__(np.argsort(self.ids))
-            ids_sorted = sorted_ali.ids
-
-            # If some ids in the id list aren't in self.ids, we'll ignore them
-            common_ids = np.intersect1d(ids, ids_sorted)
-            x = [] # Initialize a list
-            n = 0  # Iterator as we work our way through self.ids
-
-            for idx in common_ids:  # Iterate through the common ids
-                                      # each will fall in order in the sorted list
-                while (ids_sorted[n] != idx) & (n<(self.N-1)):
-                    n+=1
-                x.append(n)
+        """
+        Subset the MSA using a set of IDs. Used to be implemented in a way that turned out to be much slower, with two
+        deprecated arugments (sort & match_order); I've kept them defined by default here just for backwards compatibility
+        """
 
-            return sorted_ali[np.array(x)]
-
-        else:
-            # The simple way, preserving order, but very slow for large alignments
-            return self.__getitem__(np.isin(self.ids, ids))
+        return self.__getitem__(np.array(self.id_to_index.loc[ids]["index"]))
 
 
     def subset_by_clade(self, clade):
 
         """For a clade in the attached tree, subset the alignment to get only those sequences."""
 
         try:
@@ -768,35 +797,43 @@
         except:
             self.structures = [(nseq, structure)]
 
 def readSequences(filename, format="Detect"):
 
     if format=='Detect':
         ending = filename.split('.')[-1]
-        if 'fa' in ending:
+        if 'fastq' in ending:
+            format="fastq"
+        elif 'fa' in ending:
             format="fasta"
         elif 'sto' in ending:
             format = "stockholm"
         elif 'nex' in ending:
             format = "nexus"
         elif "a2m" in ending:
             format = "fasta"
 
-    return SequenceArray(list(SeqIO.parse(filename, format)))
+    return SequenceArray(list(SeqIO.parse(filename, format)), fmt=format)
 
 class SequenceArray:
 
-    def __init__(self, records):
+    def __init__(self, records, fmt="fasta"):
 
         self._records = records
         self.ids = np.array([record.id for record in self._records])
         self.names = np.array([record.id for record in self._records])
         self.descriptions = [record.id for record in self._records]
         self.N = len(self._records)
         self.L = np.array([len(rec.seq) for rec in self._records])
+        self.format = fmt
+
+        # For fastq sequencing reads with phred quality scores, save those phred quality scores in a centralized place
+        if fmt == "fastq":
+            self.phred_quality = [np.array(rec.letter_annotations["phred_quality"]) for rec in self._records]
+            self.mean_phred_quality = np.array([np.mean(qual_arr) for qual_arr in self.phred_quality])
 
     def __len__(self):
         return self.N
 
     def __getitem__(self, index):
 
         if isinstance(index, int):
@@ -954,15 +991,15 @@
                 elif "sto" in ending:
                     format = "stockholm"
                 elif "clust" in ending:
                     format = "clustal"
             except:
                 return TypeError("Please pass a format or a filename with an ending containing fa, sto or clust")
 
-        SeqIO.write(MultipleSeqAlignment(self._records), filename, format)
+        SeqIO.write(self._records, filename, format)
 
 
 def PairwiseAlign(sequence1, sequence2, alignment_method, alignment_params):
 
     '''
     Pairwise alignment of two sequences using simple alignment tools from pairwise2.align. A standalone function
     to make it easier to incorporate choices of different methods or parameters into a more complex workflow
@@ -1061,7 +1098,29 @@
                 use_pos = msa._coverage_mask[n] & msa._coverage_mask[nseq]
 
                 ids.append(np.mean(seq[use_pos]==msa.matrix[n][use_pos]))
 
             IM.append(ids)
 
     return np.array(IM)
+
+
+def one_hot_encode(seq_num, dim=1):
+
+    '''
+    One-hot encode a numerically-encoded amino acid sequence. Faster than training a one-hot encoder
+    and using .transform()
+    '''
+
+    L = len(seq_num)
+
+    # Initialize an array of all zeros of the correct shape
+    x = np.zeros((L,21))
+
+    # Assign the appropriate positions to be ones
+    x[np.arange(L), seq_num] = 1
+
+    # Make one-dimensional if dim=1
+    if dim==1:
+        return x.reshape((L*21))
+    elif dim==2:
+        return x
```

### Comparing `bioviper-0.1.2/bioviper.egg-info/PKG-INFO` & `bioviper-0.2.0/bioviper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioviper
-Version: 0.1.2
+Version: 0.2.0
 Summary: Enhancements to Biopython for working with biological data
 Author: Sam Berry
 Author-email: Sam Berry <sberry@g.harvard.edu>
 License: MIT License
         
         Copyright (c) 2022 Sam Berry
         
@@ -43,27 +43,21 @@
 
 The core of this code is a set of three new classes: a MultipleSequenceAlignment class, a SequenceArray class (for unaligned sequences) and a ProteinStructure class.
 
 I am working on a set of Jupyter notebooks that should explain the basic usage of these objects.
 
 ## Installation
 
-On Mac/Linux, I would recommend cloning or downloading this repository and then installing it into a conda environment. You can create a conda environment, let's called it "evo," assuming you have conda installed with:
+bioviper is now on PyPI and can be installed with pip or conda install. However, for the last development version which may have some bugs fixed or new funcitonality being tested, I recommend using
 
 ```
-conda create -n evo pip numpy pandas Biopython
+pip install git+https://github.com/samberry19/bioviper/
 ```
 
-Then navigate to the folder alignment_tools and type:
-
-```
-conda install .
-```
-
-I have no idea how to do this on Windows, but let me know if you install it and how and I can add it here :)
+for the time being.
 
 ## Basics
 
 To load an alignment from a file:
 
 ```
 msa = readAlignment("alignment.fa", format="fasta")
```

### Comparing `bioviper-0.1.2/pyproject.toml` & `bioviper-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bioviper"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Sam Berry", email="sberry@g.harvard.edu" },
 ]
 description = "Enhancements to Biopython for working with biological data"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

