# Comparing `tmp/quartodoc-0.3.4.tar.gz` & `tmp/quartodoc-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartodoc-0.3.4.tar", last modified: Wed Jun 21 17:58:07 2023, max compression
+gzip compressed data, was "quartodoc-0.3.5.tar", last modified: Thu Jul  6 21:08:34 2023, max compression
```

## Comparing `quartodoc-0.3.4.tar` & `quartodoc-0.3.5.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-21 17:57:57.000000 quartodoc-0.3.4/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-21 17:57:57.000000 quartodoc-0.3.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-21 17:57:57.000000 quartodoc-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-21 17:57:57.000000 quartodoc-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 17:57:57.000000 quartodoc-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-21 17:57:57.000000 quartodoc-0.3.4/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-21 17:57:57.000000 quartodoc-0.3.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-21 17:58:07.468516 quartodoc-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-21 17:57:57.000000 quartodoc-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 17:57:57.000000 quartodoc-0.3.4/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.452516 quartodoc-0.3.4/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/_extensions/interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 17:57:57.000000 quartodoc-0.3.4/_extensions/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 17:57:57.000000 quartodoc-0.3.4/_extensions/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-21 17:57:57.000000 quartodoc-0.3.4/_extensions/interlinks/interlinks.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/case_studies/
--rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/objects_sqla.inv
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/parsing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/some_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/sphinx-inventory.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 17:57:57.000000 quartodoc-0.3.4/case_studies/sphinx-inventory.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/about.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/advanced-layouts.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/architecture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/basic-building.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/basic-content.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/basic-docs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/crossrefs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-big-picture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-dataclasses.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-docstrings.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-prepare.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/dev-renderers.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/docstring-examples.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/docstring-style.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/extending.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/extra-build-sequence.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/interlinks.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/get-started/sidebar.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-21 17:57:57.000000 quartodoc-0.3.4/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/examples/dascore/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/dascore/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/dascore/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/dascore/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/dascore/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/examples/pkgdown/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.460516 quartodoc-0.3.4/examples/pkgdown/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/Builder.build.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/Builder.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/get_object.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/pkgdown/reference/preview.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/examples/single-page/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/single-page/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/single-page/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/single-page/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/examples/single-page/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/single-page/reference/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/examples/weird-install/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/weird-install/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/examples/weird-install/src/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 17:57:57.000000 quartodoc-0.3.4/examples/weird-install/src/some_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-21 17:57:57.000000 quartodoc-0.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/quartodoc/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/autosummary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/quartodoc/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/builder/write.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/quartodoc/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20066 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/renderers/md_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/quartodoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_alias_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/quartodoc/tests/example_interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/quartodoc/tests/example_interlinks/_inv/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/_inv/other_objects.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/interlinks.lua
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/objects.json
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/spec.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/test.md
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_interlinks/test.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/example_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_builder_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-21 17:57:57.000000 quartodoc-0.3.4/quartodoc/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.464516 quartodoc-0.3.4/quartodoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 17:58:07.000000 quartodoc-0.3.4/quartodoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-21 17:57:57.000000 quartodoc-0.3.4/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.456516 quartodoc-0.3.4/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:58:07.468516 quartodoc-0.3.4/scripts/filter-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-21 17:57:57.000000 quartodoc-0.3.4/scripts/filter-spec/generate_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-21 17:57:57.000000 quartodoc-0.3.4/scripts/filter-spec/generate_test_qmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-21 17:58:07.468516 quartodoc-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.463706 quartodoc-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-06 21:08:22.000000 quartodoc-0.3.5/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-06 21:08:22.000000 quartodoc-0.3.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-06 21:08:22.000000 quartodoc-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-06 21:08:22.000000 quartodoc-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 21:08:22.000000 quartodoc-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-06 21:08:22.000000 quartodoc-0.3.5/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-06 21:08:22.000000 quartodoc-0.3.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-06 21:08:34.463706 quartodoc-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-06 21:08:22.000000 quartodoc-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-06 21:08:22.000000 quartodoc-0.3.5/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.443705 quartodoc-0.3.5/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/_extensions/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:08:22.000000 quartodoc-0.3.5/_extensions/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 21:08:22.000000 quartodoc-0.3.5/_extensions/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-06 21:08:22.000000 quartodoc-0.3.5/_extensions/interlinks/interlinks.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/case_studies/
+-rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/objects_sqla.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/parsing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/some_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/sphinx-inventory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/sphinx-inventory.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/about.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/advanced-layouts.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/architecture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/basic-building.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/basic-content.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/basic-docs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/crossrefs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-big-picture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-dataclasses.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-docstrings.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-prepare.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-renderers.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/docstring-examples.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/docstring-style.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/extending.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/extra-build-sequence.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/interlinks.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/sidebar.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/dascore/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/dascore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/dascore/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/dascore/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/dascore/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/pkgdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/pkgdown/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/Builder.build.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/Builder.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/get_object.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/preview.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/single-page/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/single-page/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/single-page/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/single-page/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.455706 quartodoc-0.3.5/examples/single-page/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/single-page/reference/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.455706 quartodoc-0.3.5/examples/weird-install/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/weird-install/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.455706 quartodoc-0.3.5/examples/weird-install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/weird-install/src/some_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 21:08:22.000000 quartodoc-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.455706 quartodoc-0.3.5/quartodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/autosummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.459706 quartodoc-0.3.5/quartodoc/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.459706 quartodoc-0.3.5/quartodoc/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20069 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/renderers/md_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.459706 quartodoc-0.3.5/quartodoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_alias_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.463706 quartodoc-0.3.5/quartodoc/tests/example_interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.463706 quartodoc-0.3.5/quartodoc/tests/example_interlinks/_inv/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/_inv/other_objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/test.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_builder_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.459706 quartodoc-0.3.5/quartodoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-06 21:08:22.000000 quartodoc-0.3.5/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.443705 quartodoc-0.3.5/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.463706 quartodoc-0.3.5/scripts/filter-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-06 21:08:22.000000 quartodoc-0.3.5/scripts/filter-spec/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-06 21:08:22.000000 quartodoc-0.3.5/scripts/filter-spec/generate_test_qmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-06 21:08:34.463706 quartodoc-0.3.5/setup.cfg
```

### Comparing `quartodoc-0.3.4/.github/CODE_OF_CONDUCT.md` & `quartodoc-0.3.5/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/.github/workflows/ci.yml` & `quartodoc-0.3.5/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,16 @@
   push:
     branches: ["main", "dev-*"]
   pull_request:
   release:
     types: [published]
 
 jobs:
