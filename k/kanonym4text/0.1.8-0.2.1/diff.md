# Comparing `tmp/kanonym4text-0.1.8.tar.gz` & `tmp/kanonym4text-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanonym4text-0.1.8.tar", last modified: Wed Jul  5 07:39:54 2023, max compression
+gzip compressed data, was "kanonym4text-0.2.1.tar", last modified: Thu Jul  6 10:22:52 2023, max compression
```

## Comparing `kanonym4text-0.1.8.tar` & `kanonym4text-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,26 @@
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-05 07:39:54.758819 kanonym4text-0.1.8/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-05 07:39:54.758819 kanonym4text-0.1.8/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     5099 2023-07-01 20:45:19.000000 kanonym4text-0.1.8/README.md
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-05 07:39:54.758819 kanonym4text-0.1.8/kanonym4text/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       54 2023-07-01 20:45:19.000000 kanonym4text-0.1.8/kanonym4text/__init__.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-05 07:39:54.758819 kanonym4text-0.1.8/kanonym4text/data/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    35592 2023-07-01 20:45:19.000000 kanonym4text-0.1.8/kanonym4text/data/5000_most_common_words_by_order.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11980 2023-07-05 07:08:23.000000 kanonym4text-0.1.8/kanonym4text/k_anonym_text.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-05 07:39:54.758819 kanonym4text-0.1.8/kanonym4text/utils/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-07-01 20:45:19.000000 kanonym4text-0.1.8/kanonym4text/utils/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13374 2023-07-01 20:45:19.000000 kanonym4text-0.1.8/kanonym4text/utils/anonym_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8761 2023-07-01 20:45:19.000000 kanonym4text-0.1.8/kanonym4text/utils/cluster_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6041 2023-07-05 07:36:00.000000 kanonym4text-0.1.8/kanonym4text/utils/llm_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      721 2023-07-05 07:09:39.000000 kanonym4text-0.1.8/kanonym4text/utils/models.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11197 2023-07-01 20:45:19.000000 kanonym4text-0.1.8/kanonym4text/utils/nlp_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3133 2023-07-05 07:34:31.000000 kanonym4text-0.1.8/kanonym4text/utils/utilization_utils.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-05 07:39:54.758819 kanonym4text-0.1.8/kanonym4text.egg-info/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-05 07:39:54.000000 kanonym4text-0.1.8/kanonym4text.egg-info/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      685 2023-07-05 07:39:54.000000 kanonym4text-0.1.8/kanonym4text.egg-info/SOURCES.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        1 2023-07-05 07:39:54.000000 kanonym4text-0.1.8/kanonym4text.egg-info/dependency_links.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      189 2023-07-05 07:39:54.000000 kanonym4text-0.1.8/kanonym4text.egg-info/requires.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       19 2023-07-05 07:39:54.000000 kanonym4text-0.1.8/kanonym4text.egg-info/top_level.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       38 2023-07-05 07:39:54.758819 kanonym4text-0.1.8/setup.cfg
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     1571 2023-07-05 07:39:25.000000 kanonym4text-0.1.8/setup.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-05 07:39:54.758819 kanonym4text-0.1.8/utils/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-06-28 09:31:23.000000 kanonym4text-0.1.8/utils/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13294 2023-07-05 07:08:23.000000 kanonym4text-0.1.8/utils/anonym_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8723 2023-07-05 07:08:23.000000 kanonym4text-0.1.8/utils/cluster_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6048 2023-07-05 07:08:23.000000 kanonym4text-0.1.8/utils/llm_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      953 2023-07-01 20:45:19.000000 kanonym4text-0.1.8/utils/models.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11195 2023-06-28 09:31:23.000000 kanonym4text-0.1.8/utils/nlp_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3161 2023-07-01 20:45:19.000000 kanonym4text-0.1.8/utils/utilization_utils.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/PKG-INFO
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     5099 2023-07-01 20:45:19.000000 kanonym4text-0.2.1/README.md
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      119 2023-07-06 09:36:30.000000 kanonym4text-0.2.1/kanonym4text/__init__.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text/data/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    35592 2023-07-01 20:45:19.000000 kanonym4text-0.2.1/kanonym4text/data/5000_most_common_words_by_order.txt
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text/objects/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       52 2023-07-06 09:06:10.000000 kanonym4text-0.2.1/kanonym4text/objects/__init__.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8013 2023-07-06 10:20:08.000000 kanonym4text-0.2.1/kanonym4text/objects/kanonym.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text/utils/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-07-01 20:45:19.000000 kanonym4text-0.2.1/kanonym4text/utils/__init__.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13290 2023-07-06 10:16:14.000000 kanonym4text-0.2.1/kanonym4text/utils/anonym_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8723 2023-07-06 10:17:19.000000 kanonym4text-0.2.1/kanonym4text/utils/cluster_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6024 2023-07-06 10:14:17.000000 kanonym4text-0.2.1/kanonym4text/utils/llm_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      721 2023-07-05 07:09:39.000000 kanonym4text-0.2.1/kanonym4text/utils/models.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11168 2023-07-06 08:39:12.000000 kanonym4text-0.2.1/kanonym4text/utils/nlp_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3152 2023-07-06 08:40:32.000000 kanonym4text-0.2.1/kanonym4text/utils/utilization_utils.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text.egg-info/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/PKG-INFO
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      576 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/SOURCES.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        1 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/dependency_links.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      189 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/requires.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       13 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/top_level.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       38 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/setup.cfg
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     1571 2023-07-06 10:22:24.000000 kanonym4text-0.2.1/setup.py
```

### Comparing `kanonym4text-0.1.8/README.md` & `kanonym4text-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.8/kanonym4text/data/5000_most_common_words_by_order.txt` & `kanonym4text-0.2.1/kanonym4text/data/5000_most_common_words_by_order.txt`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.8/kanonym4text/utils/anonym_utils.py` & `kanonym4text-0.2.1/kanonym4text/utils/anonym_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from annoy import AnnoyIndex
 from k_means_constrained import KMeansConstrained
 from sklearn.decomposition import PCA
 from sklearn.feature_extraction.text import TfidfVectorizer
 
 from . import nlp_utils
 
+
 def reduce_dims(vecs, dims=100):
     """
     Reduces dimensions using PCA.
     Returns: the low-dimensional vectors
     """
     # Reduce dimensions only if the dimensions are big
     if dims < min(vecs.shape):
@@ -24,103 +25,92 @@
     return vecs
 
 
 def lemmatize_and_remove_stops(corpus, stop_list):
     """
     Alternative version to nlp_utils.clean_corpus
     """
-    ccorpus = []
+    c_corpus = []
     for doc in corpus:
-        cdoc = nlp_utils.cleaning(doc, stop_list)
-        ccorpus.append(cdoc)
+        c_doc = nlp_utils.cleaning(doc, stop_list)
+        c_corpus.append(c_doc)
         
-    return ccorpus
+    return c_corpus
 
 
 def remove_stops(corpus, stop_list):
     """
     remove stop words only
     """
-    
-    ccorpus = []
+    c_corpus = []
     for doc in corpus:
         if doc:
             doc_tokenize = nlp_utils.nlp(doc)
-
             txt = []
             for token in doc_tokenize:
                 word = re.sub('\W+', '', str(token)).lower()
-
                 if word and (word not in stop_list):
-                    txt.append(str(token)) # onclude all the marks that are not words 
-        
+                    txt.append(str(token))  # include all the marks that are not words
             clean_doc = ' '.join(txt)
-
         else:
             clean_doc = doc
-        ccorpus.append(clean_doc)
+        c_corpus.append(clean_doc)
+    return c_corpus
 
-    return ccorpus
 
-
-def get_bow(corpus, stop_list, lemmatize = True):
-    """ Vectorizes the corpus using CountVectorizer """
+def get_bow(corpus, stop_list, lemmatize=True):
+    """ Vectorize the corpus using CountVectorizer """
     
-    vectorizer = CountVectorizer(ngram_range=(1,1))
+    vectorizer = CountVectorizer(ngram_range=(1, 1))
     if stop_list is not None:
         if lemmatize:
             cc = lemmatize_and_remove_stops(corpus, stop_list)
         else:
             cc = remove_stops(corpus, stop_list)
     else:
         logging.warning('Creating BoW without stopwords removal')
         cc = corpus
-    # print(corpus)
-    # print(cc)
-
     try:
-        # Vectorizing
         count_data = vectorizer.fit_transform(cc)
         voc = vectorizer.get_feature_names_out()
 
     except Exception as e:
         logging.warning(f'Could not create a bow: {e}')
         count_data, voc = None, None
     return count_data, voc
 
 
-def get_tfidf(corpus): #, stop_list, clean = True, lemmatize = True):
-    """ Vectorizes the corpus using CountVectorizer """
+def get_tfidf(corpus):  # stop_list, clean = True, lemmatize = True):
+    """ Vectorize the corpus using CountVectorizer """
 
     try:
-        # Vectorizing
         tfidf_model = TfidfVectorizer()
 
         # Fit Model
         tfidf_vectors = tfidf_model.fit_transform(corpus)
         # voc = tfidf_model.get_feature_names_out()
         voc = None  # Not needed
 
     except Exception as e:
         logging.warning('Could not create a Tf-Idf:', e)
         tfidf_model, voc = None, None
     
     return tfidf_vectors, voc
 
 
-def get_anonym_degree(docs = None, vecs = None, min_k = None, stop_list=None):
+def get_anonym_degree(docs=None, vecs=None, min_k=None, stop_list=None):
     """ If K not given, returns the minimal current k and the corresponding documents.
         If k is given, return the documents with k or less neighbohrs  """
     
     if docs is not None:
         # Lemmatizing the documents
         count_data, _ = get_bow(docs, stop_list=stop_list, lemmatize=False)
     elif vecs is not None:
         count_data = vecs
-    else: # No input docs or vecs
+    else:  # No input docs or vecs
         print('You must supply documents or vectors')
         return
     if count_data is not None:
         # Converting to array if is sparse
         if scipy.sparse.issparse(count_data):
             count_data = count_data.toarray()
         # Converting any number larger than 1 into 1
@@ -131,57 +121,54 @@
         if not min_k:
             min_k = min(uniq_cnt)
             # All the unique vectors
             un_anon = uniq_arr[uniq_cnt <= min_k]
         else:
             # All the unique vectors
             un_anon = uniq_arr[uniq_cnt < min_k]
-            min_k = min(uniq_cnt) # For the return value
+            min_k = min(uniq_cnt)  # For the return value
 
-        # Getting the unique vectore indeces
-        indeces_list = []
+        # Getting the unique vector indices
+        indices_list = []
         for row in un_anon:
             # Get the similar rows
-            similar_vals = np.where((count_data == (row)).all(axis=1))
-            indeces_list.append(similar_vals[0].tolist())
+            similar_vals = np.where((count_data == row).all(axis=1))
+            indices_list.append(similar_vals[0].tolist())
     else:  # count_data is None
-        min_k, indeces_list = None, []
+        min_k, indices_list = None, []
 
-    return min_k, indeces_list
+    return min_k, indices_list
 
 
 def get_diff(vecs):
     """
     Finds the differences between arrays of 0,1.
     The input is either a list of lists or a matrix
     """
     # Creating a matrix if needed
     if isinstance(vecs, list):
         mat = np.vstack(vecs)
     else: 
         mat = vecs
     mat[mat > 0] = 1
-    #nparray = sparse_mat.toarray()
     xsum = np.sum(mat, axis=0)
 
-    #print('xsum\n', xsum)
-
     union_x = (xsum > 0).astype('int')
     inter_x = (xsum == mat.shape[0]).astype('int')
 
     diff = union_x - inter_x
     return diff
 
 
 def build_annoy_search_tree(n_list):
     """
     Builds annoy search tree
     n_list: A matrix. rows = documents. columns = vocabulary
     """
-    # Build an Annoy index with 10 trees. angular = cosine similarity
+    # Build Annoy index with 10 trees. angular = cosine similarity
     annoy_index = AnnoyIndex(n_list.shape[1], metric='angular')
     for i, x in enumerate(n_list):
         annoy_index.add_item(i, x)
     annoy_index.build(10)
 
     return annoy_index
 
@@ -191,64 +178,62 @@
     Returns k unused items.
     """
     # Find the k nearest neighbors to the first sentence
     k_unused_items = []
     new_k = k
 
     i = 0  # TEMP
-
     while len(k_unused_items) < k:
         nearest_neighbors = annoy_tree.get_nns_by_vector(item, new_k)
         for nn in nearest_neighbors:
             if (nn not in used_items) and (len(k_unused_items) < k) and (nn not in k_unused_items):
                 k_unused_items.append(nn)
         new_k += 1
         i += 1  # TEMP
     return k_unused_items
 
 
-def find_k_neighbors_using_annoy(docs, k, dim_reduct = 0, stop_list = None):
+def find_k_neighbors_using_annoy(docs, k, dim_reduct=0, stop_list = None):
     """
     1. Create BoW representation
     2. For each document, finds k nearest neighbors
     Returns a list of indexes.
     """
-    if isinstance(docs, np.ndarray): # Documents already embedded
+    if isinstance(docs, np.ndarray):  # Documents already embedded
         vecs = docs
     
-    else: # A list of texts
+    else:  # A list of texts
         # Cleaning the documents
         cdocs = [nlp_utils.lemmatize_doc(doc, stop_list=stop_list) for doc in docs]
         docs = cdocs
         vecs, _ = get_tfidf(docs)
         vecs = vecs.toarray()  # From sparse matrix to array 
         
         # Reduce dimensions
         if dim_reduct:
             vecs = reduce_dims(vecs=vecs, dims=dim_reduct)
 
     neighbor_list = []
     annoy_tree = build_annoy_search_tree(vecs)
-
     logging.debug('Finding k neighbors using Annoy...')
 
     used_indexes = set([])
     num_docs = vecs.shape[0]
     for i in range(num_docs):
-        # To prevent redandent
+        # To prevent redundant
         if i not in used_indexes:
             similar_doc_ind = get_k_unused_items(vecs[i], annoy_tree, used_indexes, k)
             neighbor_list.append(similar_doc_ind)
             for sd in similar_doc_ind:
                 if sd in used_indexes:
                     logging.warning(f'The index {sd} was already used.')
                 # Adding the index to the used items
                 used_indexes.add(sd)  
             # No more k unused indexes
-            if  len(used_indexes) > (num_docs - k):
+            if len(used_indexes) > (num_docs - k):
                 break
 
     return neighbor_list
 
 
 def reorder_documents(doc_list, neighbor_list, num):
     """
@@ -275,15 +260,15 @@
             neighbor_list_docs[i][j] = doc_list[doc_idx]
     return pd.DataFrame(neighbor_list_docs)
 
 
 def force_anonym(docs, neighbor_list, stop_list):
     """ 
     For each group of neighbors, replace different words in *.
-    Returns a list of anonymized documents.
+    Returns a list of anonymize documents.
     """
     annon_docs = docs.copy()
  
     cdocs = [nlp_utils.lemmatize_doc(doc, stop_list=stop_list) for doc in docs]
     docs = cdocs
 
     used_indexes = []
@@ -306,20 +291,20 @@
         annon_docs[i] = '*'
 
     return annon_docs
 
 
 def add_neighbor_list_to_df(df, neighbor_list):
     """
-    Adds the neigbors for each document
+    Adds the neighbors for each document
     """
-    df['neigbors'] = None
+    df['neighbors'] = None  # corrected typo in column name from "neigbors" to "neighbors"
     for k_neighbors in neighbor_list:
         for n in k_neighbors:
-            df.loc[n, 'neigbors'] = str(k_neighbors)
+            df.loc[n, 'neighbors'] = str(k_neighbors)
     return df
 
 
 def delete_uncommon_words(docs, stop_list):
     """
     Deletes the uncommon words from given documents
     """
@@ -336,15 +321,15 @@
         
         # logging.debug(f'docs: {docs} \nuncommon words: {words_to_delete}')
 
         temp_docs = []
         for d in ldocs:
             new_d = d
             for word in words_to_delete:
-                #new_d = new_d.replace(word, '*')
+                # new_d = new_d.replace(word, '*')
                 new_d = re.sub(rf'\b{word}\b', '*', new_d, flags=re.IGNORECASE)
             temp_docs.append(new_d)
     else:
         # All stop words. Return lemmatized document
         temp_docs = ldocs
     
     # logging.debug(f'After forcing: {temp_docs}')
@@ -364,22 +349,24 @@
                 break  # Exit for
 
 
 # TEMP - also in LLM-utils
 def ckmeans_clustering(docs, k, n_jobs = -1, dim_reduct = 0, stop_list = None):
     """
     Runs k-means with constrains.
-    More on constrain-k-means: https://towardsdatascience.com/advanced-k-means-controlling-groups-sizes-and-selecting-features-a998df7e6745
+    More on constrain-k-means:
+    https://towardsdatascience.com/advanced-k-means-controlling-groups-sizes-
+    and-selecting-features-a998df7e6745
     Returns a list of neighbor list
     """
     logging.debug(f'{len(docs)} documents')
     
-    if isinstance(docs, np.ndarray): # Documents already embedded
+    if isinstance(docs, np.ndarray):  # Documents already embedded
         vecs = docs
-    else: # A list of texts
+    else:  # A list of texts
         # Cleaning the documents
         cdocs = [nlp_utils.lemmatize_doc(doc, stop_list=stop_list) for doc in docs]
         docs = cdocs
         vecs, _ = get_tfidf(docs)
 
         vecs = vecs.toarray()  # From sparse matrix to array (KMeansConstrained does not work on sparse matrix)
 
@@ -407,24 +394,25 @@
      size_max=max_size,
      random_state=0,
      n_jobs=n_jobs,
      n_init=n_init,
      max_iter=max_iter
     )
     # Logging
-    logging.debug(f'Clustering... Data dimensions: {vecs.shape}, Parameters: n_init {n_init}   max_iter {max_iter}   n_jobs {n_jobs}')
+    logging.debug(f'Clustering... Data dimensions: {vecs.shape}, Parameters: n_init {n_init} '
+                  f'  max_iter {max_iter}   n_jobs {n_jobs}')
 
     try:
         clf.fit_predict(vecs)
         logging.debug('Finish clustering. Getting original indexes.')
         pair_list = []
         for i in range(1, num_clusters):
             curr_pair = np.where(clf.labels_ == (i))[0].tolist()
             if curr_pair not in pair_list:
                 pair_list.append(tuple(curr_pair))
     except Exception as e:
         logging.error(f'Could not find neighbors using k_means_constrained: {e}')
         logging.info('Finding K neighbors using Annoy')
         # Sending the already cleaned vectors
-        pair_list = find_k_neighbors_using_annoy(docs=None, k=k, vecs=vecs, dim_reduct = dim_reduct)
+        pair_list = find_k_neighbors_using_annoy(docs=None, k=k, vecs=vecs, dim_reduct=dim_reduct)
         
     return pair_list
```

