# Comparing `tmp/blastpipe-0.4.24.tar.gz` & `tmp/blastpipe-0.4.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-0.4.24.tar", last modified: Mon Jun 26 03:54:53 2023, max compression
+gzip compressed data, was "blastpipe-0.4.26.tar", last modified: Thu Jul  6 02:06:59 2023, max compression
```

## Comparing `blastpipe-0.4.24.tar` & `blastpipe-0.4.26.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.533516 blastpipe-0.4.24/
--rw-rw-r--   0 ross      (1000) ross      (1000)     3723 2023-06-26 03:54:53.000000 blastpipe-0.4.24/.gitignore
--rw-rw-r--   0 ross      (1000) ross      (1000)       56 2023-06-26 03:54:53.000000 blastpipe-0.4.24/.markdownlint.json
--rw-rw-r--   0 ross      (1000) ross      (1000)    12252 2023-06-26 03:54:53.000000 blastpipe-0.4.24/CHANGELOG.md
--rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-06-26 03:54:53.000000 blastpipe-0.4.24/LICENSE.txt
--rw-rw-r--   0 ross      (1000) ross      (1000)     4612 2023-06-26 03:54:53.000000 blastpipe-0.4.24/NOTICE.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     5099 2023-06-26 03:54:53.000000 blastpipe-0.4.24/PKG-INFO
--rw-rw-r--   0 ross      (1000) ross      (1000)     4206 2023-06-26 03:54:53.000000 blastpipe-0.4.24/README.rst
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/
--rw-rw-r--   0 ross      (1000) ross      (1000)     1629 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/__init__.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3234 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/backports.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1811 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/buffer.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1666 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/loop.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     2867 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/malloc.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      971 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     1351 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/mixin.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1808 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/sequence.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1408 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/tailcall.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3043 2023-06-26 03:54:53.000000 blastpipe-0.4.24/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     5580 2023-06-26 03:54:53.000000 blastpipe-0.4.24/meson.options
--rw-rw-r--   0 ross      (1000) ross      (1000)    11676 2023-06-26 03:54:53.000000 blastpipe-0.4.24/pyproject.toml
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/
--rw-rw-r--   0 ross      (1000) ross      (1000)      739 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/dev.wrap
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/
--rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/css/
--rw-rw-r--   0 ross      (1000) ross      (1000)      767 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 ross      (1000) ross      (1000)      693 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)      633 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_templates/
--rw-rw-r--   0 ross      (1000) ross      (1000)     1033 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 ross      (1000) ross      (1000)      694 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)      860 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/conf.cfg
--rw-rw-r--   0 ross      (1000) ross      (1000)     1751 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/index.rst
--rw-rw-r--   0 ross      (1000) ross      (1000)     2680 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     2058 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/meson.options
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/
--rw-rw-r--   0 ross      (1000) ross      (1000)     2350 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     1173 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/test_backports.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     2503 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/test_fuzz.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1689 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/test_tailcall.py
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.674680 blastpipe-0.4.26/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3723 2023-07-06 02:06:59.000000 blastpipe-0.4.26/.gitignore
+-rw-rw-r--   0 ross      (1000) ross      (1000)       56 2023-07-06 02:06:59.000000 blastpipe-0.4.26/.markdownlint.json
+-rw-rw-r--   0 ross      (1000) ross      (1000)    13270 2023-07-06 02:06:59.000000 blastpipe-0.4.26/CHANGELOG.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-07-06 02:06:59.000000 blastpipe-0.4.26/LICENSE.txt
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4612 2023-07-06 02:06:59.000000 blastpipe-0.4.26/NOTICE.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     6925 2023-07-06 02:06:59.000000 blastpipe-0.4.26/PKG-INFO
+-rw-rw-r--   0 ross      (1000) ross      (1000)     6032 2023-07-06 02:06:59.000000 blastpipe-0.4.26/README.rst
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1629 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/__init__.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3234 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/backports.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1811 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/buffer.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1666 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/loop.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2867 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/malloc.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      971 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1351 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/mixin.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1808 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/sequence.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1408 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/tailcall.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2987 2023-07-06 02:06:59.000000 blastpipe-0.4.26/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     5543 2023-07-06 02:06:59.000000 blastpipe-0.4.26/meson.options
+-rw-rw-r--   0 ross      (1000) ross      (1000)    13364 2023-07-06 02:06:59.000000 blastpipe-0.4.26/pyproject.toml
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/
+-rw-rw-r--   0 ross      (1000) ross      (1000)      739 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/dev.wrap
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/css/
+-rw-rw-r--   0 ross      (1000) ross      (1000)      767 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 ross      (1000) ross      (1000)      693 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)      633 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_templates/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1033 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 ross      (1000) ross      (1000)      694 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)      860 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/conf.cfg
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1751 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/index.rst
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2680 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2058 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/meson.options
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2350 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1173 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/test_backports.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2503 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/test_fuzz.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1689 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/test_tailcall.py
```

### Comparing `blastpipe-0.4.24/.gitignore` & `blastpipe-0.4.26/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/CHANGELOG.md` & `blastpipe-0.4.26/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -13,42 +13,42 @@
    specific language governing permissions and limitations
    under the License. -->
 
 # Changelog
 
 <!--next-version-placeholder-->
 
