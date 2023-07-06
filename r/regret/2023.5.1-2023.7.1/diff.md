# Comparing `tmp/regret-2023.5.1.tar.gz` & `tmp/regret-2023.7.1.tar.gz`

## Comparing `regret-2023.5.1.tar` & `regret-2023.7.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 regret-2023.5.1/.flake8
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 regret-2023.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 regret-2023.5.1/.readthedocs.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 regret-2023.5.1/.testr.conf
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 regret-2023.5.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 regret-2023.5.1/MANIFEST.in
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 regret-2023.5.1/noxfile.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 regret-2023.5.1/test-requirements.in
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 regret-2023.5.1/test-requirements.txt
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 regret-2023.5.1/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 regret-2023.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 regret-2023.5.1/.github/release.yml
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 regret-2023.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/Makefile
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/before-you-deprecate.rst
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/compatibility.rst
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/conf.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/index.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/requirements.in
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/requirements.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/what-you-can-deprecate.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/api/modules.rst
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/api/regret.rst
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/__init__.py
--rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/_api.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/_inspect.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/_sphinx.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/_warnings.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/emitted.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/testing.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/tests/__init__.py
--rw-r--r--   0        0        0    62906 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/tests/test_api.py
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/tests/test_integration.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/tests/test_testing.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 regret-2023.5.1/COPYING
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 regret-2023.5.1/README.rst
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 regret-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 regret-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 regret-2023.7.1/.flake8
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 regret-2023.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 regret-2023.7.1/.readthedocs.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 regret-2023.7.1/.testr.conf
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 regret-2023.7.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 regret-2023.7.1/MANIFEST.in
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 regret-2023.7.1/noxfile.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 regret-2023.7.1/test-requirements.in
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 regret-2023.7.1/test-requirements.txt
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 regret-2023.7.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 regret-2023.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 regret-2023.7.1/.github/release.yml
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 regret-2023.7.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/Makefile
+-rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/before-you-deprecate.rst
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/compatibility.rst
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/conf.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/index.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/requirements.in
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/requirements.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/what-you-can-deprecate.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/api/modules.rst
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 regret-2023.7.1/docs/api/regret.rst
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/__init__.py
+-rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/_api.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/_inspect.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/_sphinx.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/_warnings.py
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/emitted.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/testing.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/tests/__init__.py
+-rw-r--r--   0        0        0    62906 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/tests/test_api.py
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/tests/test_integration.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 regret-2023.7.1/regret/tests/test_testing.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 regret-2023.7.1/COPYING
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 regret-2023.7.1/README.rst
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 regret-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 regret-2023.7.1/PKG-INFO
```

### Comparing `regret-2023.5.1/.pre-commit-config.yaml` & `regret-2023.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/CONTRIBUTING.rst` & `regret-2023.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/noxfile.py` & `regret-2023.7.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/test-requirements.txt` & `regret-2023.7.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/.github/SECURITY.md` & `regret-2023.7.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/.github/workflows/ci.yml` & `regret-2023.7.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/docs/Makefile` & `regret-2023.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/docs/before-you-deprecate.rst` & `regret-2023.7.1/docs/before-you-deprecate.rst`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,16 @@
       Or is your use of ``attrs`` as a library maintainer simply an implementation detail?
 
     * a function in your library calls `requests.get`, a function which has mutable global state -- it allows someone to import the library and e.g. define `Transport Adapters <requests:transport-adapters>` which, even if done outside your library, affect how it will retrieve the HTTP response.
       Is your library free to change its HTTP client to another HTTP client even though this will potentially disrupt users who expect their external change to have an effect on your library's behavior?
 
     * your package depends on ``foo>1.2.3``. Are these pins part of your public API, and bumping the lower-pinned version of ``foo`` a breaking change? Doing so may of course affect users who are using ``foo==1.2.3`` alongside another of their own dependencies.
 
+    * today, your package has no binary (non-Python) dependencies. Is that a permanent promise of its installation "API"?
+
     * ...
 
 There are many many more.
 Think of things that you, a maintainer, rely on from libraries *you* use, and how many subtleties you wish were clearer.
 
 To be clear, some of the above *do* have commonly understood answers in the ecosystem -- but even beyond resolving the final bits of doubt, there may still be a lot to gain from explicitly confirming each has been considered in the course of changes made to the package.
```

### Comparing `regret-2023.5.1/docs/compatibility.rst` & `regret-2023.7.1/docs/compatibility.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/docs/conf.py` & `regret-2023.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/docs/requirements.txt` & `regret-2023.7.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/docs/what-you-can-deprecate.rst` & `regret-2023.7.1/docs/what-you-can-deprecate.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/docs/api/regret.rst` & `regret-2023.7.1/docs/api/regret.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/regret/_api.py` & `regret-2023.7.1/regret/_api.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/regret/_inspect.py` & `regret-2023.7.1/regret/_inspect.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/regret/_sphinx.py` & `regret-2023.7.1/regret/_sphinx.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/regret/emitted.py` & `regret-2023.7.1/regret/emitted.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/regret/testing.py` & `regret-2023.7.1/regret/testing.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/regret/typing.py` & `regret-2023.7.1/regret/typing.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/regret/tests/test_api.py` & `regret-2023.7.1/regret/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/regret/tests/test_integration.py` & `regret-2023.7.1/regret/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/regret/tests/test_testing.py` & `regret-2023.7.1/regret/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/COPYING` & `regret-2023.7.1/COPYING`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/README.rst` & `regret-2023.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.5.1/pyproject.toml` & `regret-2023.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -101,11 +101,7 @@
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.ruff.per-file-ignores]
 "docs/*" = ["ANN", "D"]
 "regret/tests/*" = ["ANN", "D"]
 "noxfile.py" = ["ANN", "D"]
-
-[tool.ruff.pyupgrade]
-# We support 3.8 + 3.9
-keep-runtime-typing = true
```

### Comparing `regret-2023.5.1/PKG-INFO` & `regret-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regret
-Version: 2023.5.1
+Version: 2023.7.1
 Summary: You made a thing, but now you wish it'd go away... Deprecations, a love story.
 Project-URL: Documentation, https://regret.readthedocs.io/
 Project-URL: Homepage, https://github.com/Julian/regret
 Project-URL: Issues, https://github.com/Julian/regret/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/Julian/regret
 Author: Julian Berman
```