### Comparing `kanonym4text-0.1.8/kanonym4text/utils/cluster_utils.py` & `kanonym4text-0.2.1/kanonym4text/utils/cluster_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Imports
 import numpy as np
 from sklearn.cluster import DBSCAN
 import matplotlib.pyplot as plt
 import logging
 
+
 def define_eps_cos(wemodel):
     """Defines distance between pairs of words"""
     
     # Collecting distances of good pairs - cosine similarity
     sim_list_best = get_pairs_sim_cos(get_good_pairs(), wemodel)
     # print('mean similarity between good pairs\t', np.median(sim_list_best))
 
@@ -42,70 +43,70 @@
     threshold = (best_dist + worst_dist)/2
     return threshold
 
 
 def get_good_pairs():
     """Returns pairs of similar words"""
     best_pairs_ls = [
-        ['good','great'],
-        ['dog','cat'],
-        ['green','yellow'],
-        ['dad','mom'],
-        ['purchase','buy'],
-        ['gift','present'],
-        ['fast','quick'],
-        ['big','huge'],
-        ['item','product'],
-        ['text','script'],
-        ['john','julie'], # Adding names
-        ['shirley','matthew'],
-        ['joseph','smith'],
-        ['michael','sylvia'],
-        ['bonnie','henry'],
-        ['paul','jr'],
-        ['duncan','kelly']]
+        ['good', 'great'],
+        ['dog', 'cat'],
+        ['green', 'yellow'],
+        ['dad', 'mom'],
+        ['purchase', 'buy'],
+        ['gift', 'present'],
+        ['fast', 'quick'],
+        ['big', 'huge'],
+        ['item', 'product'],
+        ['text', 'script'],
+        ['john', 'julie'],  # Adding names
+        ['shirley', 'matthew'],
+        ['joseph', 'smith'],
+        ['michael', 'sylvia'],
+        ['bonnie', 'henry'],
+        ['paul', 'jr'],
+        ['duncan', 'kelly']]
     return best_pairs_ls
 
 
 def get_bad_pairs():
