# Comparing `tmp/pretext-1.6.1.dev20230704.tar.gz` & `tmp/pretext-1.6.1.dev20230706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230704.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230706.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230704.tar` & `pretext-1.6.1.dev20230706.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/LICENSE
--rw-r--r--   0        0        0     9757 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/README.md
--rw-r--r--   0        0        0     1962 2023-07-04 06:15:41.003341 pretext-1.6.1.dev20230704/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/pretext/__main__.py
--rw-r--r--   0        0        0     8531 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/pretext/build.py
--rw-r--r--   0        0        0    25736 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/pretext/cli.py
--rw-r--r--   0        0        0     5856 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/core/__init__.py
--rw-r--r--   0        0        0   172498 2023-07-04 06:15:46.119619 pretext-1.6.1.dev20230704/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/core/resources.py
--rw-r--r--   0        0        0  1044427 2023-07-04 06:15:46.119619 pretext-1.6.1.dev20230704/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/generate.py
--rw-r--r--   0        0        0    29108 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/project.py
--rw-r--r--   0        0        0      739 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160110 2023-07-04 06:15:46.195623 pretext-1.6.1.dev20230704/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7616 2023-07-04 06:15:46.199623 pretext-1.6.1.dev20230704/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173309 2023-07-04 06:15:46.183622 pretext-1.6.1.dev20230704/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2192 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4657 2023-07-04 06:15:46.167621 pretext-1.6.1.dev20230704/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8392 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    25086 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/utils.py
--rw-r--r--   0        0        0     3333 2023-07-04 06:15:41.003341 pretext-1.6.1.dev20230704/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230704/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/LICENSE
+-rw-r--r--   0        0        0     9757 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/README.md
+-rw-r--r--   0        0        0     1962 2023-07-06 06:15:51.809100 pretext-1.6.1.dev20230706/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/__main__.py
+-rw-r--r--   0        0        0     8531 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/build.py
+-rw-r--r--   0        0        0    25736 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/cli.py
+-rw-r--r--   0        0        0     5856 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172498 2023-07-06 06:15:56.773153 pretext-1.6.1.dev20230706/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/core/resources.py
+-rw-r--r--   0        0        0  1044737 2023-07-06 06:15:56.773153 pretext-1.6.1.dev20230706/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/generate.py
+-rw-r--r--   0        0        0    29108 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/project.py
+-rw-r--r--   0        0        0      739 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160110 2023-07-06 06:15:56.837153 pretext-1.6.1.dev20230706/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7616 2023-07-06 06:15:56.837153 pretext-1.6.1.dev20230706/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173309 2023-07-06 06:15:56.825153 pretext-1.6.1.dev20230706/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2192 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4657 2023-07-06 06:15:56.813153 pretext-1.6.1.dev20230706/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8392 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    25086 2023-07-06 06:15:20.613075 pretext-1.6.1.dev20230706/pretext/utils.py
+-rw-r--r--   0        0        0     3333 2023-07-06 06:15:51.809100 pretext-1.6.1.dev20230706/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230706/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230704/LICENSE` & `pretext-1.6.1.dev20230706/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/README.md` & `pretext-1.6.1.dev20230706/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/__init__.py` & `pretext-1.6.1.dev20230706/pretext/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = 'd0c0cf9e039e95a0d1cf57dbf1a5a00c2a5e866e'
+CORE_COMMIT = 'a6a25b78566917b63f84f1e6974d71105e7d5934'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.6.1.dev20230704/pretext/build.py` & `pretext-1.6.1.dev20230706/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/cli.py` & `pretext-1.6.1.dev20230706/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/codechat.py` & `pretext-1.6.1.dev20230706/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230706/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/core/pretext.py` & `pretext-1.6.1.dev20230706/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/core/resources.py` & `pretext-1.6.1.dev20230706/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/core/resources.zip` & `pretext-1.6.1.dev20230706/pretext/core/resources.zip`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
-Zip file size: 1044427 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/utilities/
--rw-r--r--  2.0 unx     8125 b- defN 23-Jul-04 06:15 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jul-04 06:15 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jul-04 06:15 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jul-04 06:15 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jul-04 06:15 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jul-04 06:15 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jul-04 06:15 xsl/README.md
--rw-r--r--  2.0 unx     2725 b- defN 23-Jul-04 06:15 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jul-04 06:15 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Jul-04 06:15 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jul-04 06:15 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jul-04 06:15 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jul-04 06:15 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jul-04 06:15 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx   548615 b- defN 23-Jul-04 06:15 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jul-04 06:15 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jul-04 06:15 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jul-04 06:15 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jul-04 06:15 xsl/entities.ent
--rw-r--r--  2.0 unx     6281 b- defN 23-Jul-04 06:15 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jul-04 06:15 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jul-04 06:15 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    94587 b- defN 23-Jul-04 06:15 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jul-04 06:15 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jul-04 06:15 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx   611681 b- defN 23-Jul-04 06:15 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jul-04 06:15 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jul-04 06:15 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jul-04 06:15 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Jul-04 06:15 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jul-04 06:15 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jul-04 06:15 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx   112450 b- defN 23-Jul-04 06:15 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jul-04 06:15 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jul-04 06:15 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx   113634 b- defN 23-Jul-04 06:15 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jul-04 06:15 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jul-04 06:15 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx   544229 b- defN 23-Jul-04 06:15 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jul-04 06:15 xsl/utilities/README.md
--rw-r--r--  2.0 unx     4926 b- defN 23-Jul-04 06:15 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jul-04 06:15 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Jul-04 06:15 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Jul-04 06:15 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx      513 b- defN 23-Jul-04 06:15 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4760 b- defN 23-Jul-04 06:15 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15866 b- defN 23-Jul-04 06:15 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Jul-04 06:15 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    16837 b- defN 23-Jul-04 06:15 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16534 b- defN 23-Jul-04 06:15 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    19185 b- defN 23-Jul-04 06:15 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16085 b- defN 23-Jul-04 06:15 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16349 b- defN 23-Jul-04 06:15 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16312 b- defN 23-Jul-04 06:15 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    17056 b- defN 23-Jul-04 06:15 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16252 b- defN 23-Jul-04 06:15 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    20481 b- defN 23-Jul-04 06:15 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    17081 b- defN 23-Jul-04 06:15 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    15582 b- defN 23-Jul-04 06:15 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17231 b- defN 23-Jul-04 06:15 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    19326 b- defN 23-Jul-04 06:15 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    16500 b- defN 23-Jul-04 06:15 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17301 b- defN 23-Jul-04 06:15 xsl/localizations/fi-FI.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-Jul-04 06:15 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jul-04 06:15 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jul-04 06:15 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jul-04 06:15 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx    10306 b- defN 23-Jul-04 06:15 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jul-04 06:15 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jul-04 06:15 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-Jul-04 06:15 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Jul-04 06:15 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx      722 b- defN 23-Jul-04 06:15 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx    14482 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-guide.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jul-04 06:15 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jul-04 06:15 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 23-Jul-04 06:15 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-Jul-04 06:15 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 06:15 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-Jul-04 06:15 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx     1180 b- defN 23-Jul-04 06:15 schema/README.md
--rw-r--r--  2.0 unx   101829 b- defN 23-Jul-04 06:15 schema/pretext.rng
--rw-r--r--  2.0 unx    34210 b- defN 23-Jul-04 06:15 schema/pretext-dev.rng
--rw-r--r--  2.0 unx      326 b- defN 23-Jul-04 06:15 schema/xml.xsd
--rw-r--r--  2.0 unx    25870 b- defN 23-Jul-04 06:15 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-Jul-04 06:15 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   134043 b- defN 23-Jul-04 06:15 schema/pretext.xml
--rw-r--r--  2.0 unx     3135 b- defN 23-Jul-04 06:15 schema/build.sh
--rw-r--r--  2.0 unx    58086 b- defN 23-Jul-04 06:15 schema/pretext.rnc
--rw-r--r--  2.0 unx    18421 b- defN 23-Jul-04 06:15 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx   125135 b- defN 23-Jul-04 06:15 schema/pretext.xsd
--rw-r--r--  2.0 unx     1367 b- defN 23-Jul-04 06:15 pretext/README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 06:15 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Jul-04 06:15 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-Jul-04 06:15 pretext/pretext
--rw-r--r--  2.0 unx    36045 b- defN 23-Jul-04 06:15 pretext/braille_format.py
--rw-r--r--  2.0 unx   172498 b- defN 23-Jul-04 06:15 pretext/pretext.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jul-04 06:15 pretext/pretext.cfg
--rw-r--r--  2.0 unx     2608 b- defN 23-Jul-04 06:15 css/colors_default.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jul-04 06:15 css/pretext_add_on.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jul-04 06:15 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jul-04 06:15 css/kindle.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jul-04 06:15 css/README.md
--rw-r--r--  2.0 unx     1362 b- defN 23-Jul-04 06:15 css/epub.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jul-04 06:15 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jul-04 06:15 css/pretext.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jul-04 06:15 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jul-04 06:15 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-04 06:15 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jul-04 06:15 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jul-04 06:15 css/style_soundwriting.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_orange_navy.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jul-04 06:15 css/mathbook-3.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-04 06:15 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jul-04 06:15 css/setcolors.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jul-04 06:15 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jul-04 06:15 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jul-04 06:15 css/update_css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jul-04 06:15 css/style_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jul-04 06:15 css/colors_red_blue.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jul-04 06:15 css/colors_maroon_grey.css
-142 files, 4847185 bytes uncompressed, 1026853 bytes compressed:  78.8%
+Zip file size: 1044737 bytes, number of entries: 142
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/utilities/
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jul-06 06:15 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jul-06 06:15 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jul-06 06:15 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jul-06 06:15 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jul-06 06:15 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jul-06 06:15 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jul-06 06:15 xsl/README.md
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jul-06 06:15 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jul-06 06:15 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jul-06 06:15 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jul-06 06:15 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jul-06 06:15 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jul-06 06:15 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jul-06 06:15 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx   548615 b- defN 23-Jul-06 06:15 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jul-06 06:15 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jul-06 06:15 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jul-06 06:15 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jul-06 06:15 xsl/entities.ent
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jul-06 06:15 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jul-06 06:15 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jul-06 06:15 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    94587 b- defN 23-Jul-06 06:15 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jul-06 06:15 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jul-06 06:15 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx   611681 b- defN 23-Jul-06 06:15 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jul-06 06:15 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jul-06 06:15 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jul-06 06:15 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Jul-06 06:15 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jul-06 06:15 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jul-06 06:15 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jul-06 06:15 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jul-06 06:15 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jul-06 06:15 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx   113893 b- defN 23-Jul-06 06:15 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jul-06 06:15 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jul-06 06:15 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx   545213 b- defN 23-Jul-06 06:15 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jul-06 06:15 xsl/utilities/README.md
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jul-06 06:15 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jul-06 06:15 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jul-06 06:15 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-Jul-06 06:15 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx      513 b- defN 23-Jul-06 06:15 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4760 b- defN 23-Jul-06 06:15 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15866 b- defN 23-Jul-06 06:15 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Jul-06 06:15 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    16837 b- defN 23-Jul-06 06:15 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16534 b- defN 23-Jul-06 06:15 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    19185 b- defN 23-Jul-06 06:15 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16085 b- defN 23-Jul-06 06:15 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16349 b- defN 23-Jul-06 06:15 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16312 b- defN 23-Jul-06 06:15 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    17056 b- defN 23-Jul-06 06:15 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16252 b- defN 23-Jul-06 06:15 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    20481 b- defN 23-Jul-06 06:15 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    17081 b- defN 23-Jul-06 06:15 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    15582 b- defN 23-Jul-06 06:15 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17231 b- defN 23-Jul-06 06:15 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    19326 b- defN 23-Jul-06 06:15 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    16500 b- defN 23-Jul-06 06:15 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17301 b- defN 23-Jul-06 06:15 xsl/localizations/fi-FI.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-Jul-06 06:15 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jul-06 06:15 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jul-06 06:15 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jul-06 06:15 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jul-06 06:15 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jul-06 06:15 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jul-06 06:15 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jul-06 06:15 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jul-06 06:15 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx      722 b- defN 23-Jul-06 06:15 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-guide.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jul-06 06:15 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jul-06 06:15 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 23-Jul-06 06:15 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-Jul-06 06:15 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 06:15 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jul-06 06:15 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jul-06 06:15 schema/README.md
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jul-06 06:15 schema/pretext.rng
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jul-06 06:15 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx      326 b- defN 23-Jul-06 06:15 schema/xml.xsd
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jul-06 06:15 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jul-06 06:15 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jul-06 06:15 schema/pretext.xml
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jul-06 06:15 schema/build.sh
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jul-06 06:15 schema/pretext.rnc
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jul-06 06:15 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jul-06 06:15 schema/pretext.xsd
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jul-06 06:15 pretext/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 06:15 pretext/__init__.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jul-06 06:15 pretext/module-test.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jul-06 06:15 pretext/pretext
+-rw-r--r--  2.0 unx    36045 b- defN 23-Jul-06 06:15 pretext/braille_format.py
+-rw-r--r--  2.0 unx   172498 b- defN 23-Jul-06 06:15 pretext/pretext.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jul-06 06:15 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jul-06 06:15 css/colors_default.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jul-06 06:15 css/pretext_add_on.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jul-06 06:15 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jul-06 06:15 css/kindle.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jul-06 06:15 css/README.md
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jul-06 06:15 css/epub.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jul-06 06:15 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jul-06 06:15 css/pretext.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jul-06 06:15 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jul-06 06:15 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-06 06:15 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jul-06 06:15 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jul-06 06:15 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jul-06 06:15 css/mathbook-3.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-06 06:15 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jul-06 06:15 css/setcolors.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jul-06 06:15 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jul-06 06:15 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jul-06 06:15 css/update_css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jul-06 06:15 css/style_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jul-06 06:15 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jul-06 06:15 css/colors_maroon_grey.css
+142 files, 4848428 bytes uncompressed, 1027163 bytes compressed:  78.8%
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -734,16 +734,18 @@
   <!--   - every Parsons problem "exercise"             -->
   <!--   - every horizontal Parsons problem "exercise"  -->
   <!--   - every matching problem "exercise"            -->
   <!--   - every clickable area problem "exercise"      -->
   <!--   - every "exercise" with fill-in blanks         -->
   <!--   - every "exercise" with additional "program"   -->
   <!--   - every "exercise" elected as "shortanswer"    -->
+  <!--   - every "exercise" with a WeBWorK core         -->
   <!--   - every PROJECT-LIKE with additional "program" -->
-  <xsl:template match="exercise[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                       |                       project[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                      activity[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                   exploration[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                 investigation[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                          task[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]" mode="runestone-manifest">
+  <!--     NB: "task" does not have "webwork" children  -->
+  <xsl:template match="exercise[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer') or                                (@exercise-interactive = 'webwork-reps')]                       |                       project[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer') or                                (@exercise-interactive = 'webwork-reps')]                      |                      activity[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer') or                                (@exercise-interactive = 'webwork-reps')]                      |                   exploration[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer') or                                (@exercise-interactive = 'webwork-reps')]                      |                 investigation[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer') or                                (@exercise-interactive = 'webwork-reps')]                      |                          task[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]" mode="runestone-manifest">
     <question>
       <!-- A divisional exercise ("exercises/../exercise") is not really   -->
       <!-- a reading activity in the Runestone model, so we flag these     -->
       <!-- exercises as such.  Also, interactive "task" come through here, -->
       <!-- so we need to look to an ancestor to see if the containing      -->
       <!-- "exercise" is divisional. The @optional attribute matches the   -->
       <!-- "optional" flag in the Runestone database.  We simply set the   -->
@@ -757,33 +759,32 @@
       </xsl:if>
       <!-- label is from the "exercise" -->
       <xsl:apply-templates select="." mode="runestone-manifest-label"/>
       <!-- Duplicate, but still should look like original (ID, etc.),  -->
       <!-- not knowled. Solutions are available in the originals, via  -->
       <!-- an "in context" link off the Assignment page                -->
       <htmlsrc>
-        <xsl:apply-templates select="." mode="exercise-components">
-          <xsl:with-param name="b-original" select="true()"/>
-          <xsl:with-param name="block-type" select="'visible'"/>
-          <xsl:with-param name="b-has-statement" select="true()"/>
-          <xsl:with-param name="b-has-hint" select="false()"/>
-          <xsl:with-param name="b-has-answer" select="false()"/>
-          <xsl:with-param name="b-has-solution" select="false()"/>
-        </xsl:apply-templates>
-      </htmlsrc>
-    </question>
-  </xsl:template>
-  <!-- exercise and PROJECT-LIKE with WeBWorK guts -->
-  <xsl:template match="exercise[(@exercise-interactive = 'webwork-reps')]                    | project[(@exercise-interactive = 'webwork-reps')]                    | activity[(@exercise-interactive = 'webwork-reps')]                    | exploration[(@exercise-interactive = 'webwork-reps')]                    | investigation[(@exercise-interactive = 'webwork-reps')]" mode="runestone-manifest">
-    <question>
-      <xsl:apply-templates select="." mode="runestone-manifest-label"/>
-      <htmlsrc>
-        <xsl:apply-templates select="." mode="webwork-core">
-          <xsl:with-param name="b-original" select="true()"/>
-        </xsl:apply-templates>
+        <xsl:choose>
+          <!-- with "webwork" guts, the HTML is exceptional -->
+          <xsl:when test="@exercise-interactive = 'webwork-reps'">
+            <xsl:apply-templates select="." mode="webwork-core">
+              <xsl:with-param name="b-original" select="true()"/>
+            </xsl:apply-templates>
+          </xsl:when>
+          <xsl:otherwise>
+            <xsl:apply-templates select="." mode="exercise-components">
+              <xsl:with-param name="b-original" select="true()"/>
+              <xsl:with-param name="block-type" select="'visible'"/>
+              <xsl:with-param name="b-has-statement" select="true()"/>
+              <xsl:with-param name="b-has-hint" select="false()"/>
+              <xsl:with-param name="b-has-answer" select="false()"/>
+              <xsl:with-param name="b-has-solution" select="false()"/>
+            </xsl:apply-templates>
+          </xsl:otherwise>
+        </xsl:choose>
       </htmlsrc>
     </question>
   </xsl:template>
   <!-- TODO: by renaming/refactoring the templates inside of   -->
   <!-- "htmlsrc" then perhaps several of these templates with  -->
   <!-- similar structure can be combined via one larger match. -->
   <xsl:template match="video[@youtube]" mode="runestone-manifest">
```