-  run-if:
-    name: "Run If"
-    runs-on: ubuntu-latest
-    if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.fork == false
-    steps:
-      - run: |
-          echo "Running CI"
   test:
     name: "Test"
-    needs: ["run-if"]
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         # Checks based on python versions ---
         python-version: ['3.9', '3.10']
         requirements: [""]
```

### Comparing `quartodoc-0.3.4/.gitignore` & `quartodoc-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/LICENSE` & `quartodoc-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/Makefile` & `quartodoc-0.3.5/Makefile`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/PKG-INFO` & `quartodoc-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.4
+Version: 0.3.5
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.3.4/README.md` & `quartodoc-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/README.qmd` & `quartodoc-0.3.5/README.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/_extensions/interlinks/interlinks.lua` & `quartodoc-0.3.5/_extensions/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/case_studies/objects_sqla.inv` & `quartodoc-0.3.5/case_studies/objects_sqla.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/case_studies/parsing.qmd` & `quartodoc-0.3.5/case_studies/parsing.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/case_studies/some_package.py` & `quartodoc-0.3.5/case_studies/some_package.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/case_studies/sphinx-inventory.md` & `quartodoc-0.3.5/case_studies/sphinx-inventory.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/case_studies/sphinx-inventory.qmd` & `quartodoc-0.3.5/case_studies/sphinx-inventory.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/_quarto.yml` & `quartodoc-0.3.5/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/examples/index.qmd` & `quartodoc-0.3.5/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/architecture.qmd` & `quartodoc-0.3.5/docs/get-started/architecture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/basic-building.qmd` & `quartodoc-0.3.5/docs/get-started/basic-building.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/basic-content.qmd` & `quartodoc-0.3.5/docs/get-started/basic-content.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/basic-docs.qmd` & `quartodoc-0.3.5/docs/get-started/basic-docs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/crossrefs.qmd` & `quartodoc-0.3.5/docs/get-started/crossrefs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/dev-big-picture.qmd` & `quartodoc-0.3.5/docs/get-started/dev-big-picture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/dev-docstrings.qmd` & `quartodoc-0.3.5/docs/get-started/dev-docstrings.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/dev-prepare.qmd` & `quartodoc-0.3.5/docs/get-started/dev-prepare.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/dev-renderers.qmd` & `quartodoc-0.3.5/docs/get-started/dev-renderers.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/docstring-examples.qmd` & `quartodoc-0.3.5/docs/get-started/docstring-examples.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/extending.qmd` & `quartodoc-0.3.5/docs/get-started/extending.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/extra-build-sequence.qmd` & `quartodoc-0.3.5/docs/get-started/extra-build-sequence.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/interlinks.qmd` & `quartodoc-0.3.5/docs/get-started/interlinks.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/overview.qmd` & `quartodoc-0.3.5/docs/get-started/overview.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/get-started/sidebar.qmd` & `quartodoc-0.3.5/docs/get-started/sidebar.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/docs/styles.css` & `quartodoc-0.3.5/docs/styles.css`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/examples/dascore/_quarto.yml` & `quartodoc-0.3.5/examples/dascore/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/examples/dascore/generate_api.py` & `quartodoc-0.3.5/examples/dascore/generate_api.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/examples/pkgdown/_quarto.yml` & `quartodoc-0.3.5/examples/pkgdown/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/examples/pkgdown/objects.json` & `quartodoc-0.3.5/examples/pkgdown/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/examples/pkgdown/reference/Builder.qmd` & `quartodoc-0.3.5/examples/pkgdown/reference/Builder.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/examples/pkgdown/reference/get_object.qmd` & `quartodoc-0.3.5/examples/pkgdown/reference/get_object.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/examples/single-page/_quarto.yml` & `quartodoc-0.3.5/examples/single-page/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/examples/single-page/objects.json` & `quartodoc-0.3.5/examples/single-page/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/examples/single-page/reference/index.qmd` & `quartodoc-0.3.5/examples/single-page/reference/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/__main__.py` & `quartodoc-0.3.5/quartodoc/__main__.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/ast.py` & `quartodoc-0.3.5/quartodoc/ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/autosummary.py` & `quartodoc-0.3.5/quartodoc/autosummary.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/builder/blueprint.py` & `quartodoc-0.3.5/quartodoc/builder/blueprint.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,23 @@
     @staticmethod
     def _append_member_path(path: str, new: str):
         if ":" in path:
             return f"{path}.{new}"
 
         return f"{path}:{new}"
 