-## v0.4.23 (2023-06-24)
-### Other
-* PKG-INFO Updated ([`f80b3da`](https://github.com/rjdbcm/blastpipe/commit/f80b3da157f4a083922832e621b949a477238972))
-
-## v0.4.21 (2023-06-23)
-### Other
-* PKG-INFO Updated ([`5c84048`](https://github.com/rjdbcm/blastpipe/commit/5c840485844fabc70b91c5be67d7b60ab4b864b0))
+## v0.4.25 (2023-07-05)
 
-## v0.4.6 (2023-06-21)
+### Fix
 
+* :pencil2:(pyproject.toml): defer sphinxawesome-theme to ozi. ([`b1e144d`](https://github.com/rjdbcm/blastpipe/commit/b1e144d050f04f3887b1d64ac6a4f7454585792a))
+* :pencil2:(README.rst): use blastpipe badge not OZI. ([`7a71e70`](https://github.com/rjdbcm/blastpipe/commit/7a71e70618441555406c574633e49b5e842309c8))
 
-## v0.4.5 (2023-06-21)
 ### Other
-* Don't stash wheel bump. ([`a9ca7d8`](https://github.com/rjdbcm/blastpipe/commit/a9ca7d8171535ce0e29ed08874bc674a048d8e6b))
-
-## v0.3.15 (2023-06-21)
 
+* 🔨(meson.build): enable subprojects/docs ([`0cd6483`](https://github.com/rjdbcm/blastpipe/commit/0cd6483a734fa6cc8a973faacaafec163f5d2a8f))
+* 📝(README.rst): Add Contributing info. ([`96fec96`](https://github.com/rjdbcm/blastpipe/commit/96fec96befae2e886e7125c528b5a48a3b18019f))
+* 👷semantic-release: pre_commit tox. ([`61b9362`](https://github.com/rjdbcm/blastpipe/commit/61b93629158e16697479312d91382d8e1b9c32ee))
+* 🔇(CHANGELOG.md): Clean up version tags. ([`a3a50e2`](https://github.com/rjdbcm/blastpipe/commit/a3a50e2ae6826c1e57641a0d54ee0d69d229e7fe))
+* PKG-INFO Updated ([`cf7cd18`](https://github.com/rjdbcm/blastpipe/commit/cf7cd18ea0aaed5182ad547b80efe791f2825967))
 
-## v0.3.7 (2023-06-20)
-
-
-## v0.3.6 (2023-06-20)
-
-
-## v0.3.5 (2023-06-20)
+## v0.4.24 (2023-06-25)
+### Other
+* 🔨(semantic-release): git clean -dfX pre_commit. ([`230bb86`](https://github.com/rjdbcm/blastpipe/commit/230bb86a3e1899136fa7d1b854ccb12a0c986ca2))
+* 🔊 Add 0.4.23 changes. CHANGELOG.md should actually get release notes from now on. ([`cdefd70`](https://github.com/rjdbcm/blastpipe/commit/cdefd70c105036b5c43a7588a2f47ecad9316a55))
+* PKG-INFO Updated ([`55177f6`](https://github.com/rjdbcm/blastpipe/commit/55177f626333cf0322f0d89f0ff715f7cad10180))
 
+## v0.4.23 (2023-06-24)
+### Other
+* PKG-INFO Updated ([`f80b3da`](https://github.com/rjdbcm/blastpipe/commit/f80b3da157f4a083922832e621b949a477238972))
 
-## v0.3.4 (2023-06-20)
+## v0.4.21 (2023-06-23)
+### Other
+* PKG-INFO Updated ([`5c84048`](https://github.com/rjdbcm/blastpipe/commit/5c840485844fabc70b91c5be67d7b60ab4b864b0))
 
 ## v0.3.3 (2023-06-20)
 ### Other
 * 👷 add dist/*tar.gz to release. ([`c98d198`](https://github.com/rjdbcm/blastpipe/commit/c98d198ea350f35d46085927525daf157d8e36ea))
 * 👷 build wheel and sdist. ([`ec543a4`](https://github.com/rjdbcm/blastpipe/commit/ec543a4ed82ece555f7013b1ef0932fe4cb664d6))
 
 ## v0.3.2 (2023-06-20)
@@ -89,17 +89,14 @@
 ### Other
 * Changes to release. ([`fd26a79`](https://github.com/rjdbcm/blastpipe/commit/fd26a79002be80fe8ee150950bd761f03a109d2a))
 
 ## v0.2.0 (2023-06-19)
 ### Other
 * Changelogged ([`af1cd00`](https://github.com/rjdbcm/blastpipe/commit/af1cd0033c9fbe0385c237de315cb4d52f866a60))
 
-## v0.1.2 (2023-06-19)
-
-
 ## v0.1.1 (2023-06-19)
 ### Other
 * 🚨 lint for release test. ([`a292ad7`](https://github.com/rjdbcm/blastpipe/commit/a292ad70d4d5c9bf43e5d079558ddaba0b7a837b))
 * 🚀 add testpypi and github artifact upload ([`4594834`](https://github.com/rjdbcm/blastpipe/commit/4594834abfd840168e1a6e65b6ef6d4164030065))
 * 👷 add meson test and dist steps to semantic-release. ([`c2230dc`](https://github.com/rjdbcm/blastpipe/commit/c2230dc994177874aeaab8944fc1611d2930a9ec))
 * 🧑‍💻 __init__.py now supplies __version__. Uses the version from importlib.metadata. ([`46705b7`](https://github.com/rjdbcm/blastpipe/commit/46705b7e6090dc897f198868a3527d19064f19d4))
 * 🔨  scm_version updates. Meson writes fallback version and project name to pyproject.toml at dist time. ([`1c7ccc8`](https://github.com/rjdbcm/blastpipe/commit/1c7ccc87500c3b2def2fd19e128f7b996201ea88))
@@ -166,24 +163,7 @@
 * Added sequence.chr_union() ([`ec1a137`](https://github.com/rjdbcm/blastpipe/commit/ec1a137bd21baf454591d59ff67e52aaed8beee3))
 * Init ([`6a541a2`](https://github.com/rjdbcm/blastpipe/commit/6a541a2c6f9aea0fe16b55fdf8d5c3ee8198116b))
 
 ## v2023.6.0 (2023-05-06)
 
 * Switched to Meson build system
 * No longer hard coding the version
-
-## v2023.1.6 (2023-01-28)
-
-
-## v2023.1.5 (2023-01-28)
-
-
-## v2023.1.4 (2023-01-27)
-
-
-## v2023.2.0-beta.1 (2023-01-27)
-
-
-## v2023.1.4-beta.1 (2023-01-27)
-
-
-## v2023.1.4-beta.1 (2023-01-27)
```

### Comparing `blastpipe-0.4.24/LICENSE.txt` & `blastpipe-0.4.26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/NOTICE.md` & `blastpipe-0.4.26/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/PKG-INFO` & `blastpipe-0.4.26/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: blastpipe
-Version: 0.4.24
-Summary: Packaged with OZI.
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Homepage, https://github.com/rjdbcm/blastpipe
-Project-URL: Download, https://github.com/rjdbcm/blastpipe/archive/refs/heads/main.zip
-Description-Content-Type: text/x-rst
-
 .. Copyright 2023 Ross J. Duff MSc 
    The copyright holder licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at
 
       http://www.apache.org/licenses/LICENSE-2.0
@@ -33,26 +13,61 @@
    specific language governing permissions and limitations
    under the License.
 
 =========
 blastpipe
 =========
 
-|py-version-badge| |slsa-level3-badge| |semantic-release-badge|
+|py-version-badge| |openssf-badge| |slsa-level3-badge| |fossa-badge| |semantic-release-badge|
 |coverage-badge| |pytest-plugins-badge| 
 |bandit-badge| |black-badge| |isort-badge| |flake8-badge| |pyright-badge| |pylint-ckpt-badge| |rst-lint-badge|
 
 A simple utility library used as a slice demonstration for using
 Meson+OZI as Python 3 packaging management layer.
 
 .. image:: https://raw.githubusercontent.com/sigstore/community/main/artwork/badge/sigstore_codesigned_purple.png
  :align: right
  :height: 140
  :target: https://www.sigstore.dev/
 
+Contributing
+^^^^^^^^^^^^
+
+Contributions are what make the open source community such an amazing place to
+learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and
+create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the repository
+2. Create your Feature Branch (``git checkout -b feature/AmazingFeature``)
+3. Commit your Changes (``git commit -m 'Add some AmazingFeature'``)
+4. Push to the Branch (``git push origin feature/AmazingFeature``)
+5. Open a Pull Request
+
+Bug Reports
+^^^^^^^^^^^
+
+1. Create an issue with the tag "bug" with a descriptive title stating the issue succinctly.
+2. Fill out the issue template with the information requested.
+
+If you have any proposed changes related to a bug, if an Issue has not been created please
+complete the above instructions.
+The next steps are similar to the steps needed to create a feature pull request.
+
+Submitting a Fix
+################
+
+1. Fork the repository
+2. Create your Bugfix Branch (``git checkout -b bugfix/Issue#``)
+3. Commit your Changes (``git commit -m '🐛: Fix Issue#'``)
+4. Push to the Branch (``git push origin bugfix/Issue#``)
+5. Open a Pull Request
+
 License
 ^^^^^^^
 
 blastpipe is released under the terms of the 2.0 version of the Apache License,
 approved by the Apache Software Foundation. blastpipe meets the Open Source Initiative's definition of
 open source software, and the Free Software Foundation's definition of GPLv3-compatible open 
 source software.
@@ -87,15 +102,20 @@
  :target: https://www.gnu.org/
 
 
 
 .. |py-version-badge| image:: https://img.shields.io/badge/Python%20Version-3.9%20%7C%203.10%20%7C%203.11-blue
 .. |pylint-ckpt-badge| image:: https://img.shields.io/badge/linting-%E2%9C%94%20Pylint%3A%2010.00%2F10-informational
 .. |slsa-level3-badge| image:: https://slsa.dev/images/gh-badge-level3.svg
-
+.. |fossa-badge| image:: https://app.fossa.com/api/projects/git%2Bgithub.com%2Frjdbcm%2Fblastpipe.svg?type=shield
+    :target: https://app.fossa.com/projects/git%2Bgithub.com%2Frjdbcm%2Fblastpipe?ref=badge_large
+    :alt: License Compliance
+.. |openssf-badge| image:: https://bestpractices.coreinfrastructure.org/projects/7515/badge
+    :target: https://bestpractices.coreinfrastructure.org/projects/7515
+    :alt: Open Source Security Foundation self-certification status
 .. |semantic-release-badge| image:: https://img.shields.io/badge/semantic--release-gitmoji-e10079?logo=semantic-release
     :target: https://github.com/python-semantic-release/python-semantic-release
     :alt: Automatic Semantic Versioning for Python projects
 .. |bandit-badge| image:: https://img.shields.io/badge/security-%E2%9C%94%20bandit-yellow.svg
     :target: https://github.com/PyCQA/bandit
     :alt: Security Status
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-%E2%9C%94%20black-000000.svg
@@ -103,8 +123,7 @@
 .. |coverage-badge| image:: https://img.shields.io/badge/Coverage.py-%E2%9C%94%20100%25-success
 .. |flake8-badge| image:: https://img.shields.io/badge/code%20quality-%E2%9C%94%20Flake8-informational
 .. |isort-badge| image:: https://img.shields.io/badge/%20imports-%E2%9C%94%20isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 .. |pyright-badge| image:: https://img.shields.io/badge/typing-%E2%9C%94%20Pyright%3A%200%20e%2C%200%20w%2C%200%20i-informational
 .. |pytest-plugins-badge| image:: https://img.shields.io/badge/Pytest-asyncio%20cov%20%20hypothesis%20mock%20randomly%20tcpclient-informational
 .. |rst-lint-badge| image:: https://img.shields.io/badge/rst--lint-%E2%9C%94%20README.rst-informational
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `blastpipe-0.4.24/blastpipe/__init__.py` & `blastpipe-0.4.26/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/blastpipe/backports.py` & `blastpipe-0.4.26/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/blastpipe/buffer.py` & `blastpipe-0.4.26/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/blastpipe/loop.py` & `blastpipe-0.4.26/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/blastpipe/malloc.py` & `blastpipe-0.4.26/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/blastpipe/meson.build` & `blastpipe-0.4.26/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/blastpipe/mixin.py` & `blastpipe-0.4.26/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/blastpipe/sequence.py` & `blastpipe-0.4.26/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/blastpipe/tailcall.py` & `blastpipe-0.4.26/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/meson.build` & `blastpipe-0.4.26/meson.build`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 stub_files = []
 foreach dir : [project_name, test_source]
  subdir(dir)
 endforeach
 foreach file : python_files
  python.install_sources(file)
 endforeach
-# TODO: documentation build imports are broken for dist
 # docs = subproject('docs')
 # TODO: stub build imports are broken for dist
 # stubs = custom_target('stubs', install: true, install_dir: get_option('prefix'),
 #  output: stub_files,
 #  command: [find_program('pyright', required: true), '--createstub', project_name])
 foreach dir : ['prefix', 'bindir', 'libdir', 'datadir', 'localedir', 'python.install_env', 
                 'python.platlibdir', 'python.purelibdir']
```

### Comparing `blastpipe-0.4.24/meson.options` & `blastpipe-0.4.26/meson.options`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     description: 'application', type: 'array', 
     value: ['--version'])
 option('args-semantic-release',
     description: 'application', type: 'array', 
     value: ['version', '--noop', '--verbosity=debug'])
 option('args-doc8',
     description: 'application', type: 'array', 
-    value: ['--config', 'pyproject.toml', '@docs_source@'])
+    value: ['--help'])
 option('args-pydocstyle',
     description: 'application', type: 'array', 
     value: ['-v', '-d', '--config=pyproject.toml', '@docs_source@'])
 option('args-sphinx-build',
     description: 'application', type: 'array', 
     value: ['--help'])
 option('args-flake8p', type: 'array',
```

### Comparing `blastpipe-0.4.24/pyproject.toml` & `blastpipe-0.4.26/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 [project.optional_dependencies] # also OZI meson test suite names
 # Default OZI test setup
 dev  = ["[dist,docs,lint,test]"]
 ## Packaging Setup
 dist = ["pyc_wheel", "python-semantic-release", "sigstore"]
 ## Documentation Setup
 docs = ["doc8", "pydocstyle[toml]", "Pygments", "pyparsing", "sphinx",
-        "sphinx-design", "sphinxawesome-codelinter", "sphinxawesome-theme ~= 5.0.0b2"]
+        "sphinx-design", "sphinxawesome-codelinter", "sphinxawesome-theme"]
 ## Linting and Formatting Setup
 lint = ["bandit[toml]", "black", "flake8", "Flake8-pyproject", "isort", "pylint", "pyright",
         "restructuredtext-lint"]
 ## Testing Setup
 test = ["coverage[toml]", "hypothesis[all]", "pytest", "pytest-asyncio", "pytest-cov", 
         "pytest-tcpclient", "pytest-randomly", "pytest-xdist"]
 
@@ -105,61 +105,61 @@
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 log_cli_format      = "%(asctime)s [%(levelname)8s] %(name)s: %(message)s (%(filename)s:%(lineno)s)"
 log_cli_level       = "INFO"
 
 [tool.semantic_release]
 # hvcs_api_domain          = ""
 # hvcs_domain              = ""
-branch                   = "main"
-build_command            = """
-                        git stash && \
-                        python -m build -w && \
-                        git stash -- PKG-INFO && \
-                        python -m pyc_wheel dist/*.whl && \
-                        meson setup dist/build && \
-                        git stash drop && \
-                        git add PKG-INFO && \
-                        git commit PKG-INFO -m \"PKG-INFO Updated\" && \
-                        meson dist -C dist/build --formats gztar --no-tests --allow-dirty && \
-                        sigstore sign dist/*.whl dist/build/meson-dist/*.tar.gz && \
-                        git stash pop && \
-                        git add CHANGELOG.md && \
-                        git stash clear"""
-changelog_file           = "CHANGELOG.md"
-changelog_placeholder    = "<!--next-version-placeholder-->"
-commit_parser            = "semantic_release.history.emoji_parser"
-commit_version_number    = true
-dist_glob_patterns       = "*.dist-info,*.whl,build/meson-dist/*.tar.gz"
-dist_path                = "dist/"
-hvcs                     = "github"
+branch                         = "main"
+build_command                  = """
+                git stash && \
+                python -m build -w && \
+                git stash -- PKG-INFO && \
+                python -m pyc_wheel dist/*.whl && \
+                meson setup dist/build && \
+                git stash drop && \
+                git add PKG-INFO && \
+                git commit PKG-INFO -m \"PKG-INFO Updated\" && \
+                meson dist -C dist/build --formats gztar --no-tests --allow-dirty && \
+                sigstore sign dist/*.whl dist/build/meson-dist/*.tar.gz && \
+                git stash pop && \
+                git add CHANGELOG.md && \
+                git stash clear"""
+changelog_file                 = "CHANGELOG.md"
+changelog_placeholder          = "<!--next-version-placeholder-->"
+commit_parser                  = "semantic_release.history.emoji_parser"
+commit_version_number          = true
+dist_glob_patterns             = "*.dist-info,*.whl,build/meson-dist/*.tar.gz"
+dist_path                      = "dist/"
+hvcs                           = "github"
 # include_additional_files = """
 #                         dist/*.sig,\
 #                         dist/*.crt,\
 #                         dist/*.sigstore,\
 #                         build/meson-dist/*.tar.gz,\
 #                         build/meson-dist/*.sha256sum,\
 #                         build/meson-dist/*.sig,\
 #                         build/meson-dist/*.crt,\
 #                         build/meson-dist/*.sigstore"""
-major_on_zero            = false
-patch_without_tag        = false
-prerelease_tag           = "beta"
-pre_commit_command       = """
-                        git clean -dfX && \
-                        meson setup build-dist-checkpoint --reconfigure -Ddev=enabled && \
-                        meson test -C build-dist-checkpoint --setup=test --setup=lint && \
-                        git stash -- PKG-INFO && \
-                        git stash drop"""
-remove_dist              = false
-repository               = "pypi"
-tag_format               = "{version}"
-upload_to_release        = false
-upload_to_repository     = true
-version_source           = "tag_only"
-version_variable         = "PKG-INFO:Version: {version}"
+major_on_zero                  = false
+patch_without_tag              = false
+prerelease_tag                 = "beta"
+pre_commit_command             = """
+                git clean -dfX && \
+                tox && \
+                git stash -- PKG-INFO && \
+                git stash drop"""
+remove_dist                    = false
+repository                     = "pypi"
+tag_format                     = "{version}"
+upload_to_release              = false
+upload_to_repository           = true
+use_textual_changelog_sections = true
+version_source                 = "tag_only"
+version_variable               = "PKG-INFO:Version: {version}"
 
 [tool.setuptools_scm]
 write_to_template = """
 Metadata-Version: 2.1
 Name: blastpipe
 Version: {version}
 Summary: Packaged with OZI.
@@ -194,26 +194,61 @@
    specific language governing permissions and limitations
    under the License.
 
 =========
 blastpipe
 =========
 
-|py-version-badge| |slsa-level3-badge| |semantic-release-badge|
+|py-version-badge| |openssf-badge| |slsa-level3-badge| |fossa-badge| |semantic-release-badge|
 |coverage-badge| |pytest-plugins-badge| 
 |bandit-badge| |black-badge| |isort-badge| |flake8-badge| |pyright-badge| |pylint-ckpt-badge| |rst-lint-badge|
 
 A simple utility library used as a slice demonstration for using
 Meson+OZI as Python 3 packaging management layer.
 
 .. image:: https://raw.githubusercontent.com/sigstore/community/main/artwork/badge/sigstore_codesigned_purple.png
  :align: right
  :height: 140
  :target: https://www.sigstore.dev/
 
+Contributing
+^^^^^^^^^^^^
+
+Contributions are what make the open source community such an amazing place to
+learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and
+create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the repository
+2. Create your Feature Branch (``git checkout -b feature/AmazingFeature``)
+3. Commit your Changes (``git commit -m 'Add some AmazingFeature'``)
+4. Push to the Branch (``git push origin feature/AmazingFeature``)
+5. Open a Pull Request
+
+Bug Reports
+^^^^^^^^^^^
+
+1. Create an issue with the tag "bug" with a descriptive title stating the issue succinctly.
+2. Fill out the issue template with the information requested.
+
+If you have any proposed changes related to a bug, if an Issue has not been created please
+complete the above instructions.
+The next steps are similar to the steps needed to create a feature pull request.
+
+Submitting a Fix
+################
+
+1. Fork the repository
+2. Create your Bugfix Branch (``git checkout -b bugfix/Issue#``)
+3. Commit your Changes (``git commit -m '🐛: Fix Issue#'``)
+4. Push to the Branch (``git push origin bugfix/Issue#``)
+5. Open a Pull Request
+
 License
 ^^^^^^^
 
 blastpipe is released under the terms of the 2.0 version of the Apache License,
 approved by the Apache Software Foundation. blastpipe meets the Open Source Initiative's definition of
 open source software, and the Free Software Foundation's definition of GPLv3-compatible open 
 source software.
@@ -248,15 +283,20 @@
  :target: https://www.gnu.org/
 
 
 
 .. |py-version-badge| image:: https://img.shields.io/badge/Python%20Version-3.9%20%7C%203.10%20%7C%203.11-blue
 .. |pylint-ckpt-badge| image:: https://img.shields.io/badge/linting-%E2%9C%94%20Pylint%3A%2010.00%2F10-informational
 .. |slsa-level3-badge| image:: https://slsa.dev/images/gh-badge-level3.svg
-
+.. |fossa-badge| image:: https://app.fossa.com/api/projects/git%2Bgithub.com%2Frjdbcm%2Fblastpipe.svg?type=shield
+    :target: https://app.fossa.com/projects/git%2Bgithub.com%2Frjdbcm%2Fblastpipe?ref=badge_large
+    :alt: License Compliance
+.. |openssf-badge| image:: https://bestpractices.coreinfrastructure.org/projects/7515/badge
+    :target: https://bestpractices.coreinfrastructure.org/projects/7515
+    :alt: Open Source Security Foundation self-certification status
 .. |semantic-release-badge| image:: https://img.shields.io/badge/semantic--release-gitmoji-e10079?logo=semantic-release
     :target: https://github.com/python-semantic-release/python-semantic-release
     :alt: Automatic Semantic Versioning for Python projects
 .. |bandit-badge| image:: https://img.shields.io/badge/security-%E2%9C%94%20bandit-yellow.svg
     :target: https://github.com/PyCQA/bandit
     :alt: Security Status
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-%E2%9C%94%20black-000000.svg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `blastpipe-0.4.24/subprojects/dev.wrap` & `blastpipe-0.4.26/subprojects/dev.wrap`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/LICENSE.txt` & `blastpipe-0.4.26/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/_static/css/custom.css` & `blastpipe-0.4.26/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/_static/css/meson.build` & `blastpipe-0.4.26/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/_static/meson.build` & `blastpipe-0.4.26/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/_templates/layout.html` & `blastpipe-0.4.26/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/_templates/meson.build` & `blastpipe-0.4.26/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/conf.cfg` & `blastpipe-0.4.26/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/index.rst` & `blastpipe-0.4.26/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/meson.build` & `blastpipe-0.4.26/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/subprojects/docs/meson.options` & `blastpipe-0.4.26/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/tests/meson.build` & `blastpipe-0.4.26/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/tests/test_backports.py` & `blastpipe-0.4.26/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/tests/test_fuzz.py` & `blastpipe-0.4.26/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.24/tests/test_tailcall.py` & `blastpipe-0.4.26/tests/test_tailcall.py`

 * *Files identical despite different names*