-    """Returns pairs of unsimilar words"""
+    """Returns pairs of dissimilar words"""
     worst_pairs_ls = [
-        ['good','trip'],
-        ['think','fat'],
-        ['sister','white'],
-        ['grammar','small'],
-        ['boy','buy'],
-        ['playstation','old'],
-        ['cd','low'],
-        ['battery','cold'],
-        ['wonderful','check'],
-        ['book','rich'],
-        ['brother','unless'],
-        ['john','ear'],
-        ['sixty','stay'],
-        ['barbara','wave'],
-        ['buy','niece']]
+        ['good', 'trip'],
+        ['think', 'fat'],
+        ['sister', 'white'],
+        ['grammar', 'small'],
+        ['boy', 'buy'],
+        ['playstation', 'old'],
+        ['cd', 'low'],
+        ['battery', 'cold'],
+        ['wonderful', 'check'],
+        ['book', 'rich'],
+        ['brother', 'unless'],
+        ['john', 'ear'],
+        ['sixty', 'stay'],
+        ['barbara', 'wave'],
+        ['buy', 'niece']]
     return worst_pairs_ls
 
 
 def get_pairs_sim_cos(pair_list, wemodel):
-    """Embed each word in the pairs and returns the distance between thems"""
+    """Embed each word in the pairs and returns the distance between them"""
     sim_list = []
     for pair in pair_list:
         # calc cosine dist between w1 and w2
         emb1 = wemodel[pair[0]]
         emb2 = wemodel[pair[1]]
         similarity = np.dot(emb1, emb2) / (np.linalg.norm(emb1) * np.linalg.norm(emb2))
         sim_list.append(similarity)
         
     return sim_list
 
 
 def get_pairs_dist_euc(pair_list, wemodel):