#### xsl/pretext-latex.xsl

##### xsl/pretext-latex.xsl

```diff
@@ -1858,16 +1858,28 @@
     <!-- simple experiment was very effective at resolving just chapters in -->
     <!-- structural parts.                                                 -->
     <!--                                                                    -->
     <!-- For both approaches, see revalatory post:                          -->
     <!-- https://tex.stackexchange.com/questions/231361/                    -->
     <!-- table-of-contents-labels-not-directing-hyperlinks-to-correct-page  -->
     <xsl:text>%% Less-clever names for hyperlinks are more reliable, *especially* for structural parts</xsl:text>
-    <xsl:text>%% See comments in the code to learn more about the importance of tnis setting</xsl:text>
+    <xsl:text>%% See comments in the code to learn more about the importance of this setting</xsl:text>
     <xsl:text>\hypersetup{hypertexnames=false}</xsl:text>
+    <!-- Index entries now have the correct (printed) page number, but the -->
+    <!-- hyperlink is way off (owing to significant front matter) and uses -->
+    <!-- a page number that is way too early.  Fix comes from the answer:  -->
+    <!--     https://tex.stackexchange.com/a/516275                        -->
+    <!-- on the post:                                                      -->
+    <!--     https://tex.stackexchange.com/questions/516267/               -->
+    <!--     compatibility-of-hypertexnames-false-and-indexes              -->
+    <xsl:text>%%The  hypertexnames  setting then confuses the hyperlinking from the index</xsl:text>
+    <xsl:text>%%This patch resolves the incorrect links, see code for StackExchange post.</xsl:text>
+    <xsl:text>\makeatletter</xsl:text>
+    <xsl:text>\patchcmd\Hy@EveryPageBoxHook{\Hy@EveryPageAnchor}{\Hy@hypertexnamestrue\Hy@EveryPageAnchor}{}{\fail}</xsl:text>
+    <xsl:text>\makeatother</xsl:text>
     <!-- Title goes interesting places in a PDF -->
     <xsl:text>\hypersetup{pdftitle={</xsl:text>
     <xsl:apply-templates select="." mode="title-short"/>
     <xsl:text>}}</xsl:text>
     <!-- http://tex.stackexchange.com/questions/44088/when-do-i-need-to-invoke-phantomsection -->
     <!-- NB: \phantomsection is rarely used - literate programming fragments and the ToC      -->
     <xsl:text>%% If you manually remove hyperref, leave in this next command</xsl:text>
```

