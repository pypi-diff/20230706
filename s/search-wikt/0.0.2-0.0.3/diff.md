# Comparing `tmp/search_wikt-0.0.2.tar.gz` & `tmp/search_wikt-0.0.3.tar.gz`

## Comparing `search_wikt-0.0.2.tar` & `search_wikt-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 search_wikt-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 search_wikt-0.0.2/src/search_wikt/__init__.py
--rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 search_wikt-0.0.2/src/search_wikt/core.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 search_wikt-0.0.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 search_wikt-0.0.2/LICENSE
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 search_wikt-0.0.2/README.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 search_wikt-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 search_wikt-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 search_wikt-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 search_wikt-0.0.3/src/search_wikt/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 search_wikt-0.0.3/src/search_wikt/__main__.py
+-rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 search_wikt-0.0.3/src/search_wikt/core.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 search_wikt-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 search_wikt-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 search_wikt-0.0.3/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 search_wikt-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 search_wikt-0.0.3/PKG-INFO
```

### Comparing `search_wikt-0.0.2/src/search_wikt/core.py` & `search_wikt-0.0.3/src/search_wikt/core.py`

 * *Files identical despite different names*

### Comparing `search_wikt-0.0.2/LICENSE` & `search_wikt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `search_wikt-0.0.2/README.md` & `search_wikt-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,85 @@
-### Search Wiktionary
-
-A simple command-line tool for searching English Wiktionary using Wiktionary Parser ([click](https://github.com/Suyash458/WiktionaryParser)).
-
-Wiktionary definitions are licensed under CC BY-SA 4.0. Visit wiktionary at wiktionary.org ([click](wiktionary.org)).
-
-#### Installation
-To install, run:
-```
-pip install search_wikt
-```
-Or, to clone the repository run:
-```
-git clone https://github.com/lauramvx/search_wikt
-```
-##### Examples
-```
-py src\search_wikt\core.py hunig -l "Old English"
-```
-
-```
-hunig
-From Proto-West Germanic *hunag, from Proto-Germanic *hunagą. Cognate with Old Frisian hunig, Old Saxon honeg, and Old High German honag; also Old Norse hunang, from the alternative form *hunangą.
-
-IPA: /ˈxu.nij/, [ˈhu.nij]
-noun
-huniġ n
-honey
-```
-```
-py src\search_wikt\core.py ac -l "Old English" -ex -r
-```
-```
-ac 1
-From Proto-Germanic *aiks.
-
-IPA: /ɑːk/
-IPA: /ɑk/
-noun
-āc f
-oak (wood or tree)
-(poetic) an oaken ship
-(masculine) the runic character ᚪ (/a/)
-ac 2
-From Proto-Germanic *ak.
-
-IPA: /ɑːk/
-IPA: /ɑk/
-conjunction
-ac
-but
-but instead: in this sense ac should sometimes be translated as "but," but most often it is best left untranslated
-
-
-Sēo æx forġiett, ac þæt trēow ġeman.The axe forgets, but  the tree remembers.
-The axe forgets, but  the tree remembers.
-Ne ġēotaþ wē tēaras, ac blōd.We don't shed tears, we shed blood.
-We don't shed tears, we shed blood.
-Nōn egō, sed tū: “Nā iċ, ac þū.” Nōn bōs est, sed equus: “Nis hit nā oxa, ac is hors.”Non ego, sed tu: “Not me, you.” Non bos est, sed equus: “It's not an ox, it's a horse.”
-Non ego, sed tu: “Not me, you.” Non bos est, sed equus: “It's not an ox, it's a horse.”
-```
+Metadata-Version: 2.1
+Name: search_wikt
+Version: 0.0.3
+Summary: A simple command-line tool for searching Wiktionary.
+Author-email: lauramvx <lesbianhouse@gmx.com>
+License-File: LICENSE
+Keywords: CLI,Wiktionary,dictionary,etymology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: wiktionaryparser==0.0.97
+Description-Content-Type: text/markdown
+
+### Search Wiktionary
+
+A simple command-line tool for searching English Wiktionary using Wiktionary Parser ([click](https://github.com/Suyash458/WiktionaryParser)).
+
+Wiktionary definitions are licensed under CC BY-SA 4.0. Visit wiktionary at wiktionary.org ([click](wiktionary.org)).
+
+#### Installation
+To install, type:
+```
+pip install search_wikt
+```
+To run the program, type:
+```
+py -m search_wikt apricot --language English
+```
+or any other word or language you'd like to search. Run `py -m search_wikt -h` or `--help` for a more detailed explanation.
+
+Alternatively, to clone the repository type:
+```
+git clone https://github.com/lauramvx/search_wikt
+```
+then `cd` to the project directory and run:
+```
+py src\search_wikt\core.py apricot --language English
+```
+##### Examples
+```
+py src\search_wikt\core.py hunig -l "Old English"
+```
+
+```
+hunig
+From Proto-West Germanic *hunag, from Proto-Germanic *hunagą. Cognate with Old Frisian hunig, Old Saxon honeg, and Old High German honag; also Old Norse hunang, from the alternative form *hunangą.
+
+IPA: /ˈxu.nij/, [ˈhu.nij]
+noun
+huniġ n
+honey
+```
+```
+py src\search_wikt\core.py ac -l "Old English" -ex -r
+```
+```
+ac 1
+From Proto-Germanic *aiks.
+
+IPA: /ɑːk/
+IPA: /ɑk/
+noun
+āc f
+oak (wood or tree)
+(poetic) an oaken ship
+(masculine) the runic character ᚪ (/a/)
+ac 2
+From Proto-Germanic *ak.
+
+IPA: /ɑːk/
+IPA: /ɑk/
+conjunction
+ac
+but
+but instead: in this sense ac should sometimes be translated as "but," but most often it is best left untranslated
+
+
+Sēo æx forġiett, ac þæt trēow ġeman.The axe forgets, but  the tree remembers.
+The axe forgets, but  the tree remembers.
+Ne ġēotaþ wē tēaras, ac blōd.We don't shed tears, we shed blood.
+We don't shed tears, we shed blood.
+Nōn egō, sed tū: “Nā iċ, ac þū.” Nōn bōs est, sed equus: “Nis hit nā oxa, ac is hors.”Non ego, sed tu: “Not me, you.” Non bos est, sed equus: “It's not an ox, it's a horse.”
+Non ego, sed tu: “Not me, you.” Non bos est, sed equus: “It's not an ox, it's a horse.”
+```
```