-    """Embed each word in the pairs and returns the distance between thems"""
+    """Embed each word in the pairs and returns the distance between them"""
     dist_list = []
     for pair in pair_list:
         # calc cosine dist between w1 and w2
         emb1 = wemodel[pair[0]]
         emb2 = wemodel[pair[1]]
         dist = np.linalg.norm(emb1 - emb2)
         dist_list.append(dist)
@@ -113,15 +114,15 @@
     return dist_list
 
 
 def get_word_list_for_clustering(word_dict):
     """Lemmatizing and remove stop words"""
     word_list = []
     for key, val in word_dict.items():
-        if (not val['protected']):  # Not protected 
+        if not val['protected']:  # Not protected
             if val['lemma']:
                 word_list.append(val['lemma'])
             else:
                 word_list.append(key)
             
     return list(set(word_list))  # Remove duplicates 
 
@@ -140,15 +141,15 @@
                 embedded_dict[word] = wemodel[word]
             except KeyError:
                 # If the word is not in the GloVe vocabulary, assign a default embedding or skip it
                 pass
     return embedded_dict
 
 
-def run_clustering(word_dict, stop_list, wemodel, cosine = True, eps = None, n_jobs = -1):
+def run_clustering(word_dict, stop_list, wemodel, cosine=True, eps=None, n_jobs=-1):
     """ Runs clustering """
     # point to think - min_points in cluster to be defined according to k?
     # Get embedding
     embedded_dict = embed_corpus(word_dict, stop_list, wemodel)
     # Convert to numpy array
     embeddings = np.array(list(embedded_dict.values()))
 