### Comparing `pretext-1.6.1.dev20230704/pretext/generate.py` & `pretext-1.6.1.dev20230706/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/project.py` & `pretext-1.6.1.dev20230706/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230706/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230706/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230706/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160110 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
--rw-r--r--  2.0 unx       86 b- defN 23-Jul-04 06:15 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-04 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-04 06:15 assets/frog.jpg
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-04 06:15 publication/publication.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jul-04 06:15 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jul-04 06:15 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jul-04 06:15 source/section-1.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
+-rw-r--r--  2.0 unx       86 b- defN 23-Jul-06 06:15 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-06 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-06 06:15 assets/frog.jpg
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-06 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jul-06 06:15 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jul-06 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-Jul-06 06:15 source/section-1.ptx
 14 files, 164841 bytes uncompressed, 158588 bytes compressed:  3.8%
```

### Comparing `pretext-1.6.1.dev20230704/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230706/pretext/templates/resources/book.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7616 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-04 06:15 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-04 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6114 b- defN 23-Jul-04 06:15 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jul-04 06:15 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-06 06:15 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-06 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jul-06 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jul-06 06:15 source/main.ptx
 10 files, 15809 bytes uncompressed, 6522 bytes compressed:  58.7%
```

### Comparing `pretext-1.6.1.dev20230704/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230706/pretext/templates/resources/demo.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173309 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-04 06:15 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-04 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-04 06:15 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jul-04 06:15 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6092 b- defN 23-Jul-04 06:15 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/images/
--rw-r--r--  2.0 unx     1115 b- defN 23-Jul-04 06:15 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jul-04 06:15 source/backmatter.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jul-04 06:15 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-04 06:15 source/ch-empty.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jul-04 06:15 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jul-04 06:15 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jul-04 06:15 source/docinfo.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jul-04 06:15 source/main.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jul-04 06:15 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jul-04 06:15 source/frontmatter.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jul-04 06:15 source/ch-generate.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jul-04 06:15 source/ch-features.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jul-04 06:15 source/ex-first.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jul-04 06:15 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jul-04 06:15 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jul-04 06:15 source/sec-features.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-Jul-04 06:15 source/images/cflag.asy
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-04 06:15 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-04 06:15 source/images/tikz.tex
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-04 06:15 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-06 06:15 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-06 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-06 06:15 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jul-06 06:15 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jul-06 06:15 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/images/
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jul-06 06:15 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jul-06 06:15 source/backmatter.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jul-06 06:15 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-06 06:15 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jul-06 06:15 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jul-06 06:15 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jul-06 06:15 source/docinfo.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jul-06 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jul-06 06:15 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jul-06 06:15 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-06 06:15 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jul-06 06:15 source/ch-features.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jul-06 06:15 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jul-06 06:15 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jul-06 06:15 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jul-06 06:15 source/sec-features.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-Jul-06 06:15 source/images/cflag.asy
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-06 06:15 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jul-06 06:15 source/images/tikz.tex
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-06 06:15 source/images/sageplot2d.sage
 34 files, 190104 bytes uncompressed, 169353 bytes compressed:  10.9%