### Comparing `search_wikt-0.0.2/pyproject.toml` & `search_wikt-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "search_wikt"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="lauramvx", email="lesbianhouse@gmx.com" },
 ]
 description = "A simple command-line tool for searching Wiktionary."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `search_wikt-0.0.2/PKG-INFO` & `search_wikt-0.0.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,71 @@
-Metadata-Version: 2.1
-Name: search_wikt
-Version: 0.0.2
-Summary: A simple command-line tool for searching Wiktionary.
-Author-email: lauramvx <lesbianhouse@gmx.com>
-License-File: LICENSE
-Keywords: CLI,Wiktionary,dictionary,etymology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: wiktionaryparser==0.0.97
-Description-Content-Type: text/markdown
-
-### Search Wiktionary
-
-A simple command-line tool for searching English Wiktionary using Wiktionary Parser ([click](https://github.com/Suyash458/WiktionaryParser)).
-
-Wiktionary definitions are licensed under CC BY-SA 4.0. Visit wiktionary at wiktionary.org ([click](wiktionary.org)).
-
-#### Installation
-To install, run:
-```
-pip install search_wikt
-```
-Or, to clone the repository run:
-```
-git clone https://github.com/lauramvx/search_wikt
-```
-##### Examples
-```
-py src\search_wikt\core.py hunig -l "Old English"
-```
-
-```
-hunig
-From Proto-West Germanic *hunag, from Proto-Germanic *hunagą. Cognate with Old Frisian hunig, Old Saxon honeg, and Old High German honag; also Old Norse hunang, from the alternative form *hunangą.
-
-IPA: /ˈxu.nij/, [ˈhu.nij]
-noun
-huniġ n
-honey
-```
-```
-py src\search_wikt\core.py ac -l "Old English" -ex -r
-```
-```
-ac 1
-From Proto-Germanic *aiks.
-
-IPA: /ɑːk/
-IPA: /ɑk/
-noun
-āc f
-oak (wood or tree)
-(poetic) an oaken ship
-(masculine) the runic character ᚪ (/a/)
-ac 2
-From Proto-Germanic *ak.
-
-IPA: /ɑːk/
-IPA: /ɑk/
-conjunction
-ac
-but
-but instead: in this sense ac should sometimes be translated as "but," but most often it is best left untranslated
-
-
-Sēo æx forġiett, ac þæt trēow ġeman.The axe forgets, but  the tree remembers.
-The axe forgets, but  the tree remembers.
-Ne ġēotaþ wē tēaras, ac blōd.We don't shed tears, we shed blood.
-We don't shed tears, we shed blood.
-Nōn egō, sed tū: “Nā iċ, ac þū.” Nōn bōs est, sed equus: “Nis hit nā oxa, ac is hors.”Non ego, sed tu: “Not me, you.” Non bos est, sed equus: “It's not an ox, it's a horse.”
-Non ego, sed tu: “Not me, you.” Non bos est, sed equus: “It's not an ox, it's a horse.”
-```
+### Search Wiktionary
+
+A simple command-line tool for searching English Wiktionary using Wiktionary Parser ([click](https://github.com/Suyash458/WiktionaryParser)).
+
+Wiktionary definitions are licensed under CC BY-SA 4.0. Visit wiktionary at wiktionary.org ([click](wiktionary.org)).
+
+#### Installation
+To install, type:
+```
+pip install search_wikt
+```
+To run the program, type:
+```
+py -m search_wikt apricot --language English
+```
+or any other word or language you'd like to search. Run `py -m search_wikt -h` or `--help` for a more detailed explanation.
+
+Alternatively, to clone the repository type:
+```
+git clone https://github.com/lauramvx/search_wikt
+```
+then `cd` to the project directory and run:
+```
+py src\search_wikt\core.py apricot --language English
+```
+##### Examples
+```
+py src\search_wikt\core.py hunig -l "Old English"
+```
+
+```
+hunig
+From Proto-West Germanic *hunag, from Proto-Germanic *hunagą. Cognate with Old Frisian hunig, Old Saxon honeg, and Old High German honag; also Old Norse hunang, from the alternative form *hunangą.
+
+IPA: /ˈxu.nij/, [ˈhu.nij]
+noun
+huniġ n
+honey
+```
+```
+py src\search_wikt\core.py ac -l "Old English" -ex -r
+```
+```
+ac 1
+From Proto-Germanic *aiks.
+
+IPA: /ɑːk/
+IPA: /ɑk/
+noun
+āc f
+oak (wood or tree)
+(poetic) an oaken ship
+(masculine) the runic character ᚪ (/a/)
+ac 2
+From Proto-Germanic *ak.
+
+IPA: /ɑːk/
+IPA: /ɑk/
+conjunction
+ac
+but
+but instead: in this sense ac should sometimes be translated as "but," but most often it is best left untranslated
+
+
+Sēo æx forġiett, ac þæt trēow ġeman.The axe forgets, but  the tree remembers.
+The axe forgets, but  the tree remembers.
+Ne ġēotaþ wē tēaras, ac blōd.We don't shed tears, we shed blood.
+We don't shed tears, we shed blood.
+Nōn egō, sed tū: “Nā iċ, ac þū.” Nōn bōs est, sed equus: “Nis hit nā oxa, ac is hors.”Non ego, sed tu: “Not me, you.” Non bos est, sed equus: “It's not an ox, it's a horse.”
+Non ego, sed tu: “Not me, you.” Non bos est, sed equus: “It's not an ox, it's a horse.”
+```
```