-    def get_object_fixed(self, *args, **kwargs):
+    def get_object_fixed(self, path, **kwargs):
         try:
-            return self.get_object(*args, **kwargs)
+            return self.get_object(path, **kwargs)
         except KeyError as e:
-            raise WorkaroundKeyError(e.args[0])
+            key_name = e.args[0]
+            raise WorkaroundKeyError(
+                f"Cannot find an object named: {key_name}."
+                f" Does an object with the path {path} exist?"
+            )
 
     @dispatch
     def visit(self, el):
         # TODO: use a context handler
         self._log("VISITING", el)
 
         package = getattr(el, "package", MISSING())
```

### Comparing `quartodoc-0.3.4/quartodoc/builder/collect.py` & `quartodoc-0.3.5/quartodoc/builder/collect.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/builder/utils.py` & `quartodoc-0.3.5/quartodoc/builder/utils.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/interlinks.py` & `quartodoc-0.3.5/quartodoc/interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/inventory.py` & `quartodoc-0.3.5/quartodoc/inventory.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/layout.py` & `quartodoc-0.3.5/quartodoc/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
 import griffe.dataclasses as dc
 import logging
 
 from enum import Enum
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, Extra
 
 from typing_extensions import Annotated
 from typing import Literal, Union, Optional
 
 
 _log = logging.getLogger(__name__)
 
 
 class _Base(BaseModel):
     """Any data class that might appear in the quartodoc config."""
 
