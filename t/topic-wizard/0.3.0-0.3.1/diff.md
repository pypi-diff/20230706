# Comparing `tmp/topic_wizard-0.3.0.tar.gz` & `tmp/topic_wizard-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic_wizard-0.3.0.tar", max compression
+gzip compressed data, was "topic_wizard-0.3.1.tar", max compression
```

## Comparing `topic_wizard-0.3.0.tar` & `topic_wizard-0.3.1.tar`

### file list

```diff
@@ -1,51 +1,57 @@
--rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.3.0/LICENSE
--rw-r--r--   0        0        0     3746 2023-06-30 16:33:58.855285 topic_wizard-0.3.0/README.md
--rw-r--r--   0        0        0      640 2023-06-30 16:34:27.363320 topic_wizard-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      404 2023-06-30 14:25:27.164990 topic_wizard-0.3.0/topicwizard/__init__.py
--rw-r--r--   0        0        0     8707 2023-06-30 16:17:44.330421 topic_wizard-0.3.0/topicwizard/app.py
--rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.3.0/topicwizard/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.0/topicwizard/blueprints/__init__.py
--rw-r--r--   0        0        0     6348 2023-06-30 14:13:08.495596 topic_wizard-0.3.0/topicwizard/blueprints/app.py
--rw-r--r--   0        0        0     4322 2023-05-17 11:05:13.211055 topic_wizard-0.3.0/topicwizard/blueprints/documents.py
--rw-r--r--   0        0        0     1091 2023-05-17 13:10:22.409355 topic_wizard-0.3.0/topicwizard/blueprints/groups.py
--rw-r--r--   0        0        0     2338 2023-06-30 14:20:46.656474 topic_wizard-0.3.0/topicwizard/blueprints/template.py
--rw-r--r--   0        0        0     4979 2023-06-30 14:12:57.739575 topic_wizard-0.3.0/topicwizard/blueprints/topics.py
--rw-r--r--   0        0        0     3015 2023-05-17 11:05:57.615132 topic_wizard-0.3.0/topicwizard/blueprints/words.py
--rw-r--r--   0        0        0     3010 2023-05-17 11:32:05.865790 topic_wizard-0.3.0/topicwizard/compatibility/bertopic.py
--rw-r--r--   0        0        0     6425 2023-05-17 11:33:07.273886 topic_wizard-0.3.0/topicwizard/compatibility/gensim.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.0/topicwizard/components/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.0/topicwizard/components/documents/__init__.py
--rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.3.0/topicwizard/components/documents/document_map.py
--rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.3.0/topicwizard/components/documents/document_pie.py
--rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.3.0/topicwizard/components/documents/document_selector.py
--rw-r--r--   0        0        0     1468 2023-04-24 14:04:50.954173 topic_wizard-0.3.0/topicwizard/components/documents/document_timeline.py
--rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/documents/document_wordcloud.py
--rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/documents/window_slider.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/__init__.py
--rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/intertopic_map.py
--rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/relevance_slider.py
--rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/topic_barplot.py
--rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/topic_namer.py
--rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/topic_switcher.py
--rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/wordcloud.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/words/__init__.py
--rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.3.0/topicwizard/components/words/association_slider.py
--rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/words/word_barplot.py
--rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.3.0/topicwizard/components/words/word_map.py
--rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.3.0/topicwizard/components/words/word_selector.py
--rw-r--r--   0        0        0      498 2023-06-30 13:57:55.717853 topic_wizard-0.3.0/topicwizard/figures/__init__.py
--rw-r--r--   0        0        0     7715 2023-06-30 16:01:00.587374 topic_wizard-0.3.0/topicwizard/figures/documents.py
--rw-r--r--   0        0        0     9340 2023-06-30 13:03:18.543793 topic_wizard-0.3.0/topicwizard/figures/topics.py
--rw-r--r--   0        0        0     6392 2023-06-30 15:39:09.394441 topic_wizard-0.3.0/topicwizard/figures/words.py
--rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.3.0/topicwizard/plots/__init__.py
--rw-r--r--   0        0        0     5183 2023-05-17 10:58:27.942406 topic_wizard-0.3.0/topicwizard/plots/documents.py
--rw-r--r--   0        0        0     4244 2023-06-26 12:14:28.818856 topic_wizard-0.3.0/topicwizard/plots/topics.py
--rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.3.0/topicwizard/plots/words.py
--rw-r--r--   0        0        0        0 2023-06-26 12:10:25.930511 topic_wizard-0.3.0/topicwizard/prepare/__init__.py
--rw-r--r--   0        0        0     2708 2023-06-26 13:03:03.519611 topic_wizard-0.3.0/topicwizard/prepare/documents.py
--rw-r--r--   0        0        0     3681 2023-05-17 13:42:09.111617 topic_wizard-0.3.0/topicwizard/prepare/groups.py
--rw-r--r--   0        0        0     4895 2023-05-17 10:58:27.942406 topic_wizard-0.3.0/topicwizard/prepare/topics.py
--rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.3.0/topicwizard/prepare/utils.py
--rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.3.0/topicwizard/prepare/words.py
--rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 topic_wizard-0.3.0/setup.py
--rw-r--r--   0        0        0     4769 1970-01-01 00:00:00.000000 topic_wizard-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4534 2023-07-06 08:38:13.531980 topic_wizard-0.3.1/README.md
+-rw-r--r--   0        0        0      640 2023-07-06 08:26:14.602969 topic_wizard-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-06-30 14:25:27.164990 topic_wizard-0.3.1/topicwizard/__init__.py
+-rw-r--r--   0        0        0     9512 2023-07-06 08:25:44.631006 topic_wizard-0.3.1/topicwizard/app.py
+-rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.3.1/topicwizard/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.1/topicwizard/blueprints/__init__.py
+-rw-r--r--   0        0        0     7443 2023-07-06 08:25:44.631006 topic_wizard-0.3.1/topicwizard/blueprints/app.py
+-rw-r--r--   0        0        0     4322 2023-05-17 11:05:13.211055 topic_wizard-0.3.1/topicwizard/blueprints/documents.py
+-rw-r--r--   0        0        0     2490 2023-07-06 08:25:44.631006 topic_wizard-0.3.1/topicwizard/blueprints/groups.py
+-rw-r--r--   0        0        0     2516 2023-07-06 08:25:44.631006 topic_wizard-0.3.1/topicwizard/blueprints/template.py
+-rw-r--r--   0        0        0     4979 2023-06-30 14:12:57.739575 topic_wizard-0.3.1/topicwizard/blueprints/topics.py
+-rw-r--r--   0        0        0     3015 2023-05-17 11:05:57.615132 topic_wizard-0.3.1/topicwizard/blueprints/words.py
+-rw-r--r--   0        0        0     3937 2023-07-05 08:00:17.664404 topic_wizard-0.3.1/topicwizard/compatibility/bertopic.py
+-rw-r--r--   0        0        0     6425 2023-05-17 11:33:07.273886 topic_wizard-0.3.1/topicwizard/compatibility/gensim.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.1/topicwizard/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.1/topicwizard/components/documents/__init__.py
+-rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.3.1/topicwizard/components/documents/document_map.py
+-rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.3.1/topicwizard/components/documents/document_pie.py
+-rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.3.1/topicwizard/components/documents/document_selector.py
+-rw-r--r--   0        0        0     1708 2023-07-05 07:54:27.399506 topic_wizard-0.3.1/topicwizard/components/documents/document_timeline.py
+-rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/documents/document_wordcloud.py
+-rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/documents/window_slider.py
+-rw-r--r--   0        0        0      938 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/components/groups/group_barplot.py
+-rw-r--r--   0        0        0     2087 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/components/groups/group_map.py
+-rw-r--r--   0        0        0      848 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/components/groups/group_wordcloud.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/__init__.py
+-rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/intertopic_map.py
+-rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/relevance_slider.py
+-rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/topic_barplot.py
+-rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/topic_namer.py
+-rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/topic_switcher.py
+-rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/wordcloud.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/words/__init__.py
+-rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.3.1/topicwizard/components/words/association_slider.py
+-rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/words/word_barplot.py
+-rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.3.1/topicwizard/components/words/word_map.py
+-rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.3.1/topicwizard/components/words/word_selector.py
+-rw-r--r--   0        0        0      675 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/figures/__init__.py
+-rw-r--r--   0        0        0     7715 2023-07-05 07:49:54.902696 topic_wizard-0.3.1/topicwizard/figures/documents.py
+-rw-r--r--   0        0        0    10961 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/figures/groups.py
+-rw-r--r--   0        0        0     9502 2023-07-05 11:21:34.951475 topic_wizard-0.3.1/topicwizard/figures/topics.py
+-rw-r--r--   0        0        0     6392 2023-06-30 15:39:09.394441 topic_wizard-0.3.1/topicwizard/figures/words.py
+-rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.3.1/topicwizard/plots/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-17 10:58:27.942406 topic_wizard-0.3.1/topicwizard/plots/documents.py
+-rw-r--r--   0        0        0     4228 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/plots/groups.py
+-rw-r--r--   0        0        0     4244 2023-06-26 12:14:28.818856 topic_wizard-0.3.1/topicwizard/plots/topics.py
+-rw-r--r--   0        0        0      274 2023-07-05 07:56:39.267858 topic_wizard-0.3.1/topicwizard/plots/utils.py
+-rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.3.1/topicwizard/plots/words.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:10:25.930511 topic_wizard-0.3.1/topicwizard/prepare/__init__.py
+-rw-r--r--   0        0        0     2820 2023-07-05 07:49:23.926595 topic_wizard-0.3.1/topicwizard/prepare/documents.py
+-rw-r--r--   0        0        0     4837 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/prepare/groups.py
+-rw-r--r--   0        0        0     4949 2023-07-05 11:16:13.759839 topic_wizard-0.3.1/topicwizard/prepare/topics.py
+-rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.3.1/topicwizard/prepare/utils.py
+-rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.3.1/topicwizard/prepare/words.py
+-rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 topic_wizard-0.3.1/setup.py
+-rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 topic_wizard-0.3.1/PKG-INFO
```

### Comparing `topic_wizard-0.3.0/LICENSE` & `topic_wizard-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/README.md` & `topic_wizard-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,100 +13,124 @@
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 
 
 
 https://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4
 