@@ -181,59 +182,58 @@
     # Getting the maximal distance in each cluster
     distance_dict = get_dist_dict(embedded_dict, clusters, labels)
 
     return clusters, distance_dict, labels
 
 
 def get_dist_dict(embedded_dict, clusters, labels):
-    """Calculates the max distance fore each cluster and return a dicionary of cluster num: max. distance"""
+    """Calculates the max distance fore each cluster and return a dictionary of cluster num: max. distance"""
     # init dict of dist:
     dist_dict = {}
 
     # for each cluster return the pair of words and max dist of the cluster:
     for ind in set(labels):
-        filtered_dict = {k: v for k, v in embedded_dict.items() if k in clusters[ind]} # dict of embeddings of the words in the cluster
+        filtered_dict = {k: v for k, v in embedded_dict.items() if k in clusters[ind]}
         curr_vecs = list(filtered_dict.values())
 
-        # Finding the centorid
+        # Finding the centroid
         centroid = np.mean(curr_vecs, axis=0)
         curr_dis_list = []
         for v in curr_vecs:
-            # Adding the absolut distance from centorid
+            # Adding the absolut distance from centroid
             curr_dis_list.append(np.abs(v-centroid)) 
         dist = np.mean(curr_dis_list)
         dist_dict[ind] = dist
     return dist_dict
 
 
 def get_word_index_for_clustering(all_words, stop_list):
     """ Uses tokenizer to get word indexes """
     word_index = {}
     i = 0
     for word in all_words:
-        if word and (word not in stop_list): #  stopwords.words('english')):
+        if word and (word not in stop_list):  # stopwords.words('english')):
             word_index[word] = i
             i += 1
 
     return word_index
 
 
 def plot_cluster_size_distribution(clusters):  # PIE CHART
     """
     Plots cluster size distribution.
     Input: dictionary of key: [item1, item2, ...]
     """
-    # NOT INCLUSING CLUSTER -1
+    # NOT INCLUDING CLUSTER -1
     size_list = []
     copy_clusters = clusters
     if -1 in copy_clusters:
         del copy_clusters[-1]
 
     for l in copy_clusters.values():
-      #print(l)
       if l == -1:
         continue
       else:
         size_list.append(len(l))
 
     # cluster_sizes is a list or array containing the number of data points in each cluster
     plt.pie(size_list, labels=size_list)
@@ -249,10 +249,11 @@
     plt.bar(range(len(limited_size_list)), limited_size_list)
     # Customize the x-axis labels if needed
     plt.xticks(range(len(limited_size_list)), range(1, len(limited_size_list) + 1))
     plt.xlabel('Cluster No.')
     plt.ylabel('Words in cluster')
     plt.show()
 
+
 if __name__ == '__main__':
     print('YEHH')
```

### Comparing `kanonym4text-0.1.8/kanonym4text/utils/llm_utils.py` & `kanonym4text-0.2.1/kanonym4text/utils/llm_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM
 from sentence_transformers import SentenceTransformer