+    class Config:
+        extra = Extra.forbid
+
 
 class _Structural(_Base):
     """A structural element, like an index Section or Page of docs."""
 
 
 class _Docable(_Base):
     """An element meant to document something about a python object."""
@@ -241,14 +244,15 @@
     """
 
     name: str
     obj: Union[dc.Object, dc.Alias]
 
     class Config:
         arbitrary_types_allowed = True
+        extra = Extra.forbid
 
 
 class Doc(_Docable):
     """A python object to be documented.
 
     Note that this class should not be used directly. Instead, use child classes
     like DocFunction.
@@ -271,14 +275,15 @@
 
     name: str
     obj: Union[dc.Object, dc.Alias]
     anchor: str
 
     class Config:
         arbitrary_types_allowed = True
+        extra = Extra.forbid
 
     @classmethod
     def from_griffe(
         cls,
         name,
         obj: Union[dc.Object, dc.Alias],
         members=None,
@@ -370,14 +375,15 @@
     name: str
     obj: Union[dc.Object, dc.Alias]
     uri: Optional[str] = None
     dispname: Optional[str] = None
 
     class Config:
         arbitrary_types_allowed = True
+        extra = Extra.forbid
 
 
 # Update forwared refs --------------------------------------------------------
 
 Layout.update_forward_refs()
 Section.update_forward_refs()
 Page.update_forward_refs()
```

### Comparing `quartodoc-0.3.4/quartodoc/renderers/base.py` & `quartodoc-0.3.5/quartodoc/renderers/base.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/renderers/md_renderer.py` & `quartodoc-0.3.5/quartodoc/renderers/md_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,15 +417,15 @@
         header = ["Name", "Type", "Description", "Default"]
 
         return self._render_table(rows, header)
 
     @dispatch
     def render(self, el: ds.DocstringParameter) -> Tuple[str]:
         # TODO: if default is not, should return the word "required" (unescaped)
-        default = "required" if el.default is None else escape(el.default)
+        default = "_required_" if el.default is None else escape(el.default)
 
         annotation = self.render_annotation(el.annotation)
         clean_desc = sanitize(el.description, allow_markdown=True)
         return (escape(el.name), annotation, clean_desc, default)
 
     # attributes ----
 
@@ -434,18 +434,17 @@
         header = ["Name", "Type", "Description"]
         rows = list(map(self.render, el.value))
 
         return self._render_table(rows, header)
 
     @dispatch
     def render(self, el: ds.DocstringAttribute):
-        annotation = self.render_annotation(el.annotation)
         row = [
             sanitize(el.name),
-            self.render_annotation(annotation),
+            self.render_annotation(el.annotation),
             sanitize(el.description or "", allow_markdown=True)
         ]
         return row
 
     # warnings ----
 
     @dispatch
@@ -543,15 +542,16 @@
 
         str_func_table = "\n".join([thead, *rendered])
         return f"{header}\n\n{str_func_table}"
 
     @dispatch
     def summarize(self, el: layout.Page):
         if el.summary is not None:
-            return self._summary_row(f"[{el.summary.name}]({el.path})", el.summary.desc)
+            # TODO: assumes that files end with .qmd
+            return self._summary_row(f"[{el.summary.name}]({el.path}.qmd)", el.summary.desc)
 
         if len(el.contents) > 1 and not el.flatten:
             raise ValueError(
                 "Cannot summarize Page. Either set its `summary` attribute with name "
                 "and description details, or set `flatten` to True."
             )
```

### Comparing `quartodoc-0.3.4/quartodoc/tests/example_dynamic.py` & `quartodoc-0.3.5/quartodoc/tests/example_dynamic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/example_interlinks/interlinks.lua` & `quartodoc-0.3.5/quartodoc/tests/example_interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/example_interlinks/objects.json` & `quartodoc-0.3.5/quartodoc/tests/example_interlinks/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/example_interlinks/spec.yml` & `quartodoc-0.3.5/quartodoc/tests/example_interlinks/spec.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/example_interlinks/test.md` & `quartodoc-0.3.5/quartodoc/tests/example_interlinks/test.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/example_interlinks/test.qmd` & `quartodoc-0.3.5/quartodoc/tests/example_interlinks/test.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/test_ast.py` & `quartodoc-0.3.5/quartodoc/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/test_basic.py` & `quartodoc-0.3.5/quartodoc/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/test_builder.py` & `quartodoc-0.3.5/quartodoc/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/test_builder_blueprint.py` & `quartodoc-0.3.5/quartodoc/tests/test_builder_blueprint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from quartodoc import get_object
 from quartodoc import layout as lo
-from quartodoc.builder.blueprint import BlueprintTransformer, blueprint
+from quartodoc.builder.blueprint import (
+    BlueprintTransformer,
+    blueprint,
+    WorkaroundKeyError,
+)
 import pytest
 
 TEST_MOD = "quartodoc.tests.example"
 
 
 @pytest.fixture
 def lay():
@@ -86,7 +90,19 @@
 def test_blueprint_auto_package(bp):
     auto = lo.Auto(name="a_func", package="quartodoc.tests.example")
     res = bp.visit(auto)
 
     assert isinstance(res, lo.DocFunction)
     assert res.name == "a_func"
     assert res.anchor == "quartodoc.tests.example.a_func"
+
+
+def test_blueprint_lookup_error_message(bp):
+    auto = lo.Auto(name="quartodoc.bbb.ccc")
+
+    with pytest.raises(WorkaroundKeyError) as exc_info:
+        bp.visit(auto)
+
+    assert (
+        "Does an object with the path quartodoc.bbb.ccc exist?"
+        in exc_info.value.args[0]
+    )
```

### Comparing `quartodoc-0.3.4/quartodoc/tests/test_interlinks.py` & `quartodoc-0.3.5/quartodoc/tests/test_interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/tests/test_renderers.py` & `quartodoc-0.3.5/quartodoc/tests/test_renderers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import griffe.docstrings.dataclasses as ds
+import griffe.expressions as exp
 
 from quartodoc.renderers import MdRenderer
 from quartodoc import get_object
 
 
 @pytest.fixture
 def renderer():
@@ -56,7 +57,21 @@
 def test_render_table_description_interlink(renderer, pair):
     interlink = "[](`abc`)"
     cls_section, cls_par = pair
     pars = cls_section([cls_par(name="x", description=interlink)])
 
     res = renderer.render(pars)
     assert interlink in res
+
+
+def test_render_doc_attribute(renderer):
+    attr = ds.DocstringAttribute(
+        name = "abc",
+        description="xyz",
+        annotation=exp.Expression(exp.Name("Optional", full="Optional"), "[", "]"),
+        value=1
+    )
+
+    res = renderer.render(attr)
+
+    assert res == ["abc", "Optional\[\]", "xyz"]
+
```

### Comparing `quartodoc-0.3.4/quartodoc/tests/test_validation.py` & `quartodoc-0.3.5/quartodoc/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc/validation.py` & `quartodoc-0.3.5/quartodoc/validation.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/quartodoc.egg-info/PKG-INFO` & `quartodoc-0.3.5/quartodoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.4
+Version: 0.3.5
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.3.4/quartodoc.egg-info/SOURCES.txt` & `quartodoc-0.3.5/quartodoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/requirements-dev.txt` & `quartodoc-0.3.5/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/scripts/filter-spec/generate_files.py` & `quartodoc-0.3.5/scripts/filter-spec/generate_files.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.4/setup.cfg` & `quartodoc-0.3.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 
 [options]
 packages = find:
 include_package_data = True
 zipsafe = False
 python_requires = >=3.9
 install_requires = 
+	click
 	griffe
 	plum-dispatch<2.0.0;python_version<'3.10'
 	plum-dispatch;python_version>='3.10'
 	sphobjinv>=2.3.1
 	tabulate>=0.9.0
 	importlib-metadata>=5.1.0
 	importlib-resources>=5.10.2
-	pydantic>=1.9.2
+	pydantic<2.0
+	pyyaml
 	typing-extensions>=4.4.0
 
 [options.extras_require]
 dev = 
 	pytest
 	jupyterlab
 	jupytext
```