-## New in version 0.3.0 🌟 🌟
+## New in version 0.3.1 🌟 🌟
+
+- You can now investigate relations of pre-existing labels to your topics and words :mag:
+
+## New in version 0.3.0 🌟 
 
  - Exclude pages, that are not needed :bird:
  - Self-contained interactive figures :gift:
  - Topic name inference is now default behavior and is done implicitly.
 
 
 ## Features
 
--   Investigate complex relations between topics, words and documents
--   Highly interactive
--   Automatically infer topic names
--   Name topics manually
--   Pretty :art:
--   Intuitive :cow:
--   Clean API :candy:
+-   Investigate complex relations between topics, words, documents and groups/genres/labels
 -   Sklearn, Gensim and BERTopic compatible :nut_and_bolt:
+-   Highly interactive web app
+-   Interactive and composable Plotly figures
+-   Automatically infer topic names, oooor...
+-   Name topics manually
 -   Easy deployment :earth_africa:
 
 ## Installation
 
 Install from PyPI:
 
 ```bash
 pip install topic-wizard
 ```
 
 ## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))
 
+### Step 0:
+
+Have a corpus ready for analysis, in this example I am going to use 20 newgroups from scikit-learn.
+
+```python
+from sklearn.datasets import fetch_20newsgroups
+
+newsgroups = fetch_20newsgroups(subset="all")
+corpus = newsgroups.data
+
+# Sklearn gives the labels back as integers, we have to map them back to
+# the actual textual label.
+group_labels = [newsgroups.target_names[label] for label in newsgroups.target]
+```
+
 ### Step 1:
 
 Train a scikit-learn compatible topic model.
 (If you want to use non-scikit-learn topic models, check [compatibility](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html))
 
 ```python
 from sklearn.decomposition import NMF
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.pipeline import make_pipeline
 
 # Create topic pipeline
-topic_pipeline = make_pipeline(
-    CountVectorizer(),
-    NMF(n_components=10),
+pipeline = make_pipeline(
+    CountVectorizer(stop_words="english", min_df=10),
+    NMF(n_components=30),
 )
 
 # Then fit it on the given texts
-topic_pipeline.fit(texts)
+pipeline.fit(corpus)
 ```
 
 ### Step 2a:
 
 Visualize with the topicwizard webapp :bulb:
 
 ```python
 import topicwizard
 
-topicwizard.visualize(pipeline=topic_pipeline, corpus=texts)
+topicwizard.visualize(corpus, pipeline=pipeline)
 ```
 
 From version 0.3.0 you can also disable pages you do not wish to display thereby sparing a lot of time for yourself:
 
 ```python
-import topicwizard
-
 # A large corpus takes a looong time to compute 2D projections for so
 # so you can speed up preprocessing by disabling it alltogether.
-topicwizard.visualize(pipeline=topic_pipeline, corpus=texts, exclude_pages=["documents"])
+topicwizard.visualize(corpus, pipeline=pipeline, exclude_pages=["documents"])
 ```
 