-import numpy as np
 import logging
 from . import anonym_utils
 
 
 def print_example(indexes, origina_docs, new_docs):
     print('Before:')
     for i in indexes:
         print(origina_docs[i])
     print('\nAfter:')
     for i in indexes:
         print(new_docs[i])
 
 
-def sum_text_0(doc_list, tokenizer, gen_model):
+def sum_text_basic(doc_list, tokenizer, gen_model):
     # define the input sentences
-    #input_text = '. '.join(doc_list)
+    # input_text = '. '.join(doc_list)
     input_text = ''
     for doc in doc_list:
        input_text = f'{input_text}\n- {doc}. ' 
 
     # preprocess the input sentences
     input_ids = tokenizer.encode(f'Generate a general form of these sentences: \n{input_text}', return_tensors="pt")
 
@@ -29,15 +28,15 @@
     output = tokenizer.decode(output_ids[0], skip_special_tokens=True)
 
     return output
 
 
 def sum_text(doc_list, tokenizer, gen_model):
     # define the input sentences
-    #input_text = '. '.join(doc_list)
+    # input_text = '. '.join(doc_list)
     input_text = ''
     i = 1
     for doc in doc_list:
        input_text = f'{input_text}{i}: {doc}. ' 
        i += 1
     
     # print('doc_list:', doc_list)
@@ -86,31 +85,31 @@
             # Adding the document to the similar doc list
             curr_docs.append(docs[doc_index])
         sum_doc = sum_text(curr_docs, tokenizer, gen_model)
         # sum_doc = sum_text_0(curr_docs, tokenizer, gen_model)
         # print('similar_doc_ind', n, '\tSummary:', sum_doc)
         for doc_index in n:
             annon_docs[doc_index] = sum_doc
-    
+
     logging.info(f'Generation completed.')
 
     return annon_docs, neighbor_list
 
 
 def prompt_builder(docs):
     """
     Generating the prompt for document generalization
     """
 
-    # Removing /n from documens
+    # Removing /n from documents
     new_docs = []
     for d in docs:
         new_docs.append(d.replace('\n',' '))
     