```

### Comparing `pretext-1.6.1.dev20230704/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230706/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230706/pretext/templates/resources/hello.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4657 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-04 06:15 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-Jul-04 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-04 06:15 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-04 06:15 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-06 06:15 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jul-06 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-06 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-06 06:15 source/main.ptx
 10 files, 7820 bytes uncompressed, 3563 bytes compressed:  54.4%
```

### Comparing `pretext-1.6.1.dev20230704/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230706/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230706/pretext/templates/resources/slideshow.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8392 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-04 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-04 06:15 xsl/slides.xsl
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     2097 b- defN 23-Jul-04 06:15 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jul-04 06:15 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-Jul-06 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
+-rw-r--r--  2.0 unx      190 b- defN 23-Jul-06 06:15 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jul-06 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jul-06 06:15 source/main.ptx
 11 files, 20407 bytes uncompressed, 7204 bytes compressed:  64.7%
```

### Comparing `pretext-1.6.1.dev20230704/pretext/utils.py` & `pretext-1.6.1.dev20230706/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230704/pyproject.toml` & `pretext-1.6.1.dev20230706/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230704"
+version = "1.6.1.dev20230706"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230704/PKG-INFO` & `pretext-1.6.1.dev20230706/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230704
+Version: 1.6.1.dev20230706
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