+
 ![topics screenshot](assets/screenshot_topics.png)
 ![words screenshot](assets/screenshot_words.png)
 ![words screenshot](assets/screenshot_words_zoomed.png)
 ![documents screenshot](assets/screenshot_documents.png)
 
+From version 0.3.1 you can investigate groups/labels by passing them along to the webapp.
+
+```python
+topicwizard.visualize(corpus, pipeline=pipeline, group_labels=group_labels)
+```
+
+![groups screenshot](docs/_static/screenshot_groups.png)
+
 Ooooor...
 
 ### Step 2b:
 
 Produce high quality self-contained HTML plots and create your own dashboards/reports :strawberry:
 
 ### Map of words
 
 ```python
 from topicwizard.figures import word_map
 
-word_map(corpus=texts, pipeline=pipeline)
+word_map(corpus, pipeline=pipeline)
 ```
 
 ![word map screenshot](assets/word_map.png)
 
 ### Timelines of topic distributions
 
 ```python
@@ -120,13 +144,13 @@
 ![document timeline](assets/document_topic_timeline.png)
 
 ### Wordclouds of your topics :cloud:
 
 ```python
 from topicwizard.figures import topic_wordclouds
 
-topic_wordclouds(corpus=texts, pipeline=pipeline)
+topic_wordclouds(corpus, pipeline=pipeline)
 ```
 
 ![wordclouds](assets/topic_wordclouds.png)
 
-### And much more ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))
+#### And much more... ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))
```

### Comparing `topic_wizard-0.3.0/pyproject.toml` & `topic_wizard-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "topic-wizard"
-version = "0.3.0"
+version = "0.3.1"
 description = "Pretty and opinionated topic model visualization in Python."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "topicwizard"}]
 
 [tool.poetry.dependencies]