-    # Adding new line and '-' between documnets
+    # Adding new line and '-' between documents
     sents = '\n-'.join(new_docs)
     # Adding '-' before the first document
     sents = '-' + sents + '\n'
 
     prompt = f'''Write a general sentence that best represents each of the following sentences and is true to all of them. For example: 
 
 Sentences:
```

### Comparing `kanonym4text-0.1.8/kanonym4text/utils/models.py` & `kanonym4text-0.2.1/kanonym4text/utils/models.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.1.8/kanonym4text/utils/nlp_utils.py` & `kanonym4text-0.2.1/kanonym4text/utils/nlp_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,17 +246,17 @@
     """ Replaces the words in the dataframe """
 
     out_str = f'Number of clusters: {len(cluster_dict)}   num protected words: {len(stop_list)}'
     logging.debug(out_str)
 
     # Working with a copy of the df:
     df_copy = df_0
-    # word_dict_copy = word_dict_0.copy()
 
-    df_copy['anon_txt'] = df_copy[col].apply(lambda x: lemmatize_doc(x, stop_list=stop_list))
+    new_txt = 'general_txt'
+    df_copy[new_txt] = df_copy[col].apply(lambda x: lemmatize_doc(x, stop_list=stop_list))
 
     logging.debug('Going over clusters')
 
     max_size = 0
 
     for key, words in cluster_dict.items():
         if key >= 0:  # Ignoring the -1 label
@@ -277,25 +277,25 @@
                 if word not in word_dict_copy:  # Lemmatized word
                     word_dict_copy[word] = {'protected': False, 'lemma': word, 'replaced':False}
                     
                 if not word_dict_copy[word]['protected']:
                     # Updaing the word dictionary that the words were replaced
                     word_dict_copy[word]['replaced'] = general_word  # Problem: greate in line 2 miss-identified as replaced
                 
-                # df_copy['anon_txt'] = df_copy['anon_txt'].replace(fr'\b{word}\b', general_word, regex=True)
+                # df_copy[new_txt] = df_copy[new_txt].replace(fr'\b{word}\b', general_word, regex=True)
                 
                 words_to_replace.append(word)
 
             # Replacing whole words
             rep_str = create_rep_string(words_to_replace)
             # print('rep_str 1: ', rep_str)
             # rep_str = '\\b|\\b'.join(words_to_replace)
             # print('rep_str 2: ', rep_str)
 
-            df_copy['anon_txt'] = df_copy['anon_txt'].replace(fr'\b{rep_str}\b', general_word, regex=True)
+            df_copy[new_txt] = df_copy[new_txt].replace(fr'\b{rep_str}\b', general_word, regex=True)
     logging.debug('Creating history')
     logging.info(f'Largest clone size - {max_size}')
     df_copy['anon_txt_history'] = df_copy[col].apply(lambda x: print_doc(x, word_dict_copy))
 
     if stop_list:
         logging.debug('Stop word list was updated')
```

### Comparing `kanonym4text-0.1.8/kanonym4text/utils/utilization_utils.py` & `kanonym4text-0.2.1/kanonym4text/utils/utilization_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import xgboost as xgb
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.linalg import norm
 from sentence_transformers import SentenceTransformer
 import logging
 
-def get_mean_semantice_distance_for_corpus(cor1, cor2, prefix=None):
+def get_mean_semantice_distance_for_corpus(cor1, cor2, plot=False):
     """
     Calculates the distance for each pair of documents
     """
     sem_model = SentenceTransformer('sentence-transformers/all-MiniLM-L12-v1')
     cor1_embed = sem_model.encode(cor1, show_progress_bar=False)
     cor2_embed = sem_model.encode(cor2, show_progress_bar=False)
 
@@ -30,16 +30,16 @@
     # dist_list = []
     #
     # for doc1, doc2 in zip(cor1, cor2):
     #     dist_list.append(get_semantice_distance_for_docs(doc1, doc2, sem_model))
     mean_dist = np.mean(cosine_dist)
 
     # Plotting a histogram
-    if prefix:
-        plot_hist(data=cosine_dist, xlabel='Semantic Distance', fig_name=f'plots/{prefix}_semantic_hist.pdf')
+    if plot:
+        plot_hist(data=cosine_dist, xlabel='Semantic Distance', fig_name=None)
     
     return mean_dist
 
 
 def get_semantice_distance_for_docs(doc1, doc2, sem_model):
     """
     Generates sentence embedding and calculates the distance between them
@@ -53,15 +53,18 @@
 def plot_hist(data, xlabel, fig_name):
     """
     Plots a histogram and saves it.
     """
     plt.hist(data, bins=30)
     plt.ylabel('Count')
     plt.xlabel(xlabel)
-    plt.savefig(fig_name)
+    if fig_name:
+        plt.savefig(fig_name)
+    else:
+        plt.show()
 
 
 def embedded_dist(embed1, embed2):
     """
     this function recieve 2 embedings and return the cosine dist between the two
     we will use it to show the dist between embedings of a sentence before and after anonymization
     """
```

### Comparing `kanonym4text-0.1.8/setup.py` & `kanonym4text-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.8'
+VERSION = '0.2.1'
 DESCRIPTION = 'k-anonymity for texts'
 LONG_DESCRIPTION = 'A package that takes a dataframe with a corpus and return an anonymized corpus'
 
 # Setting up
 setup(
     name="kanonym4text",
     version=VERSION,
     author="Lior Trieman, Hadas Neuman",
     author_email="liortr30@gmail.com, hadas.doron@gmail.com",
     url='https://github.com/neumanh/K-anonymity-fot-texts',
 
-    download_url='https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.1.8.tar.gz',
+    download_url='https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.1.tar.gz',
 
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # package_dir={'kanonym4text': 'kanonym4text'},
     install_requires=[
```