```

### Comparing `topic_wizard-0.3.0/topicwizard/app.py` & `topic_wizard-0.3.1/topicwizard/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 def get_dash_app(
     vectorizer: Any,
     topic_model: Any,
     corpus: Iterable[str],
     exclude_pages: Set[PageName],
     document_names: Optional[List[str]] = None,
     topic_names: Optional[List[str]] = None,
+    group_labels: Optional[List[str]] = None,
 ) -> Dash:
     """Returns topicwizard Dash application.
 
     Parameters
     ----------
     vectorizer: Vectorizer
         Sklearn compatible vectorizer, that turns texts into
@@ -68,27 +69,33 @@
         List of all works in the corpus you intend to visualize.
     document_names: list of str, default None
         List of document names in the corpus, if not provided documents will
         be labeled 'Document <index>'.
     topic_names: list of str, default None
         List of topic names in the corpus, if not provided, topic
         labels will be inferred.
+    group_labels: list of str or None, default None
+        List of preexisting labels for the documents.
+        You can pass it along if you have genre labels for example.
+        In this case an additional page will get created with information
+        about how these groups relate to topics and words in the corpus.
 
     Returns
     -------
     Dash
         Dash application object for topicwizard.
     """
     blueprint = get_app_blueprint(
         vectorizer=vectorizer,
         topic_model=topic_model,
         corpus=corpus,
         document_names=document_names,
         topic_names=topic_names,
         exclude_pages=exclude_pages,
+        group_labels=group_labels,
     )
     app = Dash(
         __name__,
         blueprint=blueprint,
         title="topicwizard",
         external_scripts=[
             {
@@ -228,14 +235,15 @@
     corpus: Iterable[str],
     vectorizer: Optional[Any] = None,
     topic_model: Optional[Any] = None,
     pipeline: Optional[Pipeline] = None,
     document_names: Optional[List[str]] = None,
     topic_names: Optional[List[str]] = None,
     exclude_pages: Optional[Iterable[PageName]] = None,
+    group_labels: Optional[List[str]] = None,
     port: int = 8050,
 ) -> Optional[threading.Thread]:
     """Visualizes your topic model with topicwizard.
 
     Parameters
     ----------
     corpus: iterable of str
@@ -259,14 +267,20 @@
     exclude_pages: iterable of {"topics", "documents", "words"}
         Set of pages you want to exclude from the application.
         This can be relevant as with larger corpora for example,
         calculating UMAP embeddings for documents or words can take
         a long time and you might not be interested in them.
     port: int, default 8050
         Port where the application should run in localhost. Defaults to 8050.
+    group_labels: list of str or None, default None
+        List of preexisting labels for the documents.
+        You can pass it along if you have genre labels for example.
+        In this case an additional page will get created with information
+        about how these groups relate to topics and words in the corpus.
+
 
     Returns
     -------
     Thread or None
         Returns a Thread if running in a Jupyter notebook (so you can close the server)
         returns None otherwise.
     """
@@ -276,9 +290,10 @@
     app = get_dash_app(
         vectorizer=vectorizer,
         topic_model=topic_model,
         corpus=corpus,
         document_names=document_names,
         topic_names=topic_names,
         exclude_pages=exclude_pages,
+        group_labels=group_labels,
     )
     return run_app(app, port=port)
```

### Comparing `topic_wizard-0.3.0/topicwizard/assets/favicon.ico` & `topic_wizard-0.3.1/topicwizard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/blueprints/app.py` & `topic_wizard-0.3.1/topicwizard/blueprints/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from io import BytesIO
-from typing import Any, Dict, List, Set
+from typing import Any, Dict, List, Optional, Set
 
 import dash_mantine_components as dmc
 import joblib
 import numpy as np
 from dash_extensions.enrich import (
     DashBlueprint,
     Input,
@@ -12,14 +12,15 @@
     dcc,
     exceptions,
     html,
 )
 from dash_iconify import DashIconify
 
 import topicwizard.blueprints.documents as documents
+import topicwizard.blueprints.groups as groups
 import topicwizard.blueprints.topics as topics
 import topicwizard.blueprints.words as words
 from topicwizard.blueprints.template import create_blank_page
 
 
 def create_blueprint(
     vocab: np.ndarray,
@@ -28,14 +29,15 @@
     topic_term_matrix: np.ndarray,
     document_names: List[str],
     corpus: List[str],
     vectorizer: Any,
     topic_model: Any,
     topic_names: List[str],
     exclude_pages: Set[str],
+    group_labels: Optional[List[str]],
 ) -> DashBlueprint:
     # --------[ Collecting blueprints ]--------
     topic_blueprint = (
         topics.create_blueprint(
             vocab=vocab,
             document_term_matrix=document_term_matrix,
             document_topic_matrix=document_topic_matrix,
@@ -75,22 +77,41 @@
             vectorizer=vectorizer,
             topic_model=topic_model,
             topic_names=topic_names,
         )
         if "words" not in exclude_pages
         else create_blank_page("words")
     )
+    groups_blueprint = (
+        groups.create_blueprint(
+            vocab=vocab,
+            document_term_matrix=document_term_matrix,
+            document_topic_matrix=document_topic_matrix,
+            topic_term_matrix=topic_term_matrix,
+            document_names=document_names,
+            corpus=corpus,
+            vectorizer=vectorizer,
+            topic_model=topic_model,
+            topic_names=topic_names,
+            group_labels=group_labels,
+        )
+        if group_labels is not None
+        else create_blank_page("groups")
+    )
+    if group_labels is None:
+        exclude_pages = exclude_pages | set(["Groups"])
     options = []
-    for option in ["Topics", "Words", "Documents"]:
+    for option in ["Topics", "Words", "Documents", "Groups"]:
         if option.lower() not in exclude_pages:
             options.append(option)
     blueprints = [
         topic_blueprint,
         words_blueprint,
         documents_blueprint,
+        groups_blueprint,
     ]
 
     # --------[ Creating app blueprint ]--------
     app_blueprint = DashBlueprint()
 
     app_blueprint.layout = html.Div(
         [
@@ -98,14 +119,15 @@
             dcc.Store(
                 "topic_names",
                 data=topic_names,
             ),
             topic_blueprint.layout,
             words_blueprint.layout,
             documents_blueprint.layout,
+            groups_blueprint.layout,
             html.Div(
                 [
                     dmc.SegmentedControl(
                         id="page_picker",
                         data=options,
                         value=options[0],
                         color="orange",
@@ -165,42 +187,49 @@
 
     app_blueprint.clientside_callback(
         """
         function(currentPage){
             const visible = 'flex flex-1 flex-col p-3';
             const hidden = 'hidden';
             if (currentPage === 'Topics') {
-                return [visible, hidden, hidden];
+                return [visible, hidden, hidden, hidden];
             }
             if (currentPage === 'Words') {
-                return [hidden, visible, hidden];
+                return [hidden, visible, hidden, hidden];
             }
             if (currentPage === 'Documents') {
-                return [hidden, hidden, visible];
+                return [hidden, hidden, visible, hidden];
+            }
+            if (currentPage === 'Groups') {
+                return [hidden, hidden, hidden, visible];
             }
-            return [hidden, hidden, hidden];
+            return [hidden, hidden, hidden, hidden];
         }
         """,
         Output("topics_container", "className"),
         Output("words_container", "className"),
         Output("documents_container", "className"),
+        Output("groups_container", "className"),
         Input("page_picker", "value"),
     )
     app_blueprint.clientside_callback(
         """
         function(currentPage){
             if (currentPage === 'Topics') {
                 return 'orange';
             }
             if (currentPage === 'Words') {
                 return 'teal';
             }
             if (currentPage === 'Documents') {
                 return 'indigo';
             }
+            if (currentPage === 'Groups') {
+                return 'pink';
+            }
             return 'black';
         }
         """,
         Output("page_picker", "color"),
         Input("page_picker", "value"),
     )
```

### Comparing `topic_wizard-0.3.0/topicwizard/blueprints/documents.py` & `topic_wizard-0.3.1/topicwizard/blueprints/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/blueprints/template.py` & `topic_wizard-0.3.1/topicwizard/blueprints/template.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 def prepare_blueprint(
     vectorizer: Any,
     topic_model: Any,
     corpus: Iterable[str],
     create_blueprint: BlueprintCreator,
     document_names: Optional[List[str]] = None,
     topic_names: Optional[List[str]] = None,
+    group_labels: Optional[List[str]] = None,
     *args,
     **kwargs,
 ) -> DashBlueprint:
     corpus = list(corpus)
     n_documents = len(corpus)
     if document_names is None:
         document_names = [f"Document {i}" for i in range(n_documents)]
@@ -44,24 +45,27 @@
             f"{n_nan_docs} documents had nan values in the output of the topic model,"
             " these are removed in preprocessing and will not be visible in the app."
         )
         corpus = list(np.array(corpus)[~nan_documents])
         document_topic_matrix = document_topic_matrix[~nan_documents]
         document_term_matrix = document_term_matrix[~nan_documents]
         document_names = list(np.array(document_names)[~nan_documents])
+        if group_labels:
+            group_labels = list(np.array(group_labels)[~nan_documents])
     n_topics = topic_term_matrix.shape[0]
     if topic_names is None:
         topic_names = infer_topic_names(pipeline=make_pipeline(vectorizer, topic_model))
     blueprint = create_blueprint(
         vocab=vocab,
         document_term_matrix=document_term_matrix,
         document_topic_matrix=document_topic_matrix,
         topic_term_matrix=topic_term_matrix,
         document_names=document_names,
         corpus=corpus,
         vectorizer=vectorizer,
         topic_model=topic_model,
         topic_names=topic_names,
+        group_labels=group_labels,
         *args,
         **kwargs,
     )
     return blueprint
```

### Comparing `topic_wizard-0.3.0/topicwizard/blueprints/topics.py` & `topic_wizard-0.3.1/topicwizard/blueprints/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/blueprints/words.py` & `topic_wizard-0.3.1/topicwizard/blueprints/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/compatibility/gensim.py` & `topic_wizard-0.3.1/topicwizard/compatibility/gensim.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/documents/document_map.py` & `topic_wizard-0.3.1/topicwizard/components/documents/document_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/documents/document_pie.py` & `topic_wizard-0.3.1/topicwizard/components/documents/document_pie.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/documents/document_selector.py` & `topic_wizard-0.3.1/topicwizard/components/documents/document_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/documents/document_timeline.py` & `topic_wizard-0.3.1/topicwizard/components/documents/document_timeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 import plotly.graph_objects as go
 from dash_extensions.enrich import DashBlueprint, Input, Output, State, dcc
 
 import topicwizard.plots.documents as plots
 import topicwizard.prepare.documents as prepare
+from topicwizard.plots.utils import text_plot
 
 
 def create_timeline(
     corpus: List[str], vectorizer: Any, topic_model: Any, topic_colors: np.ndarray
 ):
     timeline = DashBlueprint()
 
@@ -29,22 +30,27 @@
         selected_document: Union[int, str],
         topic_names: List[str],
         window_size: int,
     ) -> go.Figure:
         if isinstance(selected_document, str):
             selected_document = selected_document.strip()
             selected_document = int(selected_document)
-        topic_timeline = prepare.calculate_timeline(
-            doc_id=selected_document,
-            corpus=corpus,
-            vectorizer=vectorizer,
-            topic_model=topic_model,
-            window_size=window_size,
-            step=1,
-        )
+        try:
+            topic_timeline = prepare.calculate_timeline(
+                doc_id=selected_document,
+                corpus=corpus,
+                vectorizer=vectorizer,
+                topic_model=topic_model,
+                window_size=window_size,
+                step=1,
+            )
+        except ValueError:
+            return text_plot(
+                "This document is not long enough to be broken into windows."
+            )
         return plots.document_timeline(
             topic_colors=topic_colors,
             topic_timeline=topic_timeline,
             topic_names=topic_names,
         )
 
     return timeline
```

### Comparing `topic_wizard-0.3.0/topicwizard/components/documents/document_wordcloud.py` & `topic_wizard-0.3.1/topicwizard/components/documents/document_wordcloud.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/documents/window_slider.py` & `topic_wizard-0.3.1/topicwizard/components/documents/window_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/topics/intertopic_map.py` & `topic_wizard-0.3.1/topicwizard/components/topics/intertopic_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/topics/relevance_slider.py` & `topic_wizard-0.3.1/topicwizard/components/topics/relevance_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/topics/topic_namer.py` & `topic_wizard-0.3.1/topicwizard/components/topics/topic_namer.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/topics/topic_switcher.py` & `topic_wizard-0.3.1/topicwizard/components/topics/topic_switcher.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/words/association_slider.py` & `topic_wizard-0.3.1/topicwizard/components/words/association_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/words/word_barplot.py` & `topic_wizard-0.3.1/topicwizard/components/words/word_barplot.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/words/word_map.py` & `topic_wizard-0.3.1/topicwizard/components/words/word_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/components/words/word_selector.py` & `topic_wizard-0.3.1/topicwizard/components/words/word_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/figures/documents.py` & `topic_wizard-0.3.1/topicwizard/figures/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/figures/topics.py` & `topic_wizard-0.3.1/topicwizard/figures/topics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """External API for creating self-contained figures for topics."""
 from typing import Any, Iterable, List, Optional
 
+import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from sklearn.pipeline import Pipeline, make_pipeline
 
 import topicwizard.plots.topics as plots
 import topicwizard.prepare.topics as prepare
 from topicwizard.app import split_pipeline
@@ -94,15 +95,15 @@
         bag-of-words representations.
     topic_model: TopicModel, default None
         Sklearn compatible topic model, that can transform documents
         into topic distributions.
     topic_names: list of str, default None
         List of topic names in the corpus, if not provided
         topic names will be inferred.
-    top_n: int, default 30
+    top_n: int, default 5
         Specifies the number of words to show for each topic.
     alpha: float, default 1.0
         Specifies relevance metric for obtaining the most relevant
         words. Has to be in range (0.0, 1.0).
         Numbers closer to zero will yield words that are more
         exclusive to the given topic.
     n_columns: int, default 4
@@ -135,27 +136,29 @@
         topic_names = prepare.infer_topic_names(pipeline)
     n_rows = (n_topics // n_columns) + 1
     fig = make_subplots(
         rows=n_rows,
         cols=n_columns,
         subplot_titles=topic_names,
         vertical_spacing=0.05,
-        horizontal_spacing=0.1,
+        horizontal_spacing=0.01,
     )
     for topic_id in range(n_topics):
         top_words = prepare.calculate_top_words(
             topic_id, top_n, alpha, term_importances, topic_term_importances, vocab
         )
+        max_importance = top_words.overall_importance.max()
         subfig = plots.topic_plot(top_words)
         row, column = (topic_id // n_columns) + 1, (topic_id % n_columns) + 1
         for trace in subfig.data:
             # hiding legend if it isn't the first trace.
             if topic_id:
                 trace.showlegend = False
             fig.add_trace(trace, row=row, col=column)
+            fig.update_xaxes(range=[0, max_importance * 1.5], row=row, col=column)
     fig.update_layout(
         barmode="overlay",
         plot_bgcolor="white",
         hovermode=False,
         uniformtext=dict(
             minsize=10,
             mode="show",
```

### Comparing `topic_wizard-0.3.0/topicwizard/figures/words.py` & `topic_wizard-0.3.1/topicwizard/figures/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/plots/documents.py` & `topic_wizard-0.3.1/topicwizard/plots/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/plots/topics.py` & `topic_wizard-0.3.1/topicwizard/plots/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/plots/words.py` & `topic_wizard-0.3.1/topicwizard/plots/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/prepare/documents.py` & `topic_wizard-0.3.1/topicwizard/prepare/documents.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Tuple
+from typing import Any, List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 import scipy.sparse as spr
 import umap
 
 
@@ -97,11 +97,13 @@
     Returns
     -------
     array of shape (n_windows, n_topics)
         Timeline of all topics over the entire document.
     """
     document = pd.Series(corpus[doc_id].split())
     windows = document.rolling(window_size, step=step)
-    texts = (" ".join(window) for window in windows)
+    texts = [" ".join(window) for window in windows]
+    if not texts:
+        raise ValueError("This text is not long enough for the given window size.")
     word_timeline = vectorizer.transform(texts)
     topic_timeline = topic_model.transform(word_timeline)
     return topic_timeline
```

### Comparing `topic_wizard-0.3.0/topicwizard/prepare/topics.py` & `topic_wizard-0.3.1/topicwizard/prepare/topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     x: array of shape (n_topics)
     y: array of shape (n_topics)
     """
     # Calculating distances
     n_topics = topic_term_matrix.shape[0]
     # Setting perplexity to 30, or the number of topics minus one
     perplexity = np.min((30, n_topics - 1))
-    if n_topics <= 3:
-        init = "random"
+    if n_topics >= 3:
+        manifold = umap.UMAP(
+            n_components=2, n_neighbors=perplexity, metric="cosine", init="random"
+        )
+        x, y = manifold.fit_transform(topic_term_matrix).T
     else:
-        init = "spectral"
-    manifold = umap.UMAP(
-        n_components=2, n_neighbors=perplexity, metric="cosine", init=init
-    )
-    x, y = manifold.fit_transform(topic_term_matrix).T
+        x = np.arange(n_topics)
+        y = np.zeros(n_topics)
     return x, y
 
 
 def topic_importances(
     topic_term_matrix: np.ndarray,
     document_term_matrix: np.ndarray,
     document_topic_matrix: np.ndarray,
@@ -137,15 +137,16 @@
         Number of words used to name the topic.
 
     Returns
     -------
     list of str
         List of topic names.
     """
-    ((_, vectorizer), (_, topic_model)) = pipeline.steps
+    _, vectorizer = pipeline.steps[0]
+    _, topic_model = pipeline.steps[-1]
     components = topic_model.components_
     vocab = vectorizer.get_feature_names_out()
     highest = np.argpartition(-components, top_n)[:, :top_n]
     top_words = vocab[highest]
     topic_names = []
     for i_topic, words in enumerate(top_words):
         name = "_".join(words)
```

### Comparing `topic_wizard-0.3.0/topicwizard/prepare/utils.py` & `topic_wizard-0.3.1/topicwizard/prepare/utils.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/topicwizard/prepare/words.py` & `topic_wizard-0.3.1/topicwizard/prepare/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.0/setup.py` & `topic_wizard-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 packages = \
 ['topicwizard',
  'topicwizard.blueprints',
  'topicwizard.compatibility',
  'topicwizard.components',
  'topicwizard.components.documents',
+ 'topicwizard.components.groups',
  'topicwizard.components.topics',
  'topicwizard.components.words',
  'topicwizard.figures',
  'topicwizard.plots',
  'topicwizard.prepare']
 
 package_data = \
@@ -27,17 +28,17 @@
  'scikit-learn>=1.2.0,<1.3.0',
  'scipy>=1.8.0',
  'umap-learn>=0.5.3',
  'wordcloud>=1.8.2.2,<1.9.0.0']
 
 setup_kwargs = {
     'name': 'topic-wizard',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Pretty and opinionated topic model visualization in Python.',
-    'long_description': '<img align="left" width="82" height="82" src="assets/logo.svg">\n\n# topicwizard\n\n<br>\n\nPretty and opinionated topic model visualization in Python.\n\n[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/x-tabdeveloping/topic-wizard/blob/main/examples/basic_usage.ipynb)\n[![PyPI version](https://badge.fury.io/py/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![pip downloads](https://img.shields.io/pypi/dm/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/tweetopic)\n[![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)\n<br>\n\n\n\nhttps://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4\n\n## New in version 0.3.0 🌟 🌟\n\n - Exclude pages, that are not needed :bird:\n - Self-contained interactive figures :gift:\n - Topic name inference is now default behavior and is done implicitly.\n\n\n## Features\n\n-   Investigate complex relations between topics, words and documents\n-   Highly interactive\n-   Automatically infer topic names\n-   Name topics manually\n-   Pretty :art:\n-   Intuitive :cow:\n-   Clean API :candy:\n-   Sklearn, Gensim and BERTopic compatible :nut_and_bolt:\n-   Easy deployment :earth_africa:\n\n## Installation\n\nInstall from PyPI:\n\n```bash\npip install topic-wizard\n```\n\n## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n\n### Step 1:\n\nTrain a scikit-learn compatible topic model.\n(If you want to use non-scikit-learn topic models, check [compatibility](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html))\n\n```python\nfrom sklearn.decomposition import NMF\nfrom sklearn.feature_extraction.text import CountVectorizer\nfrom sklearn.pipeline import make_pipeline\n\n# Create topic pipeline\ntopic_pipeline = make_pipeline(\n    CountVectorizer(),\n    NMF(n_components=10),\n)\n\n# Then fit it on the given texts\ntopic_pipeline.fit(texts)\n```\n\n### Step 2a:\n\nVisualize with the topicwizard webapp :bulb:\n\n```python\nimport topicwizard\n\ntopicwizard.visualize(pipeline=topic_pipeline, corpus=texts)\n```\n\nFrom version 0.3.0 you can also disable pages you do not wish to display thereby sparing a lot of time for yourself:\n\n```python\nimport topicwizard\n\n# A large corpus takes a looong time to compute 2D projections for so\n# so you can speed up preprocessing by disabling it alltogether.\ntopicwizard.visualize(pipeline=topic_pipeline, corpus=texts, exclude_pages=["documents"])\n```\n\n![topics screenshot](assets/screenshot_topics.png)\n![words screenshot](assets/screenshot_words.png)\n![words screenshot](assets/screenshot_words_zoomed.png)\n![documents screenshot](assets/screenshot_documents.png)\n\nOoooor...\n\n### Step 2b:\n\nProduce high quality self-contained HTML plots and create your own dashboards/reports :strawberry:\n\n### Map of words\n\n```python\nfrom topicwizard.figures import word_map\n\nword_map(corpus=texts, pipeline=pipeline)\n```\n\n![word map screenshot](assets/word_map.png)\n\n### Timelines of topic distributions\n\n```python\nfrom topicwizard.figures import document_topic_timeline\n\ndocument_topic_timeline(\n    "Joe Biden takes over presidential office from Donald Trump.",\n    pipeline=pipeline,\n)\n```\n![document timeline](assets/document_topic_timeline.png)\n\n### Wordclouds of your topics :cloud:\n\n```python\nfrom topicwizard.figures import topic_wordclouds\n\ntopic_wordclouds(corpus=texts, pipeline=pipeline)\n```\n\n![wordclouds](assets/topic_wordclouds.png)\n\n### And much more ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n',
+    'long_description': '<img align="left" width="82" height="82" src="assets/logo.svg">\n\n# topicwizard\n\n<br>\n\nPretty and opinionated topic model visualization in Python.\n\n[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/x-tabdeveloping/topic-wizard/blob/main/examples/basic_usage.ipynb)\n[![PyPI version](https://badge.fury.io/py/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![pip downloads](https://img.shields.io/pypi/dm/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/tweetopic)\n[![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)\n<br>\n\n\n\nhttps://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4\n\n## New in version 0.3.1 🌟 🌟\n\n- You can now investigate relations of pre-existing labels to your topics and words :mag:\n\n## New in version 0.3.0 🌟 \n\n - Exclude pages, that are not needed :bird:\n - Self-contained interactive figures :gift:\n - Topic name inference is now default behavior and is done implicitly.\n\n\n## Features\n\n-   Investigate complex relations between topics, words, documents and groups/genres/labels\n-   Sklearn, Gensim and BERTopic compatible :nut_and_bolt:\n-   Highly interactive web app\n-   Interactive and composable Plotly figures\n-   Automatically infer topic names, oooor...\n-   Name topics manually\n-   Easy deployment :earth_africa:\n\n## Installation\n\nInstall from PyPI:\n\n```bash\npip install topic-wizard\n```\n\n## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n\n### Step 0:\n\nHave a corpus ready for analysis, in this example I am going to use 20 newgroups from scikit-learn.\n\n```python\nfrom sklearn.datasets import fetch_20newsgroups\n\nnewsgroups = fetch_20newsgroups(subset="all")\ncorpus = newsgroups.data\n\n# Sklearn gives the labels back as integers, we have to map them back to\n# the actual textual label.\ngroup_labels = [newsgroups.target_names[label] for label in newsgroups.target]\n```\n\n### Step 1:\n\nTrain a scikit-learn compatible topic model.\n(If you want to use non-scikit-learn topic models, check [compatibility](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html))\n\n```python\nfrom sklearn.decomposition import NMF\nfrom sklearn.feature_extraction.text import CountVectorizer\nfrom sklearn.pipeline import make_pipeline\n\n# Create topic pipeline\npipeline = make_pipeline(\n    CountVectorizer(stop_words="english", min_df=10),\n    NMF(n_components=30),\n)\n\n# Then fit it on the given texts\npipeline.fit(corpus)\n```\n\n### Step 2a:\n\nVisualize with the topicwizard webapp :bulb:\n\n```python\nimport topicwizard\n\ntopicwizard.visualize(corpus, pipeline=pipeline)\n```\n\nFrom version 0.3.0 you can also disable pages you do not wish to display thereby sparing a lot of time for yourself:\n\n```python\n# A large corpus takes a looong time to compute 2D projections for so\n# so you can speed up preprocessing by disabling it alltogether.\ntopicwizard.visualize(corpus, pipeline=pipeline, exclude_pages=["documents"])\n```\n\n\n![topics screenshot](assets/screenshot_topics.png)\n![words screenshot](assets/screenshot_words.png)\n![words screenshot](assets/screenshot_words_zoomed.png)\n![documents screenshot](assets/screenshot_documents.png)\n\nFrom version 0.3.1 you can investigate groups/labels by passing them along to the webapp.\n\n```python\ntopicwizard.visualize(corpus, pipeline=pipeline, group_labels=group_labels)\n```\n\n![groups screenshot](docs/_static/screenshot_groups.png)\n\nOoooor...\n\n### Step 2b:\n\nProduce high quality self-contained HTML plots and create your own dashboards/reports :strawberry:\n\n### Map of words\n\n```python\nfrom topicwizard.figures import word_map\n\nword_map(corpus, pipeline=pipeline)\n```\n\n![word map screenshot](assets/word_map.png)\n\n### Timelines of topic distributions\n\n```python\nfrom topicwizard.figures import document_topic_timeline\n\ndocument_topic_timeline(\n    "Joe Biden takes over presidential office from Donald Trump.",\n    pipeline=pipeline,\n)\n```\n![document timeline](assets/document_topic_timeline.png)\n\n### Wordclouds of your topics :cloud:\n\n```python\nfrom topicwizard.figures import topic_wordclouds\n\ntopic_wordclouds(corpus, pipeline=pipeline)\n```\n\n![wordclouds](assets/topic_wordclouds.png)\n\n#### And much more... ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n',
     'author': 'Márton Kardos',
     'author_email': 'power.up1163@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `topic_wizard-0.3.0/PKG-INFO` & `topic_wizard-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topic-wizard
-Version: 0.3.0
+Version: 0.3.1
 Summary: Pretty and opinionated topic model visualization in Python.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,100 +40,124 @@
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 
 
 
 https://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4
 
-## New in version 0.3.0 🌟 🌟
+## New in version 0.3.1 🌟 🌟
+
+- You can now investigate relations of pre-existing labels to your topics and words :mag:
+
+## New in version 0.3.0 🌟 
 
  - Exclude pages, that are not needed :bird:
  - Self-contained interactive figures :gift:
  - Topic name inference is now default behavior and is done implicitly.
 
 
 ## Features
 
--   Investigate complex relations between topics, words and documents
--   Highly interactive
--   Automatically infer topic names
--   Name topics manually
--   Pretty :art:
--   Intuitive :cow:
--   Clean API :candy:
+-   Investigate complex relations between topics, words, documents and groups/genres/labels
 -   Sklearn, Gensim and BERTopic compatible :nut_and_bolt:
+-   Highly interactive web app
+-   Interactive and composable Plotly figures
+-   Automatically infer topic names, oooor...
+-   Name topics manually
 -   Easy deployment :earth_africa:
 
 ## Installation
 
 Install from PyPI:
 
 ```bash
 pip install topic-wizard
 ```
 
 ## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))
 
+### Step 0:
+
+Have a corpus ready for analysis, in this example I am going to use 20 newgroups from scikit-learn.
+
+```python
+from sklearn.datasets import fetch_20newsgroups
+
+newsgroups = fetch_20newsgroups(subset="all")
+corpus = newsgroups.data
+
+# Sklearn gives the labels back as integers, we have to map them back to
+# the actual textual label.
+group_labels = [newsgroups.target_names[label] for label in newsgroups.target]
+```
+
 ### Step 1:
 
 Train a scikit-learn compatible topic model.
 (If you want to use non-scikit-learn topic models, check [compatibility](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html))
 
 ```python
 from sklearn.decomposition import NMF
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.pipeline import make_pipeline
 
 # Create topic pipeline
-topic_pipeline = make_pipeline(
-    CountVectorizer(),
-    NMF(n_components=10),
+pipeline = make_pipeline(
+    CountVectorizer(stop_words="english", min_df=10),
+    NMF(n_components=30),
 )
 
 # Then fit it on the given texts
-topic_pipeline.fit(texts)
+pipeline.fit(corpus)
 ```
 
 ### Step 2a:
 
 Visualize with the topicwizard webapp :bulb:
 
 ```python
 import topicwizard
 
-topicwizard.visualize(pipeline=topic_pipeline, corpus=texts)
+topicwizard.visualize(corpus, pipeline=pipeline)
 ```
 
 From version 0.3.0 you can also disable pages you do not wish to display thereby sparing a lot of time for yourself:
 
 ```python
-import topicwizard
-
 # A large corpus takes a looong time to compute 2D projections for so
 # so you can speed up preprocessing by disabling it alltogether.
-topicwizard.visualize(pipeline=topic_pipeline, corpus=texts, exclude_pages=["documents"])
+topicwizard.visualize(corpus, pipeline=pipeline, exclude_pages=["documents"])
 ```
 
+
 ![topics screenshot](assets/screenshot_topics.png)
 ![words screenshot](assets/screenshot_words.png)
 ![words screenshot](assets/screenshot_words_zoomed.png)
 ![documents screenshot](assets/screenshot_documents.png)
 
+From version 0.3.1 you can investigate groups/labels by passing them along to the webapp.
+
+```python
+topicwizard.visualize(corpus, pipeline=pipeline, group_labels=group_labels)
+```
+
+![groups screenshot](docs/_static/screenshot_groups.png)
+
 Ooooor...
 
 ### Step 2b:
 
 Produce high quality self-contained HTML plots and create your own dashboards/reports :strawberry:
 
 ### Map of words
 
 ```python
 from topicwizard.figures import word_map
 
-word_map(corpus=texts, pipeline=pipeline)
+word_map(corpus, pipeline=pipeline)
 ```
 
 ![word map screenshot](assets/word_map.png)
 
 ### Timelines of topic distributions
 
 ```python
@@ -147,14 +171,14 @@
 ![document timeline](assets/document_topic_timeline.png)
 
 ### Wordclouds of your topics :cloud:
 
 ```python
 from topicwizard.figures import topic_wordclouds
 
-topic_wordclouds(corpus=texts, pipeline=pipeline)
+topic_wordclouds(corpus, pipeline=pipeline)
 ```
 
 ![wordclouds](assets/topic_wordclouds.png)
 
-### And much more ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))
+#### And much more... ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))
```

