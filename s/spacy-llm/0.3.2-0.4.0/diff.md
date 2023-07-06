# Comparing `tmp/spacy-llm-0.3.2.tar.gz` & `tmp/spacy-llm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.3.2.tar", last modified: Mon Jun 26 12:21:30 2023, max compression
+gzip compressed data, was "spacy-llm-0.4.0.tar", last modified: Thu Jul  6 12:07:58 2023, max compression
```

## Comparing `spacy-llm-0.3.2.tar` & `spacy-llm-0.4.0.tar`

### file list

```diff
@@ -1,151 +1,170 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    63200 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    61956 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      736 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1810 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.388330 spacy-llm-0.3.2/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      234 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.388330 spacy-llm-0.3.2/spacy_llm/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.388330 spacy-llm-0.3.2/spacy_llm/backends/integration/
--rw-r--r--   0 vsts      (1001) docker     (122)      502 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/
--rw-r--r--   0 vsts      (1001) docker     (122)      279 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4712 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2583 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3435 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4715 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/
--rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1256 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/minichain.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/backends/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)      229 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4784 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4157 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/cohere.py
--rw-r--r--   0 vsts      (1001) docker     (122)      571 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/openai.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1901 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7765 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11370 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3959 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7947 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      512 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7901 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8724 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/spancat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/lemma.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/ner.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/ner.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/rel.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/spancat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/spancat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)    15128 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tasks/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      220 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      223 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/parsing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4009 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4826 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/span.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2294 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_cohere.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1682 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_minichain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2092 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_stablelm.py
--rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1111 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8288 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/ner_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/ner_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/ner_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/rel_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/spacy_llm/tests/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/templates/lemma_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/templates/ner_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/templates/textcat_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)     7949 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22403 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5704 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17202 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23835 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7253 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8941 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/ty.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.388330 spacy-llm-0.3.2/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    63200 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4685 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      149 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/usage_examples/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/usage_examples/multitask_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/multitask_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/multitask_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/usage_examples/ner_dolly/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/usage_examples/ner_langchain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_langchain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_langchain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/usage_examples/ner_minichain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_minichain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_minichain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/usage_examples/rel_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/rel_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/rel_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/usage_examples/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3509 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/tests/test_readme_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/tests/test_usage_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/usage_examples/textcat_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/textcat_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/textcat_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)   103207 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)   101989 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      884 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1799 2023-07-06 12:07:58.965167 spacy-llm-0.4.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      232 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10379 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      895 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/hf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      264 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4886 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2439 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2814 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3384 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4816 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/langchain/
+-rw-r--r--   0 vsts      (1001) docker     (122)      227 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/langchain/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4540 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/langchain/model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/
+-rw-r--r--   0 vsts      (1001) docker     (122)      476 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3964 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10902 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5808 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/base.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/cohere/
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/cohere/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3369 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/cohere/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2016 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/cohere/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/noop/
+-rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/noop/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      815 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/noop/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      351 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/noop/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5801 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/openai/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19421 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/openai/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11251 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2940 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      850 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4725 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8738 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8998 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4807 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/sentiment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6944 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/span.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9497 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5720 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/summarization.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/lemma.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/ner.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/rel.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      526 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/sentiment.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/spancat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/summarization.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)    16409 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4042 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/util/serialization.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.957167 spacy-llm-0.4.0/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1107 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.957167 spacy-llm-0.4.0/spacy_llm/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2481 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3094 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1567 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1457 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1825 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3299 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.957167 spacy-llm-0.4.0/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8914 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.957167 spacy-llm-0.4.0/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/ner.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/ner.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/ner.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      349 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/ner_inconsistent.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/rel.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/sentiment.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      186 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/sentiment.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      174 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/sentiment.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3126 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/summarization.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     3093 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/summarization.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)     3089 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/summarization.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_binary.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_binary.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_binary.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_excl.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_excl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_excl.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/lemma.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/ner.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/sentiment.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/summarization.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/textcat.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)     9678 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24355 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6093 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6983 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_sentiment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17549 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13777 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_summarization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23930 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9200 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1694 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9252 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)   103207 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     5129 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3344 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2591 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.3.2/LICENSE` & `spacy-llm-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/README.md` & `spacy-llm-0.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,52 @@
+Metadata-Version: 2.1
+Name: spacy-llm
+Version: 0.4.0
+Summary: Integrating LLMs into structured NLP pipelines
+Author: Explosion
+Author-email: contact@explosion.ai
+License: MIT
+Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
+Project-URL: Source, https://github.com/explosion/spacy-llm
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: langchain
+Provides-Extra: transformers
+License-File: LICENSE
+
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-llm: Integrating LLMs into structured NLP pipelines
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/workflows/test.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 This package integrates Large Language Models (LLMs) into [spaCy](https://spacy.io), featuring a modular system for **fast prototyping** and **prompting**, and turning unstructured responses into **robust outputs** for various NLP tasks, **no training data** required.
 
 - Serializable `llm` **component** to integrate prompts into your pipeline
-- **Modular functions** to define the [**task**](#tasks) (prompting and parsing) and [**backend**](#backends) (model to use)
+- **Modular functions** to define the [**task**](#tasks) (prompting and parsing) and [**model**](#models)
 - Support for **hosted APIs** and self-hosted **open-source models**
-- Integration with [`MiniChain`](https://github.com/srush/MiniChain) and [`LangChain`](https://github.com/hwchase17/langchain)
+- Integration with [`LangChain`](https://github.com/hwchase17/langchain)
 - Access to **[OpenAI API](https://platform.openai.com/docs/api-reference/introduction)**, including GPT-4 and various GPT-3 models
 - Built-in support for **open-source [Dolly](https://huggingface.co/databricks)** models hosted on Hugging Face
 - Usage examples for **Named Entity Recognition** and **Text Classification**
 - Easy implementation of **your own functions** via [spaCy's registry](https://spacy.io/api/top-level#registry) for custom prompting, parsing and model integrations
 
 ## 🧠 Motivation
 
@@ -37,15 +68,15 @@
 python -m pip install spacy-llm
 ```
 
 > ⚠️ This package is still experimental and it is possible that changes made to the interface will be breaking in minor version updates.
 
 ## 🐍 Usage
 
-The task and the backend have to be supplied to the `llm` pipeline component using [spaCy's config
+The task and the model have to be supplied to the `llm` pipeline component using [spaCy's config
 system](https://spacy.io/api/data-formats#config). This package provides various built-in
 functionality, as detailed in the [API](#-api) documentation.
 
 ### Example 1: Add a text classifier using a GPT-3 model from OpenAI
 
 Create a new API key from openai.com or fetch an existing one, and ensure the keys are set as environmental variables.
 For more background information, see the [OpenAI](#openai) section.
@@ -63,18 +94,17 @@
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
 labels = ["COMPLIMENT", "INSULT"]
 
-[components.llm.backend]
-@llm_backends = "spacy.REST.v1"
-api = "OpenAI"
-config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
+[components.llm.model]
+@llm_models = "spacy.GPT-3-5.v1"
+config = {"temperature": 0.3}
 ```
 
 Now run:
 
 ```python
 from spacy_llm.util import assemble
 
@@ -101,18 +131,18 @@
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
 labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
-[components.llm.backend]
-@llm_backends = "spacy.Dolly_HF.v1"
-# For better performance, use databricks/dolly-v2-12b instead
-model = "databricks/dolly-v2-3b"
+[components.llm.model]
+@llm_models = "spacy.Dolly.v1"
+# For better performance, use dolly-v2-12b instead
+name = "dolly-v2-3b"
 ```
 
 Now run:
 
 ```python
 from spacy_llm.util import assemble
 
@@ -138,18 +168,16 @@
 nlp.add_pipe(
     "llm",
     config={
         "task": {
             "@llm_tasks": "spacy.NER.v2",
             "labels": ["PERSON", "ORGANISATION", "LOCATION"]
         },
-        "backend": {
-            "@llm_backends": "spacy.REST.v1",
-            "api": "OpenAI",
-            "config": {"model": "gpt-3.5-turbo"},
+        "model": {
+            "@llm_models": "spacy.gpt-3.5.v1",
         },
     },
 )
 nlp.initialize()
 doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents])
 ```
@@ -250,15 +278,15 @@
 
 
 Text:
 '''
 You look gorgeous!
 '''
 
-Backend response for doc: You look gorgeous!
+Model response for doc: You look gorgeous!
 COMPLIMENT
 ```
 
 `print(doc.cats)` to standard output should look like:
 
 ```
 {'COMPLIMENT': 1.0, 'INSULT': 0.0}
@@ -267,36 +295,36 @@
 ## 📓 API
 
 `spacy-llm` exposes a `llm` factory that accepts the following configuration options:
 
 | Argument         | Type                                        | Description                                                                         |
 | ---------------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
 | `task`           | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
-| `backend`        | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
+| `model`          | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#models).                          |
 | `cache`          | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
 | `save_io`        | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`.                 |
-| `validate_types` | `bool`                                      | Whether to check if signatures of configured backend and task are consistent.       |
+| `validate_types` | `bool`                                      | Whether to check if signatures of configured model and task are consistent.         |
 
 An `llm` component is defined by two main settings:
 
 - A [**task**](#tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
   back into structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects.
-- A [**backend**](#backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
+- A [**model**](#models) defining the model and how to connect to it. Note that `spacy-llm` supports both access to external
   APIs (such as OpenAI) as well as access to self-hosted open-source LLMs (such as using Dolly through Hugging Face).
 
 Moreover, `spacy-llm` exposes a customizable [**caching**](#cache) functionality to avoid running
 the same document through an LLM service (be it local or through a REST API) more than once.
 
 Finally, you can choose to save a stringified version of LLM prompts/responses
 within the `Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
 `Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM component
 within the spaCy pipeline. Each entry is itself a dictionary, with two keys:
 `prompt` and `response`.
 
-A note on `validate_types`: by default, `spacy-llm` checks whether the signatures of the `backend` and `task` callables
+A note on `validate_types`: by default, `spacy-llm` checks whether the signatures of the `model` and `task` callables
 are consistent with each other and emits a warning if they don't. `validate_types` can be set to `False` if you want to
 disable this behavior.
 
 ### Tasks
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
@@ -304,14 +332,47 @@
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
 
 Moreover, the task may define an optional [`scorer` method](https://spacy.io/api/scorer#score).
 It should accept an iterable of `Example`s as input and return a score dictionary.
 If the `scorer` method is defined, `spacy-llm` will call it to evaluate the component.
 
+#### Providing examples for few-shot prompts
+
+All built-in tasks support few-shot prompts, i. e. including examples in a prompt. Examples can be supplied in two ways:
+(1) as a separate file containing only examples or (2) by initializing `llm` with a `get_examples()` callback (like any
+other spaCy pipeline component).
+
+##### (1) Few-shot example file
+
+A file containing examples for few-shot prompting can be configured like this:
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.NER.v2"
+labels = PERSON,ORGANISATION,LOCATION
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "ner_examples.yml"
+```
+
+The supplied file has to conform to the format expected by the required task (see the task documentation further down).
+
+##### (2) Initializing the `llm` component with a `get_examples()` callback
+
+Alternatively, you can initialize your `nlp` pipeline by providing a `get_examples` callback for
+[`nlp.initialize`](https://spacy.io/api/language#initialize) and setting `n_prompt_examples` to a positive number to
+automatically fetch a few examples for few-shot learning. Set `n_prompt_examples` to `-1` to use all examples as
+part of the few-shot learning prompt.
+
+```ini
+[initialize.components.llm]
+n_prompt_examples = 3
+```
+
 #### <kbd>function</kbd> `task.generate_prompts`
 
 Takes a collection of documents, and returns a collection of "prompts", which can be of type `Any`.
 Often, prompts are of type `str` - but this is not enforced to allow for maximum flexibility in the framework.
 
 | Argument    | Type            | Description            |
 | ----------- | --------------- | ---------------------- |
@@ -321,37 +382,84 @@
 #### <kbd>function</kbd> `task.parse_responses`
 
 Takes a collection of LLM responses and the original documents, parses the responses into structured information,
 and sets the annotations on the documents. The `parse_responses` function is free to set the annotations in any way,
 including `Doc` fields like `ents`, `spans` or `cats`, or using custom defined fields.
 
 The `responses` are of type `Iterable[Any]`, though they will often be `str` objects. This depends on the
-return type of the [backend](#backends).
+return type of the [model](#models).
 
 | Argument    | Type            | Description              |
 | ----------- | --------------- | ------------------------ |
 | `docs`      | `Iterable[Doc]` | The input documents.     |
 | `responses` | `Iterable[Any]` | The generated prompts.   |
 | **RETURNS** | `Iterable[Doc]` | The annotated documents. |
 
+
+#### spacy.Summarization.v1
+
+The `spacy.Summarization.v1` task supports both zero-shot and few-shot prompting.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.Summarization.v1"
+examples = null
+max_n_words = null
+```
+
+| Argument      | Type                                    | Default                                                                | Description                                                                                                                              |
+|---------------|-----------------------------------------|------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
+| `template`    | `str`                                   | [summarization.jinja](./spacy_llm/tasks/templates/summarization.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
+| `examples`    | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                                 | Optional function that generates examples for few-shot learning.                                                                         |
+| `max_n_words` | `Optional[int]`                         | `None`                                                                 | Maximum number of words to be used in summary. Note that this should not expected to work exactly.                                       |
+| `field`       | `str`                                   | `summary`                                                              | Name of extension attribute to store summary in (i. e. the summary will be available in `doc._.{field}`).                                |
+
+The summarization task prompts the model for a concise summary of the provided text. It optionally allows to limit the 
+response to a certain number of tokens - note that this requirement will be included in the prompt, but the task doesn't
+perform a hard cut-off. It's hence possible that your summary exceeds `max_n_words`.
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```yaml
+- text: >
+    The United Nations, referred to informally as the UN, is an intergovernmental organization whose stated purposes are 
+    to maintain international peace and security, develop friendly relations among nations, achieve international 
+    cooperation, and serve as a centre for harmonizing the actions of nations. It is the world's largest international 
+    organization. The UN is headquartered on international territory in New York City, and the organization has other 
+    offices in Geneva, Nairobi, Vienna, and The Hague, where the International Court of Justice is headquartered.\n\n
+    The UN was established after World War II with the aim of preventing future world wars, and succeeded the League of 
+    Nations, which was characterized as ineffective. 
+  summary: "The UN is an international organization that promotes global peace, cooperation, and harmony. Established after WWII, its purpose is to prevent future world wars."
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.summarization.v1"
+max_n_words = 20
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "summarization_examples.yml"
+```
+
 #### spacy.NER.v2
 
 The built-in NER task supports both zero-shot and few-shot prompting. This version also supports explicitly defining the provided labels with custom descriptions.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
 labels = ["PERSON", "ORGANISATION", "LOCATION"]
 examples = null
 ```
 
 | Argument                  | Type                                    | Default                                                  | Description                                                                                                                                           |
 | ------------------------- | --------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `labels`                  | `Union[List[str], str]`                 |                                                          | List of labels or str of comma-separated list of labels.                                                                                              |
-| `template`                | `str`                                   | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
+| `template`                | `str`                                   | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM model. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.                |
 | `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                   | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                   | Optional function that generates examples for few-shot learning.                                                                                      |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                   | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
 | `alignment_mode`          | `str`                                   | `"contract"`                                             | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
 | `case_sensitive_matching` | `bool`                                  | `False`                                                  | Whether to search without case sensitivity.                                                                                                           |
 | `single_match`            | `bool`                                  | `False`                                                  | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                         |
 
@@ -388,26 +496,29 @@
 @llm_tasks = "spacy.NER.v2"
 labels = PERSON,ORGANISATION,LOCATION
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "ner_examples.yml"
 ```
 
-If you don't have specific examples to provide to the LLM, you can write definitions for each label and provide them via the `label_definitions` argument. This lets you tell the LLM exactly what you're looking for rather than relying on the LLM to interpret its task given just the label name. Label descriptions are freeform so you can write whatever you want here, but through some experiments a brief description along with some examples and counter examples seems to work quite well.
+You can also write definitions for each label and provide them via the `label_definitions` argument. This lets you tell
+the LLM exactly what you're looking for rather than relying on the LLM to interpret its task given just the label name.
+Label descriptions are freeform so you can write whatever you want here, but through some experiments a brief
+description along with some examples and counter examples seems to work quite well.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
 labels = PERSON,SPORTS_TEAM
 [components.llm.task.label_definitions]
 PERSON = "Extract any named individual in the text."
 SPORTS_TEAM = "Extract the names of any professional sports team. e.g. Golden State Warriors, LA Lakers, Man City, Real Madrid"
 ```
 
-> Label descriptions can also be used with explicit examples to give as much info to the LLM backend as possible.
+> Label descriptions can also be used with explicit examples to give as much info to the LLM model as possible.
 
 #### spacy.NER.v1
 
 The original version of the built-in NER task supports both zero-shot and few-shot prompting.
 
 ```ini
 [components.llm.task]
@@ -473,15 +584,15 @@
 labels = ["PERSON", "ORGANISATION", "LOCATION"]
 examples = null
 ```
 
 | Argument                  | Type                                    | Default                                                            | Description                                                                                                                                           |
 | ------------------------- | --------------------------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `labels`                  | `Union[List[str], str]`                 |                                                                    | List of labels or str of comma-separated list of labels.                                                                                              |
-| `template`                | `str`                                   | [`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
+| `template`                | `str`                                   | [`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM model. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.                |
 | `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                             | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
 | `spans_key`               | `str`                                   | `"sc"`                                                             | Key of the `Doc.spans` dict to save the spans under.                                                                                                  |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                             | Optional function that generates examples for few-shot learning.                                                                                      |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                             | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
 | `alignment_mode`          | `str`                                   | `"contract"`                                                       | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
 | `case_sensitive_matching` | `bool`                                  | `False`                                                            | Whether to search without case sensitivity.                                                                                                           |
 | `single_match`            | `bool`                                  | `False`                                                            | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                         |
@@ -512,29 +623,86 @@
 | `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
 | `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
 
 Except for the `spans_key` parameter, the SpanCat task reuses the configuration
 from the NER task.
 Refer to [its documentation](#spacynerv1) for more insight.
 
+#### spacy.TextCat.v3
+
+Version 3 (the most recent) of the built-in TextCat task supports both zero-shot and few-shot prompting. It allows
+setting definitions of labels. Those definitions are included in the prompt.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.TextCat.v3"
+labels = ["COMPLIMENT", "INSULT"]
+label_definitions = {
+    "COMPLIMENT": "a polite expression of praise or admiration.",
+    "INSULT": "a disrespectful or scornfully abusive remark or act."
+}
+examples = null
+```
+
+| Argument            | Type                                    | Default                                                      | Description                                                                                                                                      |
+| ------------------- | --------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
+| `labels`            | `Union[List[str], str]`                 |                                                              | List of labels or str of comma-separated list of labels.                                                                                         |
+| `label_definitions` | `Optional[Dict[str, str]]`              | `None`                                                       | Dictionary of label definitions. Included in the prompt, if set.                                                                                 |
+| `template`          | `str`                                   | [`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.         |
+| `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                       | Optional function that generates examples for few-shot learning.                                                                                 |
+| `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                                       | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                             |
+| `exclusive_classes` | `bool`                                  | `False`                                                      | If set to `True`, only one label per document should be valid. If set to `False`, one document can have multiple labels.                         |
+| `allow_none`        | `bool`                                  | `True`                                                       | When set to `True`, allows the LLM to not return any of the given label. The resulting dict in `doc.cats` will have `0.0` scores for all labels. |
+| `verbose`           | `bool`                                  | `False`                                                      | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                             |
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```json
+[
+  {
+    "text": "You look great!",
+    "answer": "Compliment"
+  },
+  {
+    "text": "You are not very clever at all.",
+    "answer": "Insult"
+  }
+]
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.TextCat.v3"
+labels = ["COMPLIMENT", "INSULT"]
+label_definitions = {
+    "COMPLIMENT": "a polite expression of praise or admiration.",
+    "INSULT": "a disrespectful or scornfully abusive remark or act."
+}
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "textcat_examples.json"
+```
+
 #### spacy.TextCat.v2
 
-The built-in TextCat task supports both zero-shot and few-shot prompting.
+Version 2 of the built-in TextCat task supports both zero-shot and few-shot prompting and includes an improved prompt
+template.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
 labels = ["COMPLIMENT", "INSULT"]
 examples = null
 ```
 
 | Argument            | Type                                    | Default                                                      | Description                                                                                                                                      |
 | ------------------- | --------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
 | `labels`            | `Union[List[str], str]`                 |                                                              | List of labels or str of comma-separated list of labels.                                                                                         |
-| `template`          | `str`                                   | [`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.         |
+| `template`          | `str`                                   | [`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt template to send to LLM model. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.           |
 | `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                       | Optional function that generates examples for few-shot learning.                                                                                 |
 | `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                                       | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                             |
 | `exclusive_classes` | `bool`                                  | `False`                                                      | If set to `True`, only one label per document should be valid. If set to `False`, one document can have multiple labels.                         |
 | `allow_none`        | `bool`                                  | `True`                                                       | When set to `True`, allows the LLM to not return any of the given label. The resulting dict in `doc.cats` will have `0.0` scores for all labels. |
 | `verbose`           | `bool`                                  | `False`                                                      | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                             |
 
 To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
@@ -560,15 +728,15 @@
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "textcat_examples.json"
 ```
 
 #### spacy.TextCat.v1
 
-The original version of the built-in TextCat task supports both zero-shot and few-shot prompting.
+Version 1 of the built-in TextCat task supports both zero-shot and few-shot prompting.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v1"
 labels = COMPLIMENT,INSULT
 examples = null
 ```
@@ -614,58 +782,58 @@
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.REL.v1"
 labels = ["LivesIn", "Visits"]
 ```
 
-| Argument            | Type                                    | Default                                              | Description                                                                                                                              |
-| ------------------- | --------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`            | `Union[List[str], str]`                 |                                                      | List of labels or str of comma-separated list of labels.                                                                                 |
-| `template`          | `str`                                   | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
-| `label_description` | `Optional[Dict[str, str]]`              | `None`                                               | Dictionary providing a description for each relation label.                                                                              |
-| `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                               | Optional function that generates examples for few-shot learning.                                                                         |
-| `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                               | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                     |
-| `verbose`           | `bool`                                  | `False`                                              | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                     |
+| Argument            | Type                                    | Default                                              | Description                                                                                                                            |
+| ------------------- | --------------------------------------- | ---------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
+| `labels`            | `Union[List[str], str]`                 |                                                      | List of labels or str of comma-separated list of labels.                                                                               |
+| `template`          | `str`                                   | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) | Custom prompt template to send to LLM model. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
+| `label_description` | `Optional[Dict[str, str]]`              | `None`                                               | Dictionary providing a description for each relation label.                                                                            |
+| `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                               | Optional function that generates examples for few-shot learning.                                                                       |
+| `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                               | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                   |
+| `verbose`           | `bool`                                  | `False`                                              | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                   |
 
 To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
 The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
 
-```json
+```jsonl
 {"text": "Laura bought a house in Boston with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5, "label": "PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"}, {"start_char": 48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep": 0, "dest": 1, "relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation": "LivesIn"}]}
 {"text": "Michael travelled through South America by bike.", "ents": [{"start_char": 0, "end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label": "LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]}
 ```
 
-Note: the REL task relies on pre-extracted entities to make its prediction.
-Hence, you'll need to add a component that populates `doc.ents` with recognized
-spans to your spaCy pipeline and put it _before_ the REL component.
-
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.REL.v1"
 labels = ["LivesIn", "Visits"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "rel_examples.jsonl"
 ```
 
+Note: the REL task relies on pre-extracted entities to make its prediction.
+Hence, you'll need to add a component that populates `doc.ents` with recognized
+spans to your spaCy pipeline and put it _before_ the REL component.
+
 #### spacy.Lemma.v1
 
 The `Lemma.v1` task lemmatizes the provided text and updates the `lemma_` attribute in the doc's tokens accordingly.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.Lemma.v1"
 examples = null
 ```
 
-| Argument   | Type                                    | Default                                                | Description                                                                                                                              |
-| ---------- | --------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- |
-| `template` | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
-| `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                 | Optional function that generates examples for few-shot learning.                                                                         |
+| Argument   | Type                                    | Default                                                | Description                                                                                                                            |
+| ---------- | --------------------------------------- | ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
+| `template` | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM model. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
+| `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                 | Optional function that generates examples for few-shot learning.                                                                       |
 
 `Lemma.v1` prompts the LLM to lemmatize the passed text and return the lemmatized version as a list of tokens and their
 corresponding lemma. E. g. the text
 `I'm buying ice cream for my friends` should invoke the response
 
 ```
 I: I
@@ -710,162 +878,499 @@
 [components.llm.task]
 @llm_tasks = "spacy.Lemma.v1"
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "lemma_examples.yml"
 ```
 
+#### spacy.Sentiment.v1
+
+Performs sentiment analysis on provided texts. Scores between 0 and 1 are stored in `Doc._.sentiment` - the higher, the
+more positive. Note in cases of parsing issues (e. g. in case of unexpected LLM responses) the value might be `None`.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.Sentiment.v1"
+examples = null
+```
+
+| Argument   | Type                                    | Default                                                        | Description                                                                                                                            |
+| ---------- | --------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
+| `template` | `str`                                   | [sentiment.jinja](./spacy_llm/tasks/templates/sentiment.jinja) | Custom prompt template to send to LLM model. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
+| `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                         | Optional function that generates examples for few-shot learning.                                                                       |
+| `field`    | `str`                                   | `sentiment`                                                    | Name of extension attribute to store summary in (i. e. the summary will be available in `doc._.{field}`).                              |
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```yaml
+- text: "This is horrifying."
+  score: 0
+- text: "This is underwhelming."
+  score: 0.25
+- text: "This is ok."
+  score: 0.5
+- text: "I'm looking forward to this!"
+  score: 1.0
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.Sentiment.v1"
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "sentiment_examples.yml"
+```
+
 #### spacy.NoOp.v1
 
 This task is only useful for testing - it tells the LLM to do nothing, and does not set any fields on the `docs`.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
 ```
 
-### Backends
+### Models
 
-A _backend_ defines which LLM model to query, and how to query it. It can be a simple function taking a collection
+A _model_ defines which LLM model to query, and how to query it. It can be a simple function taking a collection
 of prompts (consistent with the output type of `task.generate_prompts()`) and returning a collection of responses
 (consistent with the expected input of `parse_responses`). Generally speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
 but specific implementations can have other signatures, like `Callable[[Iterable[str]], Iterable[str]]`.
 
-All built-in backends are registered in `llm_backends`. If no backend is specified, the repo currently connects to the [`OpenAI` API](#openai) by default,
-using the built-in REST protocol, and accesses the `"gpt-3.5-turbo"` model.
+All built-in models are registered in `llm_models`. If no model is specified, the repo currently connects to the `OpenAI` API by default
+using REST, and accesses the `"gpt-3.5-turbo"` model.
+
+Currently three different approaches to use LLMs are supported:
+
+1. `spacy-llm`s native REST backend. This is the default for all hosted models (e. g. OpenAI, Cohere, Anthropic, ...).
+2. A HuggingFace integration that allows to run a limited set of HF models locally.
+3. A LangChain integration that allows to run any model supported by LangChain (hosted or locally).
+
+Approaches 1. and 2 are the default for hosted model and local models, respectively. Alternatively you can use LangChain
+to access hosted or local models by specifying one of the models registered with the `langchain.` prefix.
 
-> :question: _Why are there backends for third-party libraries in addition to a native REST backend and which should
-> I choose?_
+> :question: Why LangChain if there are also are a native REST and a HuggingFace backend? When should I use what?
 >
-> Third-party libraries like `langchain` or `minichain` focus on prompt management, integration of many different LLM
+> Third-party libraries like `langchain` focus on prompt management, integration of many different LLM
 > APIs, and other related features such as conversational memory or agents. `spacy-llm` on the other hand emphasizes
 > features we consider useful in the context of NLP pipelines utilizing LLMs to process documents (mostly) independent
-> from each other. It makes sense that the feature set of such third-party libraries and `spacy-llm` is not identical -
+> from each other. It makes sense that the feature sets of such third-party libraries and `spacy-llm` aren't identical -
 > and users might want to take advantage of features not available in `spacy-llm`.
 >
-> The advantage of offering our own REST backend is that we can ensure a larger degree of stability of robustness, as
+> The advantage of implementing our own REST and HuggingFace integrations is that we can ensure a larger degree of stability and robustness, as
 > we can guarantee backwards-compatibility and more smoothly integrated error handling.
 >
-> Ultimately we recommend trying to implement your use case using the REST backend first (which is configured as the
-> default backend). If however there are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
-> backend of a third-party library - and easy to customize the prompting mechanism, if so required.
+> If however there are features or APIs not natively covered by `spacy-llm`, it's trivial to utilize LangChain to cover
+> this - and easy to customize the prompting mechanism, if so required.
 
-#### OpenAI
+Note that when using hosted services, you have to ensure that the proper API keys are set as environment variables as
+described by the corresponding provider's documentation.
 
-When the backend uses OpenAI, you have to get an API key from openai.com, and ensure that the keys are set as
+E. g. when using OpenAI, you have to get an API key from openai.com, and ensure that the keys are set as
 environmental variables:
 
 ```shell
 export OPENAI_API_KEY="sk-..."
 export OPENAI_API_ORG="org-..."
 ```
 
-#### spacy.REST.v1
+For Cohere it's
 
-This default backend uses `requests` and a simple retry mechanism to access an API.
+```shell
+export CO_API_KEY="..."
+```
+
+and for Anthropic
+
+```shell
+export ANTHROPIC_API_KEY="..."
+```
+
+#### spacy.GPT-4.v1
+
+OpenAI's `gpt-4` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.GPT-4.v1"
+name = "gpt-4"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                                                            | Default   | Description                                                                                                          |
+| ----------- | --------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["gpt-4", "gpt-4-0314", "gpt-4-32k", "gpt-4-32k-0314"]` | `"gpt-4"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`                                                | `{}`      | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                                                          | `True`    | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                                                           | `3`       | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                                                           | `30`      | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.GPT-3-5.v1
+
+OpenAI's `gpt-3-5` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.GPT-3-5.v1"
+name = "gpt-3.5-turbo"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                                                                                            | Default           | Description                                                                                                          |
+| ----------- | ----------------------------------------------------------------------------------------------- | ----------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["gpt-3.5-turbo", "gpt-3.5-turbo-16k", "gpt-3.5-turbo-0613", "gpt-3.5-turbo-0613-16k"]` | `"gpt-3.5-turbo"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`                                                                                | `{}`              | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                                                                                          | `True`            | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                                                                                           | `3`               | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                                                                                           | `30`              | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Text-Davinci.v1
+
+OpenAI's `text-davinci` model family.
+
+Example config:
 
 ```ini
-[components.llm.backend]
-@llm_backends = "spacy.REST.v1"
-api = "OpenAI"
-config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
+[components.llm.model]
+@llm_models = "spacy.Text-Davinci.v1"
+name = "text-davinci-003"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                                              | Default              | Description                                                                                                          |
+| ----------- | ------------------------------------------------- | -------------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["text-davinci-002", "text-davinci-003"]` | `"text-davinci-003"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`                                  | `{}`                 | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                                            | `True`               | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                                             | `3`                  | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                                             | `30`                 | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Code-Davinci.v1
+
+OpenAI's `code-davinci` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Code-Davinci.v1"
+name = "code-davinci-002"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                          | Default              | Description                                                                                                          |
+| ----------- | ----------------------------- | -------------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["code-davinci-002"]` | `"code-davinci-002"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`              | `{}`                 | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                        | `True`               | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                         | `3`                  | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                         | `30`                 | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Text-Curie.v1
+
+OpenAI's `text-curie` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Text-Curie.v1"
+name = "text-curie-001"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                        | Default            | Description                                                                                                          |
+| ----------- | --------------------------- | ------------------ | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["text-curie-001"]` | `"text-curie-001"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`            | `{}`               | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                      | `True`             | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                       | `3`                | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                       | `30`               | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Text-Babbage.v1
+
+OpenAI's `text-babbage` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Text-Babbage.v1"
+name = "text-babbage-001"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                          | Default              | Description                                                                                                          |
+| ----------- | ----------------------------- | -------------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["text-babbage-001"]` | `"text-babbage-001"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`              | `{}`                 | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                        | `True`               | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                         | `3`                  | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                         | `30`                 | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Text-Ada.v1
+
+OpenAI's `text-ada` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Text-Ada.v1"
+name = "text-ada-001"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                      | Default          | Description                                                                                                          |
+| ----------- | ------------------------- | ---------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["text-ada-001"]` | `"text-ada-001"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`          | `{}`             | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                    | `True`           | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                     | `3`              | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                     | `30`             | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Davinci.v1
+
+OpenAI's `davinci` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Davinci.v1 "
+name = "davinci"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                 | Default     | Description                                                                                                          |
+| ----------- | -------------------- | ----------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["davinci"]` | `"davinci"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`     | `{}`        | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`               | `True`      | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                | `3`         | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                | `30`        | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Curie.v1
+
+OpenAI's `curie` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Curie.v1 "
+name = "curie"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type               | Default   | Description                                                                                                          |
+| ----------- | ------------------ | --------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["curie"]` | `"curie"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`   | `{}`      | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`             | `True`    | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`              | `3`       | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`              | `30`      | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Babbage.v1
+
+OpenAI's `babbage` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Babbage.v1 "
+name = "babbage"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                 | Default     | Description                                                                                                          |
+| ----------- | -------------------- | ----------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["babbage"]` | `"babbage"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`     | `{}`        | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`               | `True`      | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                | `3`         | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                | `30`        | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Ada.v1
+
+OpenAI's `ada` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Ada.v1 "
+name = "ada"
+config = {"temperature": 0.3}
 ```
 
 | Argument    | Type             | Default | Description                                                                                                          |
 | ----------- | ---------------- | ------- | -------------------------------------------------------------------------------------------------------------------- |
-| `api`       | `str`            |         | The name of a supported API. In v.0.1.0, only "OpenAI" is supported.                                                 |
-| `config`    | `Dict[Any, Any]` | `{}`    | Further configuration passed on to the backend.                                                                      |
+| `name`      | `Literal["ada"]` | `"ada"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]` | `{}`    | Further configuration passed on to the model.                                                                        |
 | `strict`    | `bool`           | `True`  | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
 | `max_tries` | `int`            | `3`     | Max. number of tries for API request.                                                                                |
 | `timeout`   | `int`            | `30`    | Timeout for API request in seconds.                                                                                  |
 
-When `api` is set to `OpenAI`, the following settings can be defined in the `config` dictionary:
+#### spacy.Command.v1
 
-- `model`: one of the following list of supported models:
-  - `"gpt-4"`
-  - `"gpt-4-0314"`
-  - `"gpt-4-32k"`
-  - `"gpt-4-32k-0314"`
-  - `"gpt-3.5-turbo"`
-  - `"gpt-3.5-turbo-0301"`
-  - `"text-davinci-003"`
-  - `"text-davinci-002"`
-  - `"text-curie-001"`
-  - `"text-babbage-001"`
-  - `"text-ada-001"`
-  - `"davinci"`
-  - `"curie"`
-  - `"babbage"`
-  - `"ada"`
-- `url`: By default, this is `https://api.openai.com/v1/completions`. For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/completions`.
+Cohere's `command` model family.
 
-#### spacy.MiniChain.v1
+Example config:
 
-To use [MiniChain](https://github.com/srush/MiniChain) for the API retrieval part, make sure you have installed it first:
+```ini
+[components.llm.model]
+@llm_models = "spacy.Command.v1 "
+name = "command"
+config = {"temperature": 0.3}
+```
 
-```shell
-python -m pip install "minichain>=0.3,<0.4"
-# Or install with spacy-llm directly
-python -m pip install "spacy-llm[minichain]"
+| Argument    | Type                                                                              | Default     | Description                                                                                                          |
+| ----------- | --------------------------------------------------------------------------------- | ----------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["command", "command-light", "command-light-nightly", "command-nightly"]` | `"command"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`                                                                  | `{}`        | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                                                                            | `True`      | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                                                                             | `3`         | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                                                                             | `30`        | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Claude-1.v1
+
+Anthropic's `claude-1` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Claude-1.v1 "
+name = "claude-1"
+config = {"temperature": 0.3}
 ```
 
-Note that MiniChain currently only supports Python 3.8, 3.9 and 3.10.
+| Argument    | Type                                   | Default      | Description                                                                                                          |
+| ----------- | -------------------------------------- | ------------ | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["claude-1", "claude-1-100k"]` | `"claude-1"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`                       | `{}`         | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                                 | `True`       | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                                  | `3`          | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                                  | `30`         | Timeout for API request in seconds.                                                                                  |
 
-Example config blocks:
+#### spacy.Claude-instant-1.v1
+
+Anthropic's `claude-instant-1` model family.
+
+Example config:
 
 ```ini
-[components.llm.backend]
-@llm_backends = "spacy.MiniChain.v1"
-api = "OpenAI"
+[components.llm.model]
+@llm_models = "spacy.Claude-instant-1.v1 "
+name = "claude-instant-1"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                                                   | Default              | Description                                                                                                          |
+| ----------- | ------------------------------------------------------ | -------------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["claude-instant-1", "claude-instant-1-100k"]` | `"claude-instant-1"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`                                       | `{}`                 | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                                                 | `True`               | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                                                  | `3`                  | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                                                  | `30`                 | Timeout for API request in seconds.                                                                                  |
 
-[components.llm.backend.query]
-@llm_queries = "spacy.RunMiniChain.v1"
+#### spacy.Claude-instant-1-1.v1
+
+Anthropic's `claude-instant-1.1` model family.
+
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Claude-instant-1-1.v1 "
+name = "claude-instant-1.1"
+config = {"temperature": 0.3}
 ```
 
-| Argument | Type                                                                              | Default | Description                                                                         |
-| -------- | --------------------------------------------------------------------------------- | ------- | ----------------------------------------------------------------------------------- |
-| `api`    | `str`                                                                             |         | The name of an API supported by MiniChain, e.g. "OpenAI".                           |
-| `config` | `Dict[Any, Any]`                                                                  | `{}`    | Further configuration passed on to the backend.                                     |
-| `query`  | `Optional[Callable[["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None`  | Function that executes the prompts. If `None`, defaults to `spacy.RunMiniChain.v1`. |
+| Argument    | Type                                                       | Default                | Description                                                                                                          |
+| ----------- | ---------------------------------------------------------- | ---------------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["claude-instant-1.1", "claude-instant-1.1-100k"]` | `"claude-instant-1.1"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`                                           | `{}`                   | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                                                     | `True`                 | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                                                      | `3`                    | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                                                      | `30`                   | Timeout for API request in seconds.                                                                                  |
 
-The default `query` (`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()` for each given textual prompt.
+#### spacy.Claude-1-0.v1
 
-#### spacy.LangChain.v1
+Anthropic's `claude-1.0` model family.
 
-To use [LangChain](https://github.com/hwchase17/langchain) for the API retrieval part, make sure you have installed it first:
+Example config:
 
-```shell
-python -m pip install "langchain>=0.0.144,<0.1"
-# Or install with spacy-llm directly
-python -m pip install "spacy-llm[langchain]"
+```ini
+[components.llm.model]
+@llm_models = "spacy.Claude-1-0.v1 "
+name = "claude-1.0"
+config = {"temperature": 0.3}
 ```
 
-Note that LangChain currently only supports Python 3.9 and beyond.
+| Argument    | Type                    | Default        | Description                                                                                                          |
+| ----------- | ----------------------- | -------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["claude-1.0"]` | `"claude-1.0"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`        | `{}`           | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                  | `True`         | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                   | `3`            | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                   | `30`           | Timeout for API request in seconds.                                                                                  |
 
-Example config block:
+#### spacy.Claude-1-2.v1
+
+Anthropic's `claude-1.2` model family.
+
+Example config:
 
 ```ini
-[components.llm.backend]
-@llm_backends = "spacy.LangChain.v1"
-api = "OpenAI"
-query = {"@llm_queries": "spacy.CallLangChain.v1"}
+[components.llm.model]
+@llm_models = "spacy.Claude-1-2.v1 "
+name = "claude-1.2"
 config = {"temperature": 0.3}
 ```
 
-| Argument | Type                                                                           | Default | Description                                                                          |
-| -------- | ------------------------------------------------------------------------------ | ------- | ------------------------------------------------------------------------------------ |
-| `api`    | `str`                                                                          |         | The name of an API supported by LangChain, e.g. "OpenAI".                            |
-| `config` | `Dict[Any, Any]`                                                               | `{}`    | Further configuration passed on to the backend.                                      |
-| `query`  | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None`  | Function that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
+| Argument    | Type                    | Default        | Description                                                                                                          |
+| ----------- | ----------------------- | -------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["claude-1.2"]` | `"claude-1.2"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`        | `{}`           | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                  | `True`         | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                   | `3`            | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                   | `30`           | Timeout for API request in seconds.                                                                                  |
 
-The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for each given textual prompt.
+#### spacy.Claude-1-3.v1
 
-#### spacy.Dolly_HF.v1
+Anthropic's `claude-1.3` model family.
 
-To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
+Example config:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.Claude-1-3.v1 "
+name = "claude-1.3"
+config = {"temperature": 0.3}
+```
+
+| Argument    | Type                                       | Default        | Description                                                                                                          |
+| ----------- | ------------------------------------------ | -------------- | -------------------------------------------------------------------------------------------------------------------- |
+| `name`      | `Literal["claude-1.3", "claude-1.3-100k"]` | `"claude-1.3"` | Model name, i. e. any supported variant for this particular model.                                                   |
+| `config`    | `Dict[Any, Any]`                           | `{}`           | Further configuration passed on to the model.                                                                        |
+| `strict`    | `bool`                                     | `True`         | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
+| `max_tries` | `int`                                      | `3`            | Max. number of tries for API request.                                                                                |
+| `timeout`   | `int`                                      | `30`           | Timeout for API request in seconds.                                                                                  |
+
+#### spacy.Dolly.v1
+
+To use this model, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
 This allows you to have the setting `device=cuda:0` in your config, which ensures that the model is loaded entirely on the GPU (and fails otherwise).
 
 You can do so with
 
 ```shell
 python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ```
@@ -876,38 +1381,39 @@
 ```shell
 python -m pip install "accelerate>=0.16.0,<1.0"
 ```
 
 Example config block:
 
 ```ini
-[components.llm.backend]
-@llm_backends = "spacy.Dolly_HF.v1"
-model = "databricks/dolly-v2-3b"
+[components.llm.model]
+@llm_models = "spacy.Dolly.v1"
+name = "dolly-v2-3b"
 ```
 
-| Argument      | Type             | Default | Description                                                                                      |
-| ------------- | ---------------- | ------- | ------------------------------------------------------------------------------------------------ |
-| `model`       | `str`            |         | The name of a Dolly model that is supported.                                                     |
-| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.pipeline()`. |
-| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                               |
+| Argument      | Type                                                    | Default | Description                                                                                      |
+| ------------- | ------------------------------------------------------- | ------- | ------------------------------------------------------------------------------------------------ |
+| `name`        | `Literal["dolly-v2-3b", "dolly-v2-7b", "dolly-v2-12b"]` |         | The name of a Dolly model that is supported (e. g. "dolly-v2-3b" or "dolly-v2-12b").             |
+| `config_init` | `Dict[str, Any]`                                        | `{}`    | Further configuration passed on to the construction of the model with `transformers.pipeline()`. |
+| `config_run`  | `Dict[str, Any]`                                        | `{}`    | Further configuration used during model inference.                                               |
 
 Supported models (see the [Databricks models page](https://huggingface.co/databricks) on Hugging Face for details):
 
 - `"databricks/dolly-v2-3b"`
 - `"databricks/dolly-v2-7b"`
 - `"databricks/dolly-v2-12b"`
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
-#### spacy.StableLM_HF.v1
+#### spacy.Falcon.v1
 
 To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
+This allows you to have the setting `device=cuda:0` in your config, which ensures that the model is loaded entirely on the GPU (and fails otherwise).
 
 You can do so with
 
 ```shell
 python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ```
 
@@ -917,39 +1423,69 @@
 ```shell
 python -m pip install "accelerate>=0.16.0,<1.0"
 ```
 
 Example config block:
 
 ```ini
-[components.llm.backend]
-@llm_backends = "spacy.StableLM_HF.v1"
-model = "stabilityai/stablelm-tuned-alpha-7b"
-```
-
-| Argument      | Type             | Default | Description                                                                                                                  |
-| ------------- | ---------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
-| `model`       | `str`            |         | The name of a StableLM model that is supported.                                                                              |
-| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
-| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                                                           |
-
-Supported models (see the [Stability AI StableLM GitHub repo](https://github.com/Stability-AI/StableLM/#stablelm-alpha) for details):
-
-- `"stabilityai/stablelm-base-alpha-3b"`
-- `"stabilityai/stablelm-base-alpha-7b"`
-- `"stabilityai/stablelm-tuned-alpha-3b"`
-- `"stabilityai/stablelm-tuned-alpha-7b"`
+[components.llm.model]
+@llm_models = "spacy.Falcon.v1"
+name = "falcon-7b"
+```
+
+| Argument      | Type                                                                                | Default         | Description                                                                                      |
+| ------------- | ----------------------------------------------------------------------------------- | --------------- | ------------------------------------------------------------------------------------------------ |
+| `name`        | `Literal["falcon-rw-1b", "falcon-7b", "falcon-7b-instruct", "falcon-40b-instruct"]` | `"7b-instruct"` | The name of a Falcon model variant that is supported.                                            |
+| `config_init` | `Dict[str, Any]`                                                                    | `{}`            | Further configuration passed on to the construction of the model with `transformers.pipeline()`. |
+| `config_run`  | `Dict[str, Any]`                                                                    | `{}`            | Further configuration used during model inference.                                               |
+
+Note that Hugging Face will download this model the first time you use it - you can
+[define the cache directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
+by setting the environmental variable `HF_HOME`.
+
+#### spacy.StableLM.v1
+
+To use this model, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
+
+You can do so with
+
+```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
+```
+
+If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries.
+
+```shell
+python -m pip install "accelerate>=0.16.0,<1.0"
+```
+
+Example config block:
+
+```ini
+[components.llm.model]
+@llm_models = "spacy.StableLM.v1"
+name = "stablelm-tuned-alpha-7b"
+```
+
+| Argument      | Type                                                                                                                | Default | Description                                                                                                                  |
+| ------------- | ------------------------------------------------------------------------------------------------------------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `name`        | `Literal["stablelm-base-alpha-3b", "stablelm-base-alpha-7b", "stablelm-tuned-alpha-3b", "stablelm-tuned-alpha-7b"]` |         | The name of a StableLM model that is supported (e. g. "stablelm-tuned-alpha-7b").                                            |
+| `config_init` | `Dict[str, Any]`                                                                                                    | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]`                                                                                                    | `{}`    | Further configuration used during model inference.                                                                           |
+
+See the [Stability AI StableLM GitHub repo](https://github.com/Stability-AI/StableLM/#stablelm-alpha) for details.
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
-#### spacy.OpenLLaMaHF.v1
+#### spacy.OpenLLaMA.v1
 
-To use this backend, ideally you have a GPU enabled and have installed
+To use this model, ideally you have a GPU enabled and have installed
 
 - `transformers[sentencepiece]`
 - `torch`
 - CUDA
   in your virtual environment.
 
 You can do so with
@@ -964,57 +1500,99 @@
 ```shell
 python -m pip install "accelerate>=0.16.0,<1.0"
 ```
 
 Example config block:
 
 ```ini
-[components.llm.backend]
-@llm_backends = "spacy.OpenLLaMaHF.v1"
-model = "openlm-research/open_llama_3b_350bt_preview"
-```
-
-| Argument      | Type             | Default | Description                                                                                                                  |
-| ------------- | ---------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
-| `model`       | `str`            |         | The name of a OpenLLaMa model that is supported.                                                                             |
-| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
-| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                                                           |
-
-Supported models (see the [OpenLM Research OpenLLaMa GitHub repo](https://github.com/openlm-research/open_llama) for details):
-
-- `"openlm-research/open_llama_3b_350bt_preview"`
-- `"openlm-research/open_llama_3b_600bt_preview"`
-- `"openlm-research/open_llama_7b_400bt_preview"`
-- `"openlm-research/open_llama_7b_700bt_preview"`
+[components.llm.model]
+@llm_models = "spacy.OpenLLaMA.v1"
+name = "open_llama_3b_350bt_preview"
+```
+
+| Argument      | Type                                                                                                                                  | Default | Description                                                                                                                  |
+| ------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `name`        | `Literal["open_llama_3b_350bt_preview", "open_llama_3b_600bt_preview", "open_llama_7b_400bt_preview", "open_llama_7b_600bt_preview"]` |         | The name of a OpenLLaMA model that is supported (e. g. "open_llama_3b_350bt_preview").                                       |
+| `config_init` | `Dict[str, Any]`                                                                                                                      | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]`                                                                                                                      | `{}`    | Further configuration used during model inference.                                                                           |
+
+See the [OpenLM Research OpenLLaMA GitHub repo](https://github.com/openlm-research/open_llama) for details.
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
+#### LangChain models
+
+To use [LangChain](https://github.com/hwchase17/langchain) for the API retrieval part, make sure you have installed it first:
+
+```shell
+python -m pip install "langchain==0.0.191"
+# Or install with spacy-llm directly
+python -m pip install "spacy-llm[extras]"
+```
+
+Note that LangChain currently only supports Python 3.9 and beyond.
+
+LangChain models in `spacy-llm` work slightly differently. `langchain`'s models are parsed automatically, each
+LLM class in `langchain` has one entry in `spacy-llm`'s registry. As `langchain`'s design has one class per API and
+not per model, this results in registry entries like `langchain.OpenAI.v1` - i. e. there is one registry entry per API
+and not per model (family), as for the REST- and HuggingFace-based entries.
+
+The name of the model to be used has to be passed in via the `name` attribute.
+
+Example config block:
+
+```ini
+[components.llm.model]
+@llm_models = "langchain.OpenAI.v1"
+name = "gpt-3.5-turbo"
+query = {"@llm_queries": "spacy.CallLangChain.v1"}
+config = {"temperature": 0.3}
+```
+
+| Argument | Type                                                                           | Default | Description                                                                          |
+| -------- | ------------------------------------------------------------------------------ | ------- | ------------------------------------------------------------------------------------ |
+| `name`   | `str`                                                                          |         | The name of a mdodel supported by LangChain for this API.                            |
+| `config` | `Dict[Any, Any]`                                                               | `{}`    | Configuration passed on to the LangChain model.                                      |
+| `query`  | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None`  | Function that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
+
+The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for each given textual prompt.
+
 ### Cache
 
 Interacting with LLMs, either through an external API or a local instance, is costly.
 Since developing an NLP pipeline generally means a lot of exploration and prototyping,
 `spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run
-that keeps batches of documents stored on disk.
+that keeps batches of documents stored on disk. 
+
+The cache implementation also ensures that documents in one cache directory were all produced using the same prompt 
+template. This is only possible however if the specified task implements 
+```python
+@property
+def prompt_template() -> str:
+    ...
+``` 
+which returns the raw prompt template as string. If `prompt_template()` isn't implemented, the cache will emit a warning
+and not check for prompt template consistency.
 
 Example config block:
 
 ```ini
 [components.llm.cache]
 @llm_misc = "spacy.BatchCache.v1"
 path = "path/to/cache"
 batch_size = 64
 max_batches_in_mem = 4
 ```
 
 | Argument             | Type                         | Default | Description                                                                                                               |
 | -------------------- | ---------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------- |
 | `path`               | `Optional[Union[str, Path]]` | `None`  | Cache directory. If `None`, no caching is performed, and this component will act as a NoOp.                               |
-| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file). Once a batch is full, it will be peristed to disk.                                    |
+| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file). Once a batch is full, it will be persisted to disk.                                   |
 | `max_batches_in_mem` | `int`                        | 4       | Max. number of batches to hold in memory. Allows you to limit the effect on your memory if you're handling a lot of docs. |
 
 When retrieving a document, the `BatchCache` will first figure out what batch the document belongs to. If the batch
 isn't in memory it will try to load the batch from disk and then move it into memory. 
 
 Note that since the cache is generated by a registered function, you can also provide your own registered function
 returning your own cache implementation. If you wish to do so, ensure that your cache object adheres to the
@@ -1074,7 +1652,11 @@
 PRs are always welcome!
 
 ## 📝️ Reporting issues
 
 If you have questions regarding the usage of `spacy-llm`, or want to give us feedback after giving it a spin, please use the
 [discussion board](https://github.com/explosion/spaCy/discussions).
 Bug reports can be filed on the [spaCy issue tracker](https://github.com/explosion/spaCy/issues). Thank you!
+
+## Migration guides
+
+Please refer to our [migration guide](migration_guide.md).
```

#### html2text {}

```diff
@@ -1,23 +1,38 @@
-[https://explosion.ai/assets/img/logo.svg] # spacy-llm: Integrating LLMs into
-structured NLP pipelines [![GitHub Workflow Status](https://img.shields.io/
-github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)]
-(https://github.com/explosion/spacy-llm/actions/workflows/test.yml) [![pypi
-Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-
-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/) [![Code
-style: black](https://img.shields.io/badge/code%20style-black-
-000000.svg?style=flat-square)](https://github.com/ambv/black) This package
-integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.0 Summary: Integrating LLMs
+into structured NLP pipelines Author: Explosion Author-email:
+contact@explosion.ai License: MIT Project-URL: Release notes, https://
+github.com/explosion/spacy-llm/releases Project-URL: Source, https://
+github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
+Content-Type: text/markdown Provides-Extra: langchain Provides-Extra:
+transformers License-File: LICENSE [https://explosion.ai/assets/img/logo.svg] #
+spacy-llm: Integrating LLMs into structured NLP pipelines [![GitHub Workflow
+Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-
+llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/
+workflows/test.yml) [![pypi Version](https://img.shields.io/pypi/v/spacy-
+llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/
+spacy-llm/) [![Code style: black](https://img.shields.io/badge/code%20style-
+black-000000.svg?style=flat-square)](https://github.com/ambv/black) This
+package integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
 featuring a modular system for **fast prototyping** and **prompting**, and
 turning unstructured responses into **robust outputs** for various NLP tasks,
 **no training data** required. - Serializable `llm` **component** to integrate
 prompts into your pipeline - **Modular functions** to define the [**task**]
-(#tasks) (prompting and parsing) and [**backend**](#backends) (model to use) -
-Support for **hosted APIs** and self-hosted **open-source models** -
-Integration with [`MiniChain`](https://github.com/srush/MiniChain) and
+(#tasks) (prompting and parsing) and [**model**](#models) - Support for
+**hosted APIs** and self-hosted **open-source models** - Integration with
 [`LangChain`](https://github.com/hwchase17/langchain) - Access to **[OpenAI
 API](https://platform.openai.com/docs/api-reference/introduction)**, including
 GPT-4 and various GPT-3 models - Built-in support for **open-source [Dolly]
 (https://huggingface.co/databricks)** models hosted on Hugging Face - Usage
 examples for **Named Entity Recognition** and **Text Classification** - Easy
 implementation of **your own functions** via [spaCy's registry](https://
 spacy.io/api/top-level#registry) for custom prompting, parsing and model
@@ -50,74 +65,72 @@
 before-and-after tasks are much easier with a mature and well-thought-out
 library, which is exactly what spaCy provides. ## â³ Install `spacy-llm` will
 be installed automatically in future spaCy versions. For now, you can run the
 following in the same virtual environment where you already have `spacy`
 [installed](https://spacy.io/usage). ```bash python -m pip install spacy-llm
 ``` > â ï¸ This package is still experimental and it is possible that changes
 made to the interface will be breaking in minor version updates. ## ð Usage
-The task and the backend have to be supplied to the `llm` pipeline component
+The task and the model have to be supplied to the `llm` pipeline component
 using [spaCy's config system](https://spacy.io/api/data-formats#config). This
 package provides various built-in functionality, as detailed in the [API](#-
 api) documentation. ### Example 1: Add a text classifier using a GPT-3 model
 from OpenAI Create a new API key from openai.com or fetch an existing one, and
 ensure the keys are set as environmental variables. For more background
 information, see the [OpenAI](#openai) section. Create a config file
 `config.cfg` containing at least the following (or see the full example [here]
 (usage_examples/textcat_openai)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"] [components.llm.backend]
-@llm_backends = "spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-
-turbo", "temperature": 0.3} ``` Now run: ```python from spacy_llm.util import
-assemble nlp = assemble("config.cfg") doc = nlp("You look gorgeous!") print
-(doc.cats) ``` ### Example 2: Add NER using an open-source model through
-Hugging Face To run this example, ensure that you have a GPU enabled, and
-`transformers`, `torch` and CUDA installed. For more background information,
-see the [DollyHF](#spacydollyhfv1) section. Create a config file `config.cfg`
-containing at least the following (or see the full example [here]
-(usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline = ["llm"]
-[components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"]
-[components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1" # For better
-performance, use databricks/dolly-v2-12b instead model = "databricks/dolly-v2-
-3b" ``` Now run: ```python from spacy_llm.util import assemble nlp = assemble
-("config.cfg") doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
-print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that Hugging Face
-will download the `"databricks/dolly-v2-3b"` model the first time you use it.
-You can [define the cached directory](https://huggingface.co/docs/
-huggingface_hub/main/en/guides/manage-cache) by setting the environmental
-variable `HF_HOME`. Also, you can upgrade the model to be `"databricks/dolly-
-v2-12b"` for better performance. ### Example 3: Create the component directly
-in Python The `llm` component behaves as any other spaCy component does, so
-adding it to an existing pipeline follows the same pattern: ```python import
-spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config={ "task":
-{ "@llm_tasks": "spacy.NER.v2", "labels": ["PERSON", "ORGANISATION",
-"LOCATION"] }, "backend": { "@llm_backends": "spacy.REST.v1", "api": "OpenAI",
-"config": {"model": "gpt-3.5-turbo"}, }, }, ) nlp.initialize() doc = nlp("Jack
-and Jill rode up the hill in Les Deux Alpes") print([(ent.text, ent.label_) for
-ent in doc.ents]) ``` Note that for efficient usage of resources, typically you
-would use [`nlp.pipe(docs)`](https://spacy.io/api/language#pipe) with a batch,
-instead of calling `nlp(doc)` with a single document. ### Example 4: Implement
-your own custom task To write a [`task`](#tasks), you need to implement two
-functions: `generate_prompts` that takes a list of spaCy [`Doc`](https://
-spacy.io/api/doc) objects and transforms them into a list of prompts, and
-`parse_responses` that transforms the LLM outputs into annotations on the
-[`Doc`](https://spacy.io/api/doc), e.g. entity spans, text categories and more.
-To register your custom task with spaCy, decorate a factory function using the
-`spacy_llm.registry.llm_tasks` decorator with a custom name that you can refer
-to in your config. > ð For more details, see the [**usage example on writing
-your own task**](usage_examples/README.md#writing-your-own-task) ```python from
-typing import Iterable, List from spacy.tokens import Doc from
-spacy_llm.registry import registry from spacy_llm.util import split_labels
-@registry.llm_tasks("my_namespace.MyTask.v1") def make_my_task(labels: str,
-my_other_config_val: float) -> "MyTask": labels_list = split_labels(labels)
-return MyTask(labels=labels_list, my_other_config_val=my_other_config_val)
-class MyTask: def __init__(self, labels: List[str], my_other_config_val:
-float): ... def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
-... def parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] )
--> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
+= "spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"] [components.llm.model]
+@llm_models = "spacy.GPT-3-5.v1" config = {"temperature": 0.3} ``` Now run:
+```python from spacy_llm.util import assemble nlp = assemble("config.cfg") doc
+= nlp("You look gorgeous!") print(doc.cats) ``` ### Example 2: Add NER using an
+open-source model through Hugging Face To run this example, ensure that you
+have a GPU enabled, and `transformers`, `torch` and CUDA installed. For more
+background information, see the [DollyHF](#spacydollyhfv1) section. Create a
+config file `config.cfg` containing at least the following (or see the full
+example [here](usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline =
+["llm"] [components] [components.llm] factory = "llm" [components.llm.task]
+@llm_tasks = "spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"]
+[components.llm.model] @llm_models = "spacy.Dolly.v1" # For better performance,
+use dolly-v2-12b instead name = "dolly-v2-3b" ``` Now run: ```python from
+spacy_llm.util import assemble nlp = assemble("config.cfg") doc = nlp("Jack and
+Jill rode up the hill in Les Deux Alpes") print([(ent.text, ent.label_) for ent
+in doc.ents]) ``` Note that Hugging Face will download the `"databricks/dolly-
+v2-3b"` model the first time you use it. You can [define the cached directory]
+(https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by
+setting the environmental variable `HF_HOME`. Also, you can upgrade the model
+to be `"databricks/dolly-v2-12b"` for better performance. ### Example 3: Create
+the component directly in Python The `llm` component behaves as any other spaCy
+component does, so adding it to an existing pipeline follows the same pattern:
+```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config=
+{ "task": { "@llm_tasks": "spacy.NER.v2", "labels": ["PERSON", "ORGANISATION",
+"LOCATION"] }, "model": { "@llm_models": "spacy.gpt-3.5.v1", }, }, )
+nlp.initialize() doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
+print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient
+usage of resources, typically you would use [`nlp.pipe(docs)`](https://
+spacy.io/api/language#pipe) with a batch, instead of calling `nlp(doc)` with a
+single document. ### Example 4: Implement your own custom task To write a
+[`task`](#tasks), you need to implement two functions: `generate_prompts` that
+takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
+them into a list of prompts, and `parse_responses` that transforms the LLM
+outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity
+spans, text categories and more. To register your custom task with spaCy,
+decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator
+with a custom name that you can refer to in your config. > ð For more
+details, see the [**usage example on writing your own task**](usage_examples/
+README.md#writing-your-own-task) ```python from typing import Iterable, List
+from spacy.tokens import Doc from spacy_llm.registry import registry from
+spacy_llm.util import split_labels @registry.llm_tasks
+("my_namespace.MyTask.v1") def make_my_task(labels: str, my_other_config_val:
+float) -> "MyTask": labels_list = split_labels(labels) return MyTask
+(labels=labels_list, my_other_config_val=my_other_config_val) class MyTask: def
+__init__(self, labels: List[str], my_other_config_val: float): ... def
+generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]: ... def
+parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] ) -
+> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1" labels = LABEL1,LABEL2,LABEL3
 my_other_config_val = 0.3 ``` ## Logging spacy-llm has a built-in logger that
 can log the prompt sent to the LLM as well as its raw response. This logger
 uses the debug level and by default has a `logging.NullHandler()` configured.
 In order to use this logger, you can setup a simple handler like this:
 ```python import logging import spacy_llm spacy_llm.logger.addHandler
 (logging.StreamHandler()) spacy_llm.logger.setLevel(logging.DEBUG) ``` > NOTE:
@@ -132,82 +145,137 @@
 Text Classification system. Your task is to accept Text as input and provide a
 category for the text based on the predefined labels. Classify the text below
 to any of the following labels: COMPLIMENT, INSULT The task is non-exclusive,
 so you can provide more than one label as long as they're comma-delimited. For
 example: Label1, Label2, Label3. Do not put any other text in your answer, only
 one or more of the provided labels with nothing before or after. If the text
 cannot be classified into any of the provided labels, answer `==NONE==`. Here
-is the text that needs classification Text: ''' You look gorgeous! ''' Backend
+is the text that needs classification Text: ''' You look gorgeous! ''' Model
 response for doc: You look gorgeous! COMPLIMENT ``` `print(doc.cats)` to
 standard output should look like: ``` {'COMPLIMENT': 1.0, 'INSULT': 0.0} ``` ##
 ð API `spacy-llm` exposes a `llm` factory that accepts the following
 configuration options: | Argument | Type | Description | | ---------------- | -
 ------------------------------------------ | ----------------------------------
 ------------------------------------------------- | | `task` | `Optional
 [LLMTask]` | An LLMTask can generate prompts and parse LLM responses. See
-[docs](#tasks). | | `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` |
-Callable querying a specific LLM API. See [docs](#backends). | | `cache` |
+[docs](#tasks). | | `model` | `Callable[[Iterable[Any]], Iterable[Any]]]` |
+Callable querying a specific LLM API. See [docs](#models). | | `cache` |
 `Cache` | Cache to use for caching prompts and responses per doc (batch). See
 [docs](#cache). | | `save_io` | `bool` | Whether to save prompts/responses
 within `Doc.user_data["llm_io"]`. | | `validate_types` | `bool` | Whether to
-check if signatures of configured backend and task are consistent. | An `llm`
+check if signatures of configured model and task are consistent. | An `llm`
 component is defined by two main settings: - A [**task**](#tasks), defining the
 prompt to send to the LLM as well as the functionality to parse the resulting
 response back into structured fields on spaCy's [Doc](https://spacy.io/api/doc)
-objects. - A [**backend**](#backends) defining the model to use and how to
-connect to it. Note that `spacy-llm` supports both access to external APIs
-(such as OpenAI) as well as access to self-hosted open-source LLMs (such as
-using Dolly through Hugging Face). Moreover, `spacy-llm` exposes a customizable
-[**caching**](#cache) functionality to avoid running the same document through
-an LLM service (be it local or through a REST API) more than once. Finally, you
-can choose to save a stringified version of LLM prompts/responses within the
+objects. - A [**model**](#models) defining the model and how to connect to it.
+Note that `spacy-llm` supports both access to external APIs (such as OpenAI) as
+well as access to self-hosted open-source LLMs (such as using Dolly through
+Hugging Face). Moreover, `spacy-llm` exposes a customizable [**caching**]
+(#cache) functionality to avoid running the same document through an LLM
+service (be it local or through a REST API) more than once. Finally, you can
+choose to save a stringified version of LLM prompts/responses within the
 `Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
 `Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM
 component within the spaCy pipeline. Each entry is itself a dictionary, with
 two keys: `prompt` and `response`. A note on `validate_types`: by default,
-`spacy-llm` checks whether the signatures of the `backend` and `task` callables
+`spacy-llm` checks whether the signatures of the `model` and `task` callables
 are consistent with each other and emits a warning if they don't.
 `validate_types` can be set to `False` if you want to disable this behavior.
 ### Tasks A _task_ defines an NLP problem or question, that will be sent to the
 LLM via a prompt. Further, the task defines how to parse the LLM's responses
 back into structured information. All tasks are registered in spaCy's
 `llm_tasks` registry. Practically speaking, a task should adhere to the
 `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py). It needs to define
 a `generate_prompts` function and a `parse_responses` function. Moreover, the
 task may define an optional [`scorer` method](https://spacy.io/api/
 scorer#score). It should accept an iterable of `Example`s as input and return a
 score dictionary. If the `scorer` method is defined, `spacy-llm` will call it
-to evaluate the component. #### function `task.generate_prompts` Takes a
-collection of documents, and returns a collection of "prompts", which can be of
-type `Any`. Often, prompts are of type `str` - but this is not enforced to
-allow for maximum flexibility in the framework. | Argument | Type | Description
-| | ----------- | --------------- | ---------------------- | | `docs` |
-`Iterable[Doc]` | The input documents. | | **RETURNS** | `Iterable[Any]` | The
-generated prompts. | #### function `task.parse_responses` Takes a collection of
-LLM responses and the original documents, parses the responses into structured
-information, and sets the annotations on the documents. The `parse_responses`
-function is free to set the annotations in any way, including `Doc` fields like
-`ents`, `spans` or `cats`, or using custom defined fields. The `responses` are
-of type `Iterable[Any]`, though they will often be `str` objects. This depends
-on the return type of the [backend](#backends). | Argument | Type | Description
-| | ----------- | --------------- | ------------------------ | | `docs` |
-`Iterable[Doc]` | The input documents. | | `responses` | `Iterable[Any]` | The
-generated prompts. | | **RETURNS** | `Iterable[Doc]` | The annotated documents.
-| #### spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
+to evaluate the component. #### Providing examples for few-shot prompts All
+built-in tasks support few-shot prompts, i. e. including examples in a prompt.
+Examples can be supplied in two ways: (1) as a separate file containing only
+examples or (2) by initializing `llm` with a `get_examples()` callback (like
+any other spaCy pipeline component). ##### (1) Few-shot example file A file
+containing examples for few-shot prompting can be configured like this: ```ini
+[components.llm.task] @llm_tasks = "spacy.NER.v2" labels =
+PERSON,ORGANISATION,LOCATION [components.llm.task.examples] @misc =
+"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` The supplied file has to
+conform to the format expected by the required task (see the task documentation
+further down). ##### (2) Initializing the `llm` component with a `get_examples
+()` callback Alternatively, you can initialize your `nlp` pipeline by providing
+a `get_examples` callback for [`nlp.initialize`](https://spacy.io/api/
+language#initialize) and setting `n_prompt_examples` to a positive number to
+automatically fetch a few examples for few-shot learning. Set
+`n_prompt_examples` to `-1` to use all examples as part of the few-shot
+learning prompt. ```ini [initialize.components.llm] n_prompt_examples = 3 ```
+#### function `task.generate_prompts` Takes a collection of documents, and
+returns a collection of "prompts", which can be of type `Any`. Often, prompts
+are of type `str` - but this is not enforced to allow for maximum flexibility
+in the framework. | Argument | Type | Description | | ----------- | -----------
+---- | ---------------------- | | `docs` | `Iterable[Doc]` | The input
+documents. | | **RETURNS** | `Iterable[Any]` | The generated prompts. | ####
+function `task.parse_responses` Takes a collection of LLM responses and the
+original documents, parses the responses into structured information, and sets
+the annotations on the documents. The `parse_responses` function is free to set
+the annotations in any way, including `Doc` fields like `ents`, `spans` or
+`cats`, or using custom defined fields. The `responses` are of type `Iterable
+[Any]`, though they will often be `str` objects. This depends on the return
+type of the [model](#models). | Argument | Type | Description | | ----------- |
+--------------- | ------------------------ | | `docs` | `Iterable[Doc]` | The
+input documents. | | `responses` | `Iterable[Any]` | The generated prompts. | |
+**RETURNS** | `Iterable[Doc]` | The annotated documents. | ####
+spacy.Summarization.v1 The `spacy.Summarization.v1` task supports both zero-
+shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks =
+"spacy.Summarization.v1" examples = null max_n_words = null ``` | Argument |
+Type | Default | Description | |---------------|-------------------------------
+----------|--------------------------------------------------------------------
+----|--------------------------------------------------------------------------
+----------------------------------------------------------------| | `template`
+| `str` | [summarization.jinja](./spacy_llm/tasks/templates/
+summarization.jinja) | Custom prompt template to send to LLM backend. Default
+templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
+Optional function that generates examples for few-shot learning. | |
+`max_n_words` | `Optional[int]` | `None` | Maximum number of words to be used
+in summary. Note that this should not expected to work exactly. | | `field` |
+`str` | `summary` | Name of extension attribute to store summary in (i. e. the
+summary will be available in `doc._.{field}`). | The summarization task prompts
+the model for a concise summary of the provided text. It optionally allows to
+limit the response to a certain number of tokens - note that this requirement
+will be included in the prompt, but the task doesn't perform a hard cut-off.
+It's hence possible that your summary exceeds `max_n_words`. To perform few-
+shot learning, you can write down a few examples in a separate file, and
+provide these to be injected into the prompt to the LLM. The default reader
+`spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+```yaml - text: > The United Nations, referred to informally as the UN, is an
+intergovernmental organization whose stated purposes are to maintain
+international peace and security, develop friendly relations among nations,
+achieve international cooperation, and serve as a centre for harmonizing the
+actions of nations. It is the world's largest international organization. The
+UN is headquartered on international territory in New York City, and the
+organization has other offices in Geneva, Nairobi, Vienna, and The Hague, where
+the International Court of Justice is headquartered.\n\n The UN was established
+after World War II with the aim of preventing future world wars, and succeeded
+the League of Nations, which was characterized as ineffective. summary: "The UN
+is an international organization that promotes global peace, cooperation, and
+harmony. Established after WWII, its purpose is to prevent future world wars."
+``` ```ini [components.llm.task] @llm_tasks = "spacy.summarization.v1"
+max_n_words = 20 [components.llm.task.examples] @misc =
+"spacy.FewShotReader.v1" path = "summarization_examples.yml" ``` ####
+spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
 prompting. This version also supports explicitly defining the provided labels
 with custom descriptions. ```ini [components.llm.task] @llm_tasks =
 "spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"] examples = null
 ``` | Argument | Type | Default | Description | | ------------------------- | -
 -------------------------------------- | --------------------------------------
 ------------------ | ----------------------------------------------------------
 -------------------------------------------------------------------------------
 ------------ | | `labels` | `Union[List[str], str]` | | List of labels or str
 of comma-separated list of labels. | | `template` | `str` | [ner.v2.jinja](./
 spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM
-backend. Default templates for each task are located in the `spacy_llm/tasks/
+model. Default templates for each task are located in the `spacy_llm/tasks/
 templates` directory. | | `label_definitions` | `Optional[Dict[str, str]]` |
 `None` | Optional dict mapping a label to a description of that label. These
 descriptions are added to the prompt to help instruct the LLM on what to
 extract. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
 Optional function that generates examples for few-shot learning. | |
 `normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
 normalizes the labels as returned by the LLM. If `None`, defaults to
@@ -236,28 +304,27 @@
 a few examples in a separate file, and provide these to be injected into the
 prompt to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
 `.yaml`, `.json` and `.jsonl`. ```yaml - text: Jack and Jill went up the hill.
 entities: PERSON: - Jack - Jill LOCATION: - hill - text: Jack fell down and
 broke his crown. entities: PERSON: - Jack ``` ```ini [components.llm.task]
 @llm_tasks = "spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION
 [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
-"ner_examples.yml" ``` If you don't have specific examples to provide to the
-LLM, you can write definitions for each label and provide them via the
-`label_definitions` argument. This lets you tell the LLM exactly what you're
-looking for rather than relying on the LLM to interpret its task given just the
-label name. Label descriptions are freeform so you can write whatever you want
-here, but through some experiments a brief description along with some examples
-and counter examples seems to work quite well. ```ini [components.llm.task]
-@llm_tasks = "spacy.NER.v2" labels = PERSON,SPORTS_TEAM
+"ner_examples.yml" ``` You can also write definitions for each label and
+provide them via the `label_definitions` argument. This lets you tell the LLM
+exactly what you're looking for rather than relying on the LLM to interpret its
+task given just the label name. Label descriptions are freeform so you can
+write whatever you want here, but through some experiments a brief description
+along with some examples and counter examples seems to work quite well. ```ini
+[components.llm.task] @llm_tasks = "spacy.NER.v2" labels = PERSON,SPORTS_TEAM
 [components.llm.task.label_definitions] PERSON = "Extract any named individual
 in the text." SPORTS_TEAM = "Extract the names of any professional sports team.
 e.g. Golden State Warriors, LA Lakers, Man City, Real Madrid" ``` > Label
 descriptions can also be used with explicit examples to give as much info to
-the LLM backend as possible. #### spacy.NER.v1 The original version of the
-built-in NER task supports both zero-shot and few-shot prompting. ```ini
+the LLM model as possible. #### spacy.NER.v1 The original version of the built-
+in NER task supports both zero-shot and few-shot prompting. ```ini
 [components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
 PERSON,ORGANISATION,LOCATION examples = null ``` | Argument | Type | Default |
 Description | | ------------------------- | -----------------------------------
 ---- | ------------ | ---------------------------------------------------------
 -------------------------------------------------------------------------------
 ---- | | `labels` | `str` | | Comma-separated list of labels. | | `examples` |
 `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
@@ -300,15 +367,15 @@
 Description | | ------------------------- | -----------------------------------
 ---- | ------------------------------------------------------------------ | ---
 -------------------------------------------------------------------------------
 ------------------------------------------------------------------- | |
 `labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
 list of labels. | | `template` | `str` | [`spancat.v2.jinja`](./spacy_llm/
 tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM
-backend. Default templates for each task are located in the `spacy_llm/tasks/
+model. Default templates for each task are located in the `spacy_llm/tasks/
 templates` directory. | | `label_definitions` | `Optional[Dict[str, str]]` |
 `None` | Optional dict mapping a label to a description of that label. These
 descriptions are added to the prompt to help instruct the LLM on what to
 extract. | | `spans_key` | `str` | `"sc"` | Key of the `Doc.spans` dict to save
 the spans under. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` |
 `None` | Optional function that generates examples for few-shot learning. | |
 `normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
@@ -338,25 +405,30 @@
 Alignment mode in case the LLM returns entities that do not align with token
 boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
 `case_sensitive_matching` | `bool` | `False` | Whether to search without case
 sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
 in the LLM's response only once (the first hit) or multiple times. | Except for
 the `spans_key` parameter, the SpanCat task reuses the configuration from the
 NER task. Refer to [its documentation](#spacynerv1) for more insight. ####
-spacy.TextCat.v2 The built-in TextCat task supports both zero-shot and few-shot
-prompting. ```ini [components.llm.task] @llm_tasks = "spacy.TextCat.v2" labels
-= ["COMPLIMENT", "INSULT"] examples = null ``` | Argument | Type | Default |
-Description | | ------------------- | --------------------------------------- |
------------------------------------------------------------- | ----------------
--------------------------------------------------------------------------------
-------------------------------------------------- | | `labels` | `Union[List
-[str], str]` | | List of labels or str of comma-separated list of labels. | |
-`template` | `str` | [`textcat.jinja`](./spacy_llm/tasks/templates/
-textcat.jinja) | Custom prompt template to send to LLM backend. Default
-templates for each task are located in the `spacy_llm/tasks/templates`
+spacy.TextCat.v3 Version 3 (the most recent) of the built-in TextCat task
+supports both zero-shot and few-shot prompting. It allows setting definitions
+of labels. Those definitions are included in the prompt. ```ini
+[components.llm.task] @llm_tasks = "spacy.TextCat.v3" labels = ["COMPLIMENT",
+"INSULT"] label_definitions = { "COMPLIMENT": "a polite expression of praise or
+admiration.", "INSULT": "a disrespectful or scornfully abusive remark or act."
+} examples = null ``` | Argument | Type | Default | Description | | -----------
+-------- | --------------------------------------- | --------------------------
+---------------------------------- | ------------------------------------------
+-------------------------------------------------------------------------------
+----------------------- | | `labels` | `Union[List[str], str]` | | List of
+labels or str of comma-separated list of labels. | | `label_definitions` |
+`Optional[Dict[str, str]]` | `None` | Dictionary of label definitions. Included
+in the prompt, if set. | | `template` | `str` | [`textcat.jinja`](./spacy_llm/
+tasks/templates/textcat.jinja) | Custom prompt template to send to LLM backend.
+Default templates for each task are located in the `spacy_llm/tasks/templates`
 directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
 Optional function that generates examples for few-shot learning. | |
 `normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
 normalizes the labels as returned by the LLM. If `None`, falls back to
 `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` | `False` | If
 set to `True`, only one label per document should be valid. If set to `False`,
 one document can have multiple labels. | | `allow_none` | `bool` | `True` |
@@ -365,18 +437,50 @@
 `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
 when the LLM returns invalid responses. | To perform few-shot learning, you can
 write down a few examples in a separate file, and provide these to be injected
 into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
 supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
 great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
 "answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
+"spacy.TextCat.v3" labels = ["COMPLIMENT", "INSULT"] label_definitions =
+{ "COMPLIMENT": "a polite expression of praise or admiration.", "INSULT": "a
+disrespectful or scornfully abusive remark or act." }
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"textcat_examples.json" ``` #### spacy.TextCat.v2 Version 2 of the built-in
+TextCat task supports both zero-shot and few-shot prompting and includes an
+improved prompt template. ```ini [components.llm.task] @llm_tasks =
+"spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"] examples = null ``` |
+Argument | Type | Default | Description | | ------------------- | -------------
+-------------------------- | --------------------------------------------------
+---------- | ------------------------------------------------------------------
+-----------------------------------------------------------------------------
+- | | `labels` | `Union[List[str], str]` | | List of labels or str of comma-
+separated list of labels. | | `template` | `str` | [`textcat.jinja`](./
+spacy_llm/tasks/templates/textcat.jinja) | Custom prompt template to send to
+LLM model. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
+| `None` | Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, falls back to
+`spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` | `False` | If
+set to `True`, only one label per document should be valid. If set to `False`,
+one document can have multiple labels. | | `allow_none` | `bool` | `True` |
+When set to `True`, allows the LLM to not return any of the given label. The
+resulting dict in `doc.cats` will have `0.0` scores for all labels. | |
+`verbose` | `bool` | `False` | If set to `True`, warnings will be generated
+when the LLM returns invalid responses. | To perform few-shot learning, you can
+write down a few examples in a separate file, and provide these to be injected
+into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
+supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
+great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
+"answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
 "spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"]
 [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
-"textcat_examples.json" ``` #### spacy.TextCat.v1 The original version of the
-built-in TextCat task supports both zero-shot and few-shot prompting. ```ini
+"textcat_examples.json" ``` #### spacy.TextCat.v1 Version 1 of the built-in
+TextCat task supports both zero-shot and few-shot prompting. ```ini
 [components.llm.task] @llm_tasks = "spacy.TextCat.v1" labels =
 COMPLIMENT,INSULT examples = null ``` | Argument | Type | Default | Description
 | | ------------------- | --------------------------------------- | ------- | -
 -------------------------------------------------------------------------------
 ---------------------------------------------------------------- | | `labels` |
 str | | Comma-separated list of labels. | | `examples` | `Optional[Callable[[],
 Iterable[Any]]]` | `None` | Optional function that generates examples for few-
@@ -398,249 +502,505 @@
 @misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
 spacy.REL.v1 The built-in REL task supports both zero-shot and few-shot
 prompting. It relies on an upstream NER component for entities extraction.
 ```ini [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
 "Visits"] ``` | Argument | Type | Default | Description | | ------------------
 - | --------------------------------------- | ---------------------------------
 ------------------- | ---------------------------------------------------------
-------------------------------------------------------------------------------
-- | | `labels` | `Union[List[str], str]` | | List of labels or str of comma-
+----------------------------------------------------------------------------- |
+| `labels` | `Union[List[str], str]` | | List of labels or str of comma-
 separated list of labels. | | `template` | `str` | [`rel.jinja`](./spacy_llm/
-tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend.
+tasks/templates/rel.jinja) | Custom prompt template to send to LLM model.
 Default templates for each task are located in the `spacy_llm/tasks/templates`
 directory. | | `label_description` | `Optional[Dict[str, str]]` | `None` |
 Dictionary providing a description for each relation label. | | `examples` |
 `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
 generates examples for few-shot learning. | | `normalizer` | `Optional[Callable
 [[str], str]]` | `None` | Function that normalizes the labels as returned by
 the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`. | | `verbose`
 | `bool` | `False` | If set to `True`, warnings will be generated when the LLM
 returns invalid responses. | To perform few-shot learning, you can write down a
 few examples in a separate file, and provide these to be injected into the
 prompt to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
-`.yaml`, `.json` and `.jsonl`. ```json {"text": "Laura bought a house in Boston
-with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5, "label":
-"PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"}, {"start_char":
-48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep": 0, "dest": 1,
-"relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation": "LivesIn"}]} {"text":
-"Michael travelled through South America by bike.", "ents": [{"start_char": 0,
-"end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label":
-"LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]} ``` Note:
-the REL task relies on pre-extracted entities to make its prediction. Hence,
-you'll need to add a component that populates `doc.ents` with recognized spans
-to your spaCy pipeline and put it _before_ the REL component. ```ini
-[components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
-"Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
-= "rel_examples.jsonl" ``` #### spacy.Lemma.v1 The `Lemma.v1` task lemmatizes
-the provided text and updates the `lemma_` attribute in the doc's tokens
-accordingly. ```ini [components.llm.task] @llm_tasks = "spacy.Lemma.v1"
-examples = null ``` | Argument | Type | Default | Description | | ---------- |
---------------------------------------- | -------------------------------------
+`.yaml`, `.json` and `.jsonl`. ```jsonl {"text": "Laura bought a house in
+Boston with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5,
+"label": "PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"},
+{"start_char": 48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep":
+0, "dest": 1, "relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation":
+"LivesIn"}]} {"text": "Michael travelled through South America by bike.",
+"ents": [{"start_char": 0, "end_char": 7, "label": "PERSON"}, {"start_char":
+26, "end_char": 39, "label": "LOC"}], "relations": [{"dep": 0, "dest": 1,
+"relation": "Visits"}]} ``` ```ini [components.llm.task] @llm_tasks =
+"spacy.REL.v1" labels = ["LivesIn", "Visits"] [components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1" path = "rel_examples.jsonl" ``` Note: the REL
+task relies on pre-extracted entities to make its prediction. Hence, you'll
+need to add a component that populates `doc.ents` with recognized spans to your
+spaCy pipeline and put it _before_ the REL component. #### spacy.Lemma.v1 The
+`Lemma.v1` task lemmatizes the provided text and updates the `lemma_` attribute
+in the doc's tokens accordingly. ```ini [components.llm.task] @llm_tasks =
+"spacy.Lemma.v1" examples = null ``` | Argument | Type | Default | Description
+| | ---------- | --------------------------------------- | --------------------
+---------------------------------- | ------------------------------------------
+-------------------------------------------------------------------------------
+------------- | | `template` | `str` | [lemma.jinja](./spacy_llm/tasks/
+templates/lemma.jinja) | Custom prompt template to send to LLM model. Default
+templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
+Optional function that generates examples for few-shot learning. | `Lemma.v1`
+prompts the LLM to lemmatize the passed text and return the lemmatized version
+as a list of tokens and their corresponding lemma. E. g. the text `I'm buying
+ice cream for my friends` should invoke the response ``` I: I 'm: be buying:
+buy ice: ice cream: cream for: for my: my friends: friend .: . ``` If for any
+given text/doc instance the number of lemmas returned by the LLM doesn't match
+the number of tokens recognized by spaCy, no lemmas are stored in the
+corresponding doc's tokens. Otherwise the tokens `.lemma_` property is updated
+with the lemma suggested by the LLM. To perform few-shot learning, you can
+write down a few examples in a separate file, and provide these to be injected
+into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
+supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```yaml - text: I'm buying ice
+cream. lemmas: - "I": "I" - "'m": "be" - "buying": "buy" - "ice": "ice" -
+"cream": "cream" - ".": "." - text: I've watered the plants. lemmas: - "I": "I"
+- "'ve": "have" - "watered": "water" - "the": "the" - "plants": "plant" - ".":
+"." ``` ```ini [components.llm.task] @llm_tasks = "spacy.Lemma.v1"
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"lemma_examples.yml" ``` #### spacy.Sentiment.v1 Performs sentiment analysis on
+provided texts. Scores between 0 and 1 are stored in `Doc._.sentiment` - the
+higher, the more positive. Note in cases of parsing issues (e. g. in case of
+unexpected LLM responses) the value might be `None`. ```ini
+[components.llm.task] @llm_tasks = "spacy.Sentiment.v1" examples = null ``` |
+Argument | Type | Default | Description | | ---------- | ----------------------
 ----------------- | -----------------------------------------------------------
------------------------------------------------------------------------------ |
-| `template` | `str` | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) |
-Custom prompt template to send to LLM backend. Default templates for each task
-are located in the `spacy_llm/tasks/templates` directory. | | `examples` |
+--- | -------------------------------------------------------------------------
+------------------------------------------------------------- | | `template` |
+`str` | [sentiment.jinja](./spacy_llm/tasks/templates/sentiment.jinja) | Custom
+prompt template to send to LLM model. Default templates for each task are
+located in the `spacy_llm/tasks/templates` directory. | | `examples` |
 `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
-generates examples for few-shot learning. | `Lemma.v1` prompts the LLM to
-lemmatize the passed text and return the lemmatized version as a list of tokens
-and their corresponding lemma. E. g. the text `I'm buying ice cream for my
-friends` should invoke the response ``` I: I 'm: be buying: buy ice: ice cream:
-cream for: for my: my friends: friend .: . ``` If for any given text/doc
-instance the number of lemmas returned by the LLM doesn't match the number of
-tokens recognized by spaCy, no lemmas are stored in the corresponding doc's
-tokens. Otherwise the tokens `.lemma_` property is updated with the lemma
-suggested by the LLM. To perform few-shot learning, you can write down a few
-examples in a separate file, and provide these to be injected into the prompt
-to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
-`.yaml`, `.json` and `.jsonl`. ```yaml - text: I'm buying ice cream. lemmas: -
-"I": "I" - "'m": "be" - "buying": "buy" - "ice": "ice" - "cream": "cream" -
-".": "." - text: I've watered the plants. lemmas: - "I": "I" - "'ve": "have" -
-"watered": "water" - "the": "the" - "plants": "plant" - ".": "." ``` ```ini
-[components.llm.task] @llm_tasks = "spacy.Lemma.v1"
+generates examples for few-shot learning. | | `field` | `str` | `sentiment` |
+Name of extension attribute to store summary in (i. e. the summary will be
+available in `doc._.{field}`). | To perform few-shot learning, you can write
+down a few examples in a separate file, and provide these to be injected into
+the prompt to the LLM. The default reader `spacy.FewShotReader.v1` supports
+`.yml`, `.yaml`, `.json` and `.jsonl`. ```yaml - text: "This is horrifying."
+score: 0 - text: "This is underwhelming." score: 0.25 - text: "This is ok."
+score: 0.5 - text: "I'm looking forward to this!" score: 1.0 ``` ```ini
+[components.llm.task] @llm_tasks = "spacy.Sentiment.v1"
 [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
-"lemma_examples.yml" ``` #### spacy.NoOp.v1 This task is only useful for
+"sentiment_examples.yml" ``` #### spacy.NoOp.v1 This task is only useful for
 testing - it tells the LLM to do nothing, and does not set any fields on the
 `docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
-Backends A _backend_ defines which LLM model to query, and how to query it. It
-can be a simple function taking a collection of prompts (consistent with the
-output type of `task.generate_prompts()`) and returning a collection of
-responses (consistent with the expected input of `parse_responses`). Generally
-speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
-but specific implementations can have other signatures, like `Callable[
-[Iterable[str]], Iterable[str]]`. All built-in backends are registered in
-`llm_backends`. If no backend is specified, the repo currently connects to the
-[`OpenAI` API](#openai) by default, using the built-in REST protocol, and
-accesses the `"gpt-3.5-turbo"` model. > :question: _Why are there backends for
-third-party libraries in addition to a native REST backend and which should > I
-choose?_ > > Third-party libraries like `langchain` or `minichain` focus on
-prompt management, integration of many different LLM > APIs, and other related
-features such as conversational memory or agents. `spacy-llm` on the other hand
-emphasizes > features we consider useful in the context of NLP pipelines
-utilizing LLMs to process documents (mostly) independent > from each other. It
-makes sense that the feature set of such third-party libraries and `spacy-llm`
-is not identical - > and users might want to take advantage of features not
-available in `spacy-llm`. > > The advantage of offering our own REST backend is
-that we can ensure a larger degree of stability of robustness, as > we can
-guarantee backwards-compatibility and more smoothly integrated error handling.
-> > Ultimately we recommend trying to implement your use case using the REST
-backend first (which is configured as the > default backend). If however there
-are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
-> backend of a third-party library - and easy to customize the prompting
-mechanism, if so required. #### OpenAI When the backend uses OpenAI, you have
-to get an API key from openai.com, and ensure that the keys are set as
-environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
-OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
-`requests` and a simple retry mechanism to access an API. ```ini
-[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
-= {"model": "gpt-3.5-turbo", "temperature": 0.3} ``` | Argument | Type |
-Default | Description | | ----------- | ---------------- | ------- | ----------
--------------------------------------------------------------------------------
---------------------------- | | `api` | `str` | | The name of a supported API.
-In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
-| Further configuration passed on to the backend. | | `strict` | `bool` |
+Models A _model_ defines which LLM model to query, and how to query it. It can
+be a simple function taking a collection of prompts (consistent with the output
+type of `task.generate_prompts()`) and returning a collection of responses
+(consistent with the expected input of `parse_responses`). Generally speaking,
+it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`, but
+specific implementations can have other signatures, like `Callable[[Iterable
+[str]], Iterable[str]]`. All built-in models are registered in `llm_models`. If
+no model is specified, the repo currently connects to the `OpenAI` API by
+default using REST, and accesses the `"gpt-3.5-turbo"` model. Currently three
+different approaches to use LLMs are supported: 1. `spacy-llm`s native REST
+backend. This is the default for all hosted models (e. g. OpenAI, Cohere,
+Anthropic, ...). 2. A HuggingFace integration that allows to run a limited set
+of HF models locally. 3. A LangChain integration that allows to run any model
+supported by LangChain (hosted or locally). Approaches 1. and 2 are the default
+for hosted model and local models, respectively. Alternatively you can use
+LangChain to access hosted or local models by specifying one of the models
+registered with the `langchain.` prefix. > :question: Why LangChain if there
+are also are a native REST and a HuggingFace backend? When should I use what? >
+> Third-party libraries like `langchain` focus on prompt management,
+integration of many different LLM > APIs, and other related features such as
+conversational memory or agents. `spacy-llm` on the other hand emphasizes >
+features we consider useful in the context of NLP pipelines utilizing LLMs to
+process documents (mostly) independent > from each other. It makes sense that
+the feature sets of such third-party libraries and `spacy-llm` aren't identical
+- > and users might want to take advantage of features not available in `spacy-
+llm`. > > The advantage of implementing our own REST and HuggingFace
+integrations is that we can ensure a larger degree of stability and robustness,
+as > we can guarantee backwards-compatibility and more smoothly integrated
+error handling. > > If however there are features or APIs not natively covered
+by `spacy-llm`, it's trivial to utilize LangChain to cover > this - and easy to
+customize the prompting mechanism, if so required. Note that when using hosted
+services, you have to ensure that the proper API keys are set as environment
+variables as described by the corresponding provider's documentation. E. g.
+when using OpenAI, you have to get an API key from openai.com, and ensure that
+the keys are set as environmental variables: ```shell export
+OPENAI_API_KEY="sk-..." export OPENAI_API_ORG="org-..." ``` For Cohere it's
+```shell export CO_API_KEY="..." ``` and for Anthropic ```shell export
+ANTHROPIC_API_KEY="..." ``` #### spacy.GPT-4.v1 OpenAI's `gpt-4` model family.
+Example config: ```ini [components.llm.model] @llm_models = "spacy.GPT-4.v1"
+name = "gpt-4" config = {"temperature": 0.3} ``` | Argument | Type | Default |
+Description | | ----------- | -------------------------------------------------
+-------------- | --------- | --------------------------------------------------
+------------------------------------------------------------------ | | `name` |
+`Literal["gpt-4", "gpt-4-0314", "gpt-4-32k", "gpt-4-32k-0314"]` | `"gpt-4"` |
+Model name, i. e. any supported variant for this particular model. | | `config`
+| `Dict[Any, Any]` | `{}` | Further configuration passed on to the model. | |
+`strict` | `bool` | `True` | If `True`, raises an error if the LLM API returns
+a malformed response. Otherwise, return the error responses as is. | |
+`max_tries` | `int` | `3` | Max. number of tries for API request. | | `timeout`
+| `int` | `30` | Timeout for API request in seconds. | #### spacy.GPT-3-5.v1
+OpenAI's `gpt-3-5` model family. Example config: ```ini [components.llm.model]
+@llm_models = "spacy.GPT-3-5.v1" name = "gpt-3.5-turbo" config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | --------
+--- | -------------------------------------------------------------------------
+---------------------- | ----------------- | ----------------------------------
+-------------------------------------------------------------------------------
+--- | | `name` | `Literal["gpt-3.5-turbo", "gpt-3.5-turbo-16k", "gpt-3.5-turbo-
+0613", "gpt-3.5-turbo-0613-16k"]` | `"gpt-3.5-turbo"` | Model name, i. e. any
+supported variant for this particular model. | | `config` | `Dict[Any, Any]` |
+`{}` | Further configuration passed on to the model. | | `strict` | `bool` |
 `True` | If `True`, raises an error if the LLM API returns a malformed
 response. Otherwise, return the error responses as is. | | `max_tries` | `int`
 | `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
-Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
-following settings can be defined in the `config` dictionary: - `model`: one of
-the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
-`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
-babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
-`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
-For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
-completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
-srush/MiniChain) for the API retrieval part, make sure you have installed it
-first: ```shell python -m pip install "minichain>=0.3,<0.4" # Or install with
-spacy-llm directly python -m pip install "spacy-llm[minichain]" ``` Note that
-MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
-blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
-api = "OpenAI" [components.llm.backend.query] @llm_queries =
-"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
+Timeout for API request in seconds. | #### spacy.Text-Davinci.v1 OpenAI's
+`text-davinci` model family. Example config: ```ini [components.llm.model]
+@llm_models = "spacy.Text-Davinci.v1" name = "text-davinci-003" config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | --------
+--- | ------------------------------------------------- | -------------------
+- | ---------------------------------------------------------------------------
+----------------------------------------- | | `name` | `Literal["text-davinci-
+002", "text-davinci-003"]` | `"text-davinci-003"` | Model name, i. e. any
+supported variant for this particular model. | | `config` | `Dict[Any, Any]` |
+`{}` | Further configuration passed on to the model. | | `strict` | `bool` |
+`True` | If `True`, raises an error if the LLM API returns a malformed
+response. Otherwise, return the error responses as is. | | `max_tries` | `int`
+| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
+Timeout for API request in seconds. | #### spacy.Code-Davinci.v1 OpenAI's
+`code-davinci` model family. Example config: ```ini [components.llm.model]
+@llm_models = "spacy.Code-Davinci.v1" name = "code-davinci-002" config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | --------
+--- | ----------------------------- | -------------------- | ------------------
+-------------------------------------------------------------------------------
+------------------- | | `name` | `Literal["code-davinci-002"]` | `"code-
+davinci-002"` | Model name, i. e. any supported variant for this particular
+model. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration passed on
+to the model. | | `strict` | `bool` | `True` | If `True`, raises an error if
+the LLM API returns a malformed response. Otherwise, return the error responses
+as is. | | `max_tries` | `int` | `3` | Max. number of tries for API request. |
+| `timeout` | `int` | `30` | Timeout for API request in seconds. | ####
+spacy.Text-Curie.v1 OpenAI's `text-curie` model family. Example config: ```ini
+[components.llm.model] @llm_models = "spacy.Text-Curie.v1" name = "text-curie-
+001" config = {"temperature": 0.3} ``` | Argument | Type | Default |
+Description | | ----------- | --------------------------- | -----------------
+- | ---------------------------------------------------------------------------
+----------------------------------------- | | `name` | `Literal["text-curie-
+001"]` | `"text-curie-001"` | Model name, i. e. any supported variant for this
+particular model. | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the model. | | `strict` | `bool` | `True` | If
+`True`, raises an error if the LLM API returns a malformed response. Otherwise,
+return the error responses as is. | | `max_tries` | `int` | `3` | Max. number
+of tries for API request. | | `timeout` | `int` | `30` | Timeout for API
+request in seconds. | #### spacy.Text-Babbage.v1 OpenAI's `text-babbage` model
+family. Example config: ```ini [components.llm.model] @llm_models =
+"spacy.Text-Babbage.v1" name = "text-babbage-001" config = {"temperature": 0.3}
+``` | Argument | Type | Default | Description | | ----------- | ---------------
+-------------- | -------------------- | ---------------------------------------
+----------------------------------------------------------------------------- |
+| `name` | `Literal["text-babbage-001"]` | `"text-babbage-001"` | Model name,
+i. e. any supported variant for this particular model. | | `config` | `Dict
+[Any, Any]` | `{}` | Further configuration passed on to the model. | | `strict`
+| `bool` | `True` | If `True`, raises an error if the LLM API returns a
+malformed response. Otherwise, return the error responses as is. | |
+`max_tries` | `int` | `3` | Max. number of tries for API request. | | `timeout`
+| `int` | `30` | Timeout for API request in seconds. | #### spacy.Text-Ada.v1
+OpenAI's `text-ada` model family. Example config: ```ini [components.llm.model]
+@llm_models = "spacy.Text-Ada.v1" name = "text-ada-001" config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | --------
+--- | ------------------------- | ---------------- | --------------------------
+-------------------------------------------------------------------------------
+----------- | | `name` | `Literal["text-ada-001"]` | `"text-ada-001"` | Model
+name, i. e. any supported variant for this particular model. | | `config` |
+`Dict[Any, Any]` | `{}` | Further configuration passed on to the model. | |
+`strict` | `bool` | `True` | If `True`, raises an error if the LLM API returns
+a malformed response. Otherwise, return the error responses as is. | |
+`max_tries` | `int` | `3` | Max. number of tries for API request. | | `timeout`
+| `int` | `30` | Timeout for API request in seconds. | #### spacy.Davinci.v1
+OpenAI's `davinci` model family. Example config: ```ini [components.llm.model]
+@llm_models = "spacy.Davinci.v1 " name = "davinci" config = {"temperature":
+0.3} ``` | Argument | Type | Default | Description | | ----------- | ----------
+---------- | ----------- | ----------------------------------------------------
+---------------------------------------------------------------- | | `name` |
+`Literal["davinci"]` | `"davinci"` | Model name, i. e. any supported variant
+for this particular model. | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the model. | | `strict` | `bool` | `True` | If
+`True`, raises an error if the LLM API returns a malformed response. Otherwise,
+return the error responses as is. | | `max_tries` | `int` | `3` | Max. number
+of tries for API request. | | `timeout` | `int` | `30` | Timeout for API
+request in seconds. | #### spacy.Curie.v1 OpenAI's `curie` model family.
+Example config: ```ini [components.llm.model] @llm_models = "spacy.Curie.v1 "
+name = "curie" config = {"temperature": 0.3} ``` | Argument | Type | Default |
+Description | | ----------- | ------------------ | --------- | ----------------
+-------------------------------------------------------------------------------
+--------------------- | | `name` | `Literal["curie"]` | `"curie"` | Model name,
+i. e. any supported variant for this particular model. | | `config` | `Dict
+[Any, Any]` | `{}` | Further configuration passed on to the model. | | `strict`
+| `bool` | `True` | If `True`, raises an error if the LLM API returns a
+malformed response. Otherwise, return the error responses as is. | |
+`max_tries` | `int` | `3` | Max. number of tries for API request. | | `timeout`
+| `int` | `30` | Timeout for API request in seconds. | #### spacy.Babbage.v1
+OpenAI's `babbage` model family. Example config: ```ini [components.llm.model]
+@llm_models = "spacy.Babbage.v1 " name = "babbage" config = {"temperature":
+0.3} ``` | Argument | Type | Default | Description | | ----------- | ----------
+---------- | ----------- | ----------------------------------------------------
+---------------------------------------------------------------- | | `name` |
+`Literal["babbage"]` | `"babbage"` | Model name, i. e. any supported variant
+for this particular model. | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the model. | | `strict` | `bool` | `True` | If
+`True`, raises an error if the LLM API returns a malformed response. Otherwise,
+return the error responses as is. | | `max_tries` | `int` | `3` | Max. number
+of tries for API request. | | `timeout` | `int` | `30` | Timeout for API
+request in seconds. | #### spacy.Ada.v1 OpenAI's `ada` model family. Example
+config: ```ini [components.llm.model] @llm_models = "spacy.Ada.v1 " name =
+"ada" config = {"temperature": 0.3} ``` | Argument | Type | Default |
+Description | | ----------- | ---------------- | ------- | --------------------
+-------------------------------------------------------------------------------
+----------------- | | `name` | `Literal["ada"]` | `"ada"` | Model name, i. e.
+any supported variant for this particular model. | | `config` | `Dict[Any,
+Any]` | `{}` | Further configuration passed on to the model. | | `strict` |
+`bool` | `True` | If `True`, raises an error if the LLM API returns a malformed
+response. Otherwise, return the error responses as is. | | `max_tries` | `int`
+| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
+Timeout for API request in seconds. | #### spacy.Command.v1 Cohere's `command`
+model family. Example config: ```ini [components.llm.model] @llm_models =
+"spacy.Command.v1 " name = "command" config = {"temperature": 0.3} ``` |
+Argument | Type | Default | Description | | ----------- | ---------------------
+------------------------------------------------------------ | ----------- | --
+-------------------------------------------------------------------------------
+----------------------------------- | | `name` | `Literal["command", "command-
+light", "command-light-nightly", "command-nightly"]` | `"command"` | Model
+name, i. e. any supported variant for this particular model. | | `config` |
+`Dict[Any, Any]` | `{}` | Further configuration passed on to the model. | |
+`strict` | `bool` | `True` | If `True`, raises an error if the LLM API returns
+a malformed response. Otherwise, return the error responses as is. | |
+`max_tries` | `int` | `3` | Max. number of tries for API request. | | `timeout`
+| `int` | `30` | Timeout for API request in seconds. | #### spacy.Claude-1.v1
+Anthropic's `claude-1` model family. Example config: ```ini
+[components.llm.model] @llm_models = "spacy.Claude-1.v1 " name = "claude-1"
+config = {"temperature": 0.3} ``` | Argument | Type | Default | Description | |
+----------- | -------------------------------------- | ------------ | ---------
+-------------------------------------------------------------------------------
+---------------------------- | | `name` | `Literal["claude-1", "claude-1-
+100k"]` | `"claude-1"` | Model name, i. e. any supported variant for this
+particular model. | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the model. | | `strict` | `bool` | `True` | If
+`True`, raises an error if the LLM API returns a malformed response. Otherwise,
+return the error responses as is. | | `max_tries` | `int` | `3` | Max. number
+of tries for API request. | | `timeout` | `int` | `30` | Timeout for API
+request in seconds. | #### spacy.Claude-instant-1.v1 Anthropic's `claude-
+instant-1` model family. Example config: ```ini [components.llm.model]
+@llm_models = "spacy.Claude-instant-1.v1 " name = "claude-instant-1" config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | --------
+--- | ------------------------------------------------------ | ----------------
+---- | ------------------------------------------------------------------------
+-------------------------------------------- | | `name` | `Literal["claude-
+instant-1", "claude-instant-1-100k"]` | `"claude-instant-1"` | Model name, i.
+e. any supported variant for this particular model. | | `config` | `Dict[Any,
+Any]` | `{}` | Further configuration passed on to the model. | | `strict` |
+`bool` | `True` | If `True`, raises an error if the LLM API returns a malformed
+response. Otherwise, return the error responses as is. | | `max_tries` | `int`
+| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
+Timeout for API request in seconds. | #### spacy.Claude-instant-1-1.v1
+Anthropic's `claude-instant-1.1` model family. Example config: ```ini
+[components.llm.model] @llm_models = "spacy.Claude-instant-1-1.v1 " name =
+"claude-instant-1.1" config = {"temperature": 0.3} ``` | Argument | Type |
+Default | Description | | ----------- | ---------------------------------------
+------------------- | ---------------------- | --------------------------------
+-------------------------------------------------------------------------------
+----- | | `name` | `Literal["claude-instant-1.1", "claude-instant-1.1-100k"]` |
+`"claude-instant-1.1"` | Model name, i. e. any supported variant for this
+particular model. | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the model. | | `strict` | `bool` | `True` | If
+`True`, raises an error if the LLM API returns a malformed response. Otherwise,
+return the error responses as is. | | `max_tries` | `int` | `3` | Max. number
+of tries for API request. | | `timeout` | `int` | `30` | Timeout for API
+request in seconds. | #### spacy.Claude-1-0.v1 Anthropic's `claude-1.0` model
+family. Example config: ```ini [components.llm.model] @llm_models =
+"spacy.Claude-1-0.v1 " name = "claude-1.0" config = {"temperature": 0.3} ``` |
+Argument | Type | Default | Description | | ----------- | ---------------------
+-- | -------------- | ---------------------------------------------------------
+----------------------------------------------------------- | | `name` |
+`Literal["claude-1.0"]` | `"claude-1.0"` | Model name, i. e. any supported
+variant for this particular model. | | `config` | `Dict[Any, Any]` | `{}` |
+Further configuration passed on to the model. | | `strict` | `bool` | `True` |
+If `True`, raises an error if the LLM API returns a malformed response.
+Otherwise, return the error responses as is. | | `max_tries` | `int` | `3` |
+Max. number of tries for API request. | | `timeout` | `int` | `30` | Timeout
+for API request in seconds. | #### spacy.Claude-1-2.v1 Anthropic's `claude-1.2`
+model family. Example config: ```ini [components.llm.model] @llm_models =
+"spacy.Claude-1-2.v1 " name = "claude-1.2" config = {"temperature": 0.3} ``` |
+Argument | Type | Default | Description | | ----------- | ---------------------
+-- | -------------- | ---------------------------------------------------------
+----------------------------------------------------------- | | `name` |
+`Literal["claude-1.2"]` | `"claude-1.2"` | Model name, i. e. any supported
+variant for this particular model. | | `config` | `Dict[Any, Any]` | `{}` |
+Further configuration passed on to the model. | | `strict` | `bool` | `True` |
+If `True`, raises an error if the LLM API returns a malformed response.
+Otherwise, return the error responses as is. | | `max_tries` | `int` | `3` |
+Max. number of tries for API request. | | `timeout` | `int` | `30` | Timeout
+for API request in seconds. | #### spacy.Claude-1-3.v1 Anthropic's `claude-1.3`
+model family. Example config: ```ini [components.llm.model] @llm_models =
+"spacy.Claude-1-3.v1 " name = "claude-1.3" config = {"temperature": 0.3} ``` |
+Argument | Type | Default | Description | | ----------- | ---------------------
+--------------------- | -------------- | --------------------------------------
+-----------------------------------------------------------------------------
+- | | `name` | `Literal["claude-1.3", "claude-1.3-100k"]` | `"claude-1.3"` |
+Model name, i. e. any supported variant for this particular model. | | `config`
+| `Dict[Any, Any]` | `{}` | Further configuration passed on to the model. | |
+`strict` | `bool` | `True` | If `True`, raises an error if the LLM API returns
+a malformed response. Otherwise, return the error responses as is. | |
+`max_tries` | `int` | `3` | Max. number of tries for API request. | | `timeout`
+| `int` | `30` | Timeout for API request in seconds. | #### spacy.Dolly.v1 To
+use this model, ideally you have a GPU enabled and have installed
+`transformers`, `torch` and CUDA in your virtual environment. This allows you
+to have the setting `device=cuda:0` in your config, which ensures that the
+model is loaded entirely on the GPU (and fails otherwise). You can do so with
+```shell python -m pip install "spacy-llm[transformers]" "transformers
+[sentencepiece]" ``` If you don't have access to a GPU, you can install
+`accelerate` and set`device_map=auto` instead, but be aware that this may
+result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries. ```shell python -m pip
+install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.model] @llm_models = "spacy.Dolly.v1" name = "dolly-v2-3b" ```
+| Argument | Type | Default | Description | | ------------- | -----------------
+-------------------------------------- | ------- | ----------------------------
+-------------------------------------------------------------------- | | `name`
+| `Literal["dolly-v2-3b", "dolly-v2-7b", "dolly-v2-12b"]` | | The name of a
+Dolly model that is supported (e. g. "dolly-v2-3b" or "dolly-v2-12b"). | |
+`config_init` | `Dict[str, Any]` | `{}` | Further configuration passed on to
+the construction of the model with `transformers.pipeline()`. | | `config_run`
+| `Dict[str, Any]` | `{}` | Further configuration used during model inference.
+| Supported models (see the [Databricks models page](https://huggingface.co/
+databricks) on Hugging Face for details): - `"databricks/dolly-v2-3b"` -
+`"databricks/dolly-v2-7b"` - `"databricks/dolly-v2-12b"` Note that Hugging Face
+will download this model the first time you use it - you can [define the cached
+directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-
+cache) by setting the environmental variable `HF_HOME`. #### spacy.Falcon.v1 To
+use this backend, ideally you have a GPU enabled and have installed
+`transformers`, `torch` and CUDA in your virtual environment. This allows you
+to have the setting `device=cuda:0` in your config, which ensures that the
+model is loaded entirely on the GPU (and fails otherwise). You can do so with
+```shell python -m pip install "spacy-llm[transformers]" "transformers
+[sentencepiece]" ``` If you don't have access to a GPU, you can install
+`accelerate` and set`device_map=auto` instead, but be aware that this may
+result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries. ```shell python -m pip
+install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.model] @llm_models = "spacy.Falcon.v1" name = "falcon-7b" ``` |
+Argument | Type | Default | Description | | ------------- | -------------------
+---------------------------------------------------------------- | ------------
 --- | -------------------------------------------------------------------------
--------- | ------- | ----------------------------------------------------------
-------------------------- | | `api` | `str` | | The name of an API supported by
-MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
-configuration passed on to the backend. | | `query` | `Optional[Callable[
-["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
-Function that executes the prompts. If `None`, defaults to
-`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
-executes the prompts by running `model(text).run()` for each given textual
-prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
-hwchase17/langchain) for the API retrieval part, make sure you have installed
-it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" # Or install
-with spacy-llm directly python -m pip install "spacy-llm[langchain]" ``` Note
-that LangChain currently only supports Python 3.9 and beyond. Example config
-block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
-= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
+----------------------- | | `name` | `Literal["falcon-rw-1b", "falcon-7b",
+"falcon-7b-instruct", "falcon-40b-instruct"]` | `"7b-instruct"` | The name of a
+Falcon model variant that is supported. | | `config_init` | `Dict[str, Any]` |
+`{}` | Further configuration passed on to the construction of the model with
+`transformers.pipeline()`. | | `config_run` | `Dict[str, Any]` | `{}` | Further
+configuration used during model inference. | Note that Hugging Face will
+download this model the first time you use it - you can [define the cache
+directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-
+cache) by setting the environmental variable `HF_HOME`. #### spacy.StableLM.v1
+To use this model, ideally you have a GPU enabled and have installed
+`transformers`, `torch` and CUDA in your virtual environment. You can do so
+with ```shell python -m pip install "spacy-llm[transformers]" "transformers
+[sentencepiece]" ``` If you don't have access to a GPU, you can install
+`accelerate` and set`device_map=auto` instead, but be aware that this may
+result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries. ```shell python -m pip
+install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.model] @llm_models = "spacy.StableLM.v1" name = "stablelm-
+tuned-alpha-7b" ``` | Argument | Type | Default | Description | | ------------
+- | ---------------------------------------------------------------------------
+---------------------------------------- | ------- | --------------------------
+-------------------------------------------------------------------------------
+------------------- | | `name` | `Literal["stablelm-base-alpha-3b", "stablelm-
+base-alpha-7b", "stablelm-tuned-alpha-3b", "stablelm-tuned-alpha-7b"]` | | The
+name of a StableLM model that is supported (e. g. "stablelm-tuned-alpha-7b"). |
+| `config_init` | `Dict[str, Any]` | `{}` | Further configuration passed on to
+the construction of the model with
+`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
+[str, Any]` | `{}` | Further configuration used during model inference. | See
+the [Stability AI StableLM GitHub repo](https://github.com/Stability-AI/
+StableLM/#stablelm-alpha) for details. Note that Hugging Face will download
+this model the first time you use it - you can [define the cached directory]
+(https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by
+setting the environmental variable `HF_HOME`. #### spacy.OpenLLaMA.v1 To use
+this model, ideally you have a GPU enabled and have installed - `transformers
+[sentencepiece]` - `torch` - CUDA in your virtual environment. You can do so
+with ```shell python -m pip install "spacy-llm[transformers]" "transformers
+[sentencepiece]" ``` If you don't have access to a GPU, you can install
+`accelerate` and set`device_map=auto` instead, but be aware that this may
+result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries. ```shell python -m pip
+install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.model] @llm_models = "spacy.OpenLLaMA.v1" name =
+"open_llama_3b_350bt_preview" ``` | Argument | Type | Default | Description | |
+------------- | ---------------------------------------------------------------
+---------------------------------------------------------------------- | ------
+- | ---------------------------------------------------------------------------
+------------------------------------------------- | | `name` | `Literal
+["open_llama_3b_350bt_preview", "open_llama_3b_600bt_preview",
+"open_llama_7b_400bt_preview", "open_llama_7b_600bt_preview"]` | | The name of
+a OpenLLaMA model that is supported (e. g. "open_llama_3b_350bt_preview"). | |
+`config_init` | `Dict[str, Any]` | `{}` | Further configuration passed on to
+the construction of the model with
+`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
+[str, Any]` | `{}` | Further configuration used during model inference. | See
+the [OpenLM Research OpenLLaMA GitHub repo](https://github.com/openlm-research/
+open_llama) for details. Note that Hugging Face will download this model the
+first time you use it - you can [define the cached directory](https://
+huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
+environmental variable `HF_HOME`. #### LangChain models To use [LangChain]
+(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
+you have installed it first: ```shell python -m pip install
+"langchain==0.0.191" # Or install with spacy-llm directly python -m pip install
+"spacy-llm[extras]" ``` Note that LangChain currently only supports Python 3.9
+and beyond. LangChain models in `spacy-llm` work slightly differently.
+`langchain`'s models are parsed automatically, each LLM class in `langchain`
+has one entry in `spacy-llm`'s registry. As `langchain`'s design has one class
+per API and not per model, this results in registry entries like
+`langchain.OpenAI.v1` - i. e. there is one registry entry per API and not per
+model (family), as for the REST- and HuggingFace-based entries. The name of the
+model to be used has to be passed in via the `name` attribute. Example config
+block: ```ini [components.llm.model] @llm_models = "langchain.OpenAI.v1" name =
+"gpt-3.5-turbo" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
 {"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
 - | ---------------------------------------------------------------------------
 --- | ------- | ---------------------------------------------------------------
---------------------- | | `api` | `str` | | The name of an API supported by
-LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
-configuration passed on to the backend. | | `query` | `Optional[Callable[
+--------------------- | | `name` | `str` | | The name of a mdodel supported by
+LangChain for this API. | | `config` | `Dict[Any, Any]` | `{}` | Configuration
+passed on to the LangChain model. | | `query` | `Optional[Callable[
 ["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
 that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
 The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
-`model(text)` for each given textual prompt. #### spacy.Dolly_HF.v1 To use this
-backend, ideally you have a GPU enabled and have installed `transformers`,
-`torch` and CUDA in your virtual environment. This allows you to have the
-setting `device=cuda:0` in your config, which ensures that the model is loaded
-entirely on the GPU (and fails otherwise). You can do so with ```shell python -
-m pip install "spacy-llm[transformers]" "transformers[sentencepiece]" ``` If
-you don't have access to a GPU, you can install `accelerate` and
-set`device_map=auto` instead, but be aware that this may result in some layers
-getting distributed to the CPU or even the hard drive, which may ultimately
-result in extremely slow queries. ```shell python -m pip install
-"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
-[components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1" model =
-"databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
---------- | ---------------- | ------- | --------------------------------------
----------------------------------------------------------- | | `model` | `str`
-| | The name of a Dolly model that is supported. | | `config_init` | `Dict[str,
-Any]` | `{}` | Further configuration passed on to the construction of the model
-with `transformers.pipeline()`. | | `config_run` | `Dict[str, Any]` | `{}` |
-Further configuration used during model inference. | Supported models (see the
-[Databricks models page](https://huggingface.co/databricks) on Hugging Face for
-details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-v2-7b"` -
-`"databricks/dolly-v2-12b"` Note that Hugging Face will download this model the
-first time you use it - you can [define the cached directory](https://
-huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
-environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
-backend, ideally you have a GPU enabled and have installed `transformers`,
-`torch` and CUDA in your virtual environment. You can do so with ```shell
-python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
-``` If you don't have access to a GPU, you can install `accelerate` and
-set`device_map=auto` instead, but be aware that this may result in some layers
-getting distributed to the CPU or even the hard drive, which may ultimately
-result in extremely slow queries. ```shell python -m pip install
-"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
-[components.llm.backend] @llm_backends = "spacy.StableLM_HF.v1" model =
-"stabilityai/stablelm-tuned-alpha-7b" ``` | Argument | Type | Default |
-Description | | ------------- | ---------------- | ------- | ------------------
--------------------------------------------------------------------------------
---------------------------- | | `model` | `str` | | The name of a StableLM
-model that is supported. | | `config_init` | `Dict[str, Any]` | `{}` | Further
-configuration passed on to the construction of the model with
-`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
-[str, Any]` | `{}` | Further configuration used during model inference. |
-Supported models (see the [Stability AI StableLM GitHub repo](https://
-github.com/Stability-AI/StableLM/#stablelm-alpha) for details): -
-`"stabilityai/stablelm-base-alpha-3b"` - `"stabilityai/stablelm-base-alpha-7b"`
-- `"stabilityai/stablelm-tuned-alpha-3b"` - `"stabilityai/stablelm-tuned-alpha-
-7b"` Note that Hugging Face will download this model the first time you use it
-- you can [define the cached directory](https://huggingface.co/docs/
-huggingface_hub/main/en/guides/manage-cache) by setting the environmental
-variable `HF_HOME`. #### spacy.OpenLLaMaHF.v1 To use this backend, ideally you
-have a GPU enabled and have installed - `transformers[sentencepiece]` - `torch`
-- CUDA in your virtual environment. You can do so with ```shell python -m pip
-install "spacy-llm[transformers]" "transformers[sentencepiece]" ``` If you
-don't have access to a GPU, you can install `accelerate` and
-set`device_map=auto` instead, but be aware that this may result in some layers
-getting distributed to the CPU or even the hard drive, which may ultimately
-result in extremely slow queries. ```shell python -m pip install
-"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
-[components.llm.backend] @llm_backends = "spacy.OpenLLaMaHF.v1" model =
-"openlm-research/open_llama_3b_350bt_preview" ``` | Argument | Type | Default |
-Description | | ------------- | ---------------- | ------- | ------------------
--------------------------------------------------------------------------------
---------------------------- | | `model` | `str` | | The name of a OpenLLaMa
-model that is supported. | | `config_init` | `Dict[str, Any]` | `{}` | Further
-configuration passed on to the construction of the model with
-`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
-[str, Any]` | `{}` | Further configuration used during model inference. |
-Supported models (see the [OpenLM Research OpenLLaMa GitHub repo](https://
-github.com/openlm-research/open_llama) for details): - `"openlm-research/
-open_llama_3b_350bt_preview"` - `"openlm-research/open_llama_3b_600bt_preview"`
-- `"openlm-research/open_llama_7b_400bt_preview"` - `"openlm-research/
-open_llama_7b_700bt_preview"` Note that Hugging Face will download this model
-the first time you use it - you can [define the cached directory](https://
-huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
-environmental variable `HF_HOME`. ### Cache Interacting with LLMs, either
-through an external API or a local instance, is costly. Since developing an NLP
-pipeline generally means a lot of exploration and prototyping, `spacy-llm`
-implements a built-in cache to avoid reprocessing the same documents at each
-run that keeps batches of documents stored on disk. Example config block:
-```ini [components.llm.cache] @llm_misc = "spacy.BatchCache.v1" path = "path/
-to/cache" batch_size = 64 max_batches_in_mem = 4 ``` | Argument | Type |
-Default | Description | | -------------------- | ---------------------------- |
-------- | ---------------------------------------------------------------------
----------------------------------------------------- | | `path` | `Optional
-[Union[str, Path]]` | `None` | Cache directory. If `None`, no caching is
-performed, and this component will act as a NoOp. | | `batch_size` | `int` | 64
-| Number of docs in one batch (file). Once a batch is full, it will be peristed
-to disk. | | `max_batches_in_mem` | `int` | 4 | Max. number of batches to hold
-in memory. Allows you to limit the effect on your memory if you're handling a
-lot of docs. | When retrieving a document, the `BatchCache` will first figure
-out what batch the document belongs to. If the batch isn't in memory it will
-try to load the batch from disk and then move it into memory. Note that since
-the cache is generated by a registered function, you can also provide your own
-registered function returning your own cache implementation. If you wish to do
-so, ensure that your cache object adheres to the `Protocol` defined in
+`model(text)` for each given textual prompt. ### Cache Interacting with LLMs,
+either through an external API or a local instance, is costly. Since developing
+an NLP pipeline generally means a lot of exploration and prototyping, `spacy-
+llm` implements a built-in cache to avoid reprocessing the same documents at
+each run that keeps batches of documents stored on disk. The cache
+implementation also ensures that documents in one cache directory were all
+produced using the same prompt template. This is only possible however if the
+specified task implements ```python @property def prompt_template() -> str: ...
+``` which returns the raw prompt template as string. If `prompt_template()`
+isn't implemented, the cache will emit a warning and not check for prompt
+template consistency. Example config block: ```ini [components.llm.cache]
+@llm_misc = "spacy.BatchCache.v1" path = "path/to/cache" batch_size = 64
+max_batches_in_mem = 4 ``` | Argument | Type | Default | Description | | ------
+-------------- | ---------------------------- | ------- | ---------------------
+-------------------------------------------------------------------------------
+--------------------- | | `path` | `Optional[Union[str, Path]]` | `None` |
+Cache directory. If `None`, no caching is performed, and this component will
+act as a NoOp. | | `batch_size` | `int` | 64 | Number of docs in one batch
+(file). Once a batch is full, it will be persisted to disk. | |
+`max_batches_in_mem` | `int` | 4 | Max. number of batches to hold in memory.
+Allows you to limit the effect on your memory if you're handling a lot of docs.
+| When retrieving a document, the `BatchCache` will first figure out what batch
+the document belongs to. If the batch isn't in memory it will try to load the
+batch from disk and then move it into memory. Note that since the cache is
+generated by a registered function, you can also provide your own registered
+function returning your own cache implementation. If you wish to do so, ensure
+that your cache object adheres to the `Protocol` defined in
 `spacy_llm.ty.Cache`. ### Various functions #### spacy.FewShotReader.v1 This
 function is registered in spaCy's `misc` registry, and reads in examples from a
 `.yml`, `.yaml`, `.json` or `.jsonl` file. It uses [`srsly`](https://
 github.com/explosion/srsly) to read in these files and parses them depending on
 the file extension. ```ini [components.llm.task.examples] @misc =
 "spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument | Type |
 Description | | -------- | ------------------ | -------------------------------
@@ -663,8 +1023,9 @@
 will - Add more example tasks - Support a broader range of models - Provide
 more example use-cases and tutorials - Make the built-in tasks easier to
 customize via Jinja templates to define the instructions & examples PRs are
 always welcome! ## ðï¸ Reporting issues If you have questions regarding the
 usage of `spacy-llm`, or want to give us feedback after giving it a spin,
 please use the [discussion board](https://github.com/explosion/spaCy/
 discussions). Bug reports can be filed on the [spaCy issue tracker](https://
-github.com/explosion/spaCy/issues). Thank you!
+github.com/explosion/spaCy/issues). Thank you! ## Migration guides Please refer
+to our [migration guide](migration_guide.md).
```

### Comparing `spacy-llm-0.3.2/pyproject.toml` & `spacy-llm-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 filterwarnings = [
     "error",
     "ignore:^.*pkg_resources.*:DeprecationWarning",
     "ignore:.*function is now available as sqlalchemy.orm.declarative_base().*:",
     "ignore:^.*You are trying to use a chat model. This way of initializing it is no longer supported. Instead, please use.*:UserWarning",
+    "ignore:^.*Xformers is not installed correctly.*:",
+    "ignore:^.*The 'warn' method is deprecated, use 'warning' instead.*:DeprecationWarning"
 ]
 markers = [
     "external: interacts with a (potentially cost-incurring) third-party API"
 ]
 
 [tool.isort]
 multi_line_output = 9
```

### Comparing `spacy-llm-0.3.2/setup.cfg` & `spacy-llm-0.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.3.2
+version = 0.4.0
 description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -39,21 +39,21 @@
 spacy_factories = 
 	llm = spacy_llm.pipeline.llm:make_llm
 spacy_misc = 
 	spacy.FewShotReader.v1 = spacy_llm.registry:fewshot_reader
 	spacy.FileReader.v1 = spacy_llm.registry:file_reader
 
 [options.extras_require]
-minichain = 
-	minichain>=0.3,<0.4
 langchain = 
 	langchain==0.0.191
 transformers = 
 	torch>=1.13.1,<2.0
 	transformers>=4.28.1,<5.0
+	einops>=0.4
+	xformers
 
 [bdist_wheel]
 universal = true
 
 [sdist]
 formats = gztar
```

### Comparing `spacy-llm-0.3.2/spacy_llm/backends/integration/hf/base.py` & `spacy-llm-0.4.0/spacy_llm/models/hf/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 import abc
 import warnings
-from typing import Any, Dict, Iterable, Optional, Tuple, TypeVar
+from typing import Any, Dict, Iterable, Optional, Tuple
 
 from thinc.compat import has_torch_cuda_gpu
 
-from ....compat import has_accelerate, has_torch, has_transformers, torch
+from ...compat import Literal, has_accelerate, has_torch, has_transformers, torch
 
-# Type of prompts returned from Task.generate_prompts().
-_PromptType = TypeVar("_PromptType")
-# Type of responses returned from query function.
-_ResponseType = TypeVar("_ResponseType")
 
+class HuggingFace(abc.ABC):
+    """Base class for HuggingFace model classes."""
 
-class HuggingFaceBackend(abc.ABC):
-    """Backend for HuggingFace models."""
+    MODEL_NAMES = Literal[None]  # noqa: F722
 
     def __init__(
         self,
-        model: str,
+        name: str,
         config_init: Optional[Dict[str, Any]],
         config_run: Optional[Dict[str, Any]],
     ):
-        """Initializes Backend instance.
-        query (Callable[[Any, Iterable[_PromptType]], Iterable[_ResponseType]]): Callable executing LLM prompts when
+        """Initializes HF model instance.
+        query (Callable[[Any, Iterable[Any]], Iterable[Any]): Callable executing LLM prompts when
             supplied with the `integration` object.
-        model (str): Name of HF model to load.
+        name (str): Name of HF model to load (without account name).
         config_init (Optional[Dict[str, Any]]): HF config for initializing the model.
         config_run (Optional[Dict[str, Any]]): HF config for running the model.
         inference_config (Dict[Any, Any]): HF config for model run.
         """
-        self._model_name = model
+        self._name = name if self.hf_account in name else f"{self.hf_account}/{name}"
         self._config_init, self._config_run = self.compile_default_configs()
         if config_init:
             self._config_init = {**self._config_init, **config_init}
         if config_run:
             self._config_run = {**self._config_run, **config_run}
 
         # Init HF model.
-        HuggingFaceBackend.check_installation()
-        self.check_model()
+        HuggingFace.check_installation()
+        self._check_model()
         self._model = self.init_model()
 
     @abc.abstractmethod
-    def __call__(self, prompts: Iterable[_PromptType]) -> Iterable[_ResponseType]:
+    def __call__(self, prompts: Iterable[Any]) -> Iterable[Any]:
         """Executes prompts on specified API.
-        prompts (Iterable[_PromptType]): Prompts to execute.
-        RETURNS (Iterable[_ResponseType]): API responses.
+        prompts (Iterable[Any]): Prompts to execute.
+        RETURNS (Iterable[Any]): API responses.
         """
 
+    def _check_model(self) -> None:
+        """Checks whether model is supported. Raises if it isn't."""
+        if self._name.replace(f"{self.hf_account}/", "") not in self.get_model_names():
+            raise ValueError(
+                f"Model '{self._name}' is not supported - select one of {self.get_model_names()} instead"
+            )
+
+    @classmethod
+    def get_model_names(cls) -> Tuple[str, ...]:
+        """Names of supported models for this HF model implementation.
+        RETURNS (Tuple[str]): Names of supported models.
+        """
+        return tuple(str(arg) for arg in cls.MODEL_NAMES.__args__)  # type: ignore[attr-defined]
+
     @property
     @abc.abstractmethod
-    def supported_models(self) -> Iterable[str]:
-        """Get names of supported models.
-        RETURNS (Iterable[str]): Names of supported models.
+    def hf_account(self) -> str:
+        """Name of HF account for this model.
+        RETURNS (str): Name of HF account.
         """
 
     @staticmethod
     def check_installation() -> None:
         """Checks whether the required external libraries are installed. Raises an error otherwise."""
         if not has_torch:
             raise ValueError(
-                "The HF backend requires `torch` to be installed, which it is not. See "
+                "The HF model requires `torch` to be installed, which it is not. See "
                 "https://pytorch.org/ for installation instructions."
             )
         if not has_transformers:
             raise ValueError(
-                "The HF backend requires `transformers` to be installed, which it is not. See "
+                "The HF model requires `transformers` to be installed, which it is not. See "
                 "https://huggingface.co/docs/transformers/installation for installation instructions."
             )
 
-    def check_model(self) -> None:
-        """Checks whether model is supported. Raises if it isn't."""
-        if self._model_name not in self.supported_models:
-            raise ValueError(
-                f"Model '{self._model_name}' is not supported - select one of {self.supported_models} instead"
-            )
-
     @staticmethod
     def compile_default_configs() -> Tuple[Dict[str, Any], Dict[str, Any]]:
         """Compiles default init and run configs for HF model.
         RETURNS (Tuple[Dict[str, Any], Dict[str, Any]]): HF model default init config, HF model default run config.
         """
         default_cfg_init: Dict[str, Any] = {}
         default_cfg_run: Dict[str, Any] = {}
```

### Comparing `spacy-llm-0.3.2/spacy_llm/backends/integration/hf/dolly.py` & `spacy-llm-0.4.0/spacy_llm/models/hf/falcon.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 from typing import Any, Callable, Dict, Iterable, Optional, Tuple
 
-from spacy.util import SimpleFrozenDict, SimpleFrozenList
+from spacy.util import SimpleFrozenDict
 
-from ....compat import transformers
-from ....registry.util import registry
-from . import HuggingFaceBackend
+from ...compat import Literal, transformers
+from ...registry.util import registry
+from .base import HuggingFace
+
+
+class Falcon(HuggingFace):
+    MODEL_NAMES = Literal[
+        "falcon-rw-1b", "falcon-7b", "falcon-7b-instruct", "falcon-40b-instruct"
+    ]  # noqa: F722
+
+    def __init__(
+        self,
+        name: MODEL_NAMES,
+        config_init: Optional[Dict[str, Any]],
+        config_run: Optional[Dict[str, Any]],
+    ):
+        self._tokenizer: Optional["transformers.AutoTokenizer"] = None
+        self._device: Optional[str] = None
+        super().__init__(name=name, config_init=config_init, config_run=config_run)
+        assert isinstance(self._tokenizer, transformers.PreTrainedTokenizerBase)
+        self._config_run["eos_token_id"] = self._tokenizer.eos_token_id
 
-
-class DollyBackend(HuggingFaceBackend):
     def init_model(self) -> Any:
-        """Sets up HF model and needed utilities.
-        RETURNS (Any): HF model.
-        """
-        return transformers.pipeline(model=self._model_name, **self._config_init)
+        self._tokenizer = transformers.AutoTokenizer.from_pretrained(self._name)
+        return transformers.pipeline(
+            "text-generation",
+            model=self._name,
+            tokenizer=self._tokenizer,
+            **self._config_init,
+        )
 
     @property
-    def supported_models(self) -> Iterable[str]:
-        return SimpleFrozenList(
-            [
-                "databricks/dolly-v2-3b",
-                "databricks/dolly-v2-7b",
-                "databricks/dolly-v2-12b",
-            ]
-        )
+    def hf_account(self) -> str:
+        return "tiiuae"
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:  # type: ignore[override]
-        """Queries Dolly HF model.
-        pipeline (transformers.pipeline): Transformers pipeline to query.
-        prompts (Iterable[str]): Prompts to query Dolly model with.
-        RETURNS (Iterable[str]): Prompt responses.
-        """
         return [
             self._model(pr, **self._config_run)[0]["generated_text"] for pr in prompts
         ]
 
     @staticmethod
     def compile_default_configs() -> Tuple[Dict[str, Any], Dict[str, Any]]:
-        default_cfg_init, default_cfg_run = HuggingFaceBackend.compile_default_configs()
+        default_cfg_init, default_cfg_run = HuggingFace.compile_default_configs()
         return (
             {
                 **default_cfg_init,
-                # Loads a custom pipeline from
-                # https://huggingface.co/databricks/dolly-v2-3b/blob/main/instruct_pipeline.py
-                # cf also https://huggingface.co/databricks/dolly-v2-12b
                 "trust_remote_code": True,
             },
-            default_cfg_run,
+            {
+                **default_cfg_run,
+                "max_length": 200,
+                "do_sample": True,
+                "top_k": 10,
+                "num_return_sequences": 1,
+            },
         )
 
 
-@registry.llm_backends("spacy.DollyHF.v1")
-@registry.llm_backends("spacy.Dolly_HF.v1")
-def backend_dolly_hf(
-    model: str,
+@registry.llm_models("spacy.Falcon.v1")
+def falcon_hf(
+    name: Falcon.MODEL_NAMES,
     config_init: Optional[Dict[str, Any]] = SimpleFrozenDict(),
     config_run: Optional[Dict[str, Any]] = SimpleFrozenDict(),
 ) -> Callable[[Iterable[str]], Iterable[str]]:
-    """Returns Callable that can execute a set of prompts and return the raw responses.
-    model (str): Name of the HF model.
+    """Generates Falcon instance that can execute a set of prompts and return the raw responses.
+    name (Literal): Name of the Falcon model. Has to be one of Falcon.get_model_names().
     config_init (Optional[Dict[str, Any]]): HF config for initializing the model.
     config_run (Optional[Dict[str, Any]]): HF config for running the model.
-    RETURNS (Callable[[Iterable[str]], Iterable[str]]): Callable executing the prompts and returning raw responses.
+    RETURNS (Callable[[Iterable[str]], Iterable[str]]): Falcon instance that can execute a set of prompts and return
+        the raw responses.
     """
-    return DollyBackend(
-        model=model,
-        config_init=config_init,
-        config_run=config_run,
-    )
+    return Falcon(name=name, config_init=config_init, config_run=config_run)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/backends/integration/hf/openllama.py` & `spacy-llm-0.4.0/spacy_llm/models/hf/openllama.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from typing import Any, Callable, Dict, Iterable, Optional, Tuple
 
-from spacy.util import SimpleFrozenDict, SimpleFrozenList
+from spacy.util import SimpleFrozenDict
 
-from ....compat import torch, transformers
-from ....registry.util import registry
-from .base import HuggingFaceBackend
+from ...compat import Literal, torch, transformers
+from ...registry.util import registry
+from .base import HuggingFace
 
 
-class OpenLLaMaBackend(HuggingFaceBackend):
+class OpenLLaMA(HuggingFace):
+    MODEL_NAMES = Literal[
+        "open_llama_3b_350bt_preview",  # noqa: F722
+        "open_llama_3b_600bt_preview",  # noqa: F722
+        "open_llama_7b_400bt_preview",  # noqa: F722
+        "open_llama_7b_600bt_preview",  # noqa: F722
+    ]
+
     def __init__(
         self,
-        model: str,
+        name: str,
         config_init: Optional[Dict[str, Any]],
         config_run: Optional[Dict[str, Any]],
     ):
         self._tokenizer: Optional["transformers.AutoTokenizer"] = None
         self._device: Optional[str] = None
-        super().__init__(model=model, config_init=config_init, config_run=config_run)
+        super().__init__(name=name, config_init=config_init, config_run=config_run)
 
     def init_model(self) -> "transformers.AutoModelForCausalLM":
         """Sets up HF model and needed utilities.
         RETURNS (Any): HF model.
         """
         # Initialize tokenizer and model.
-        self._tokenizer = transformers.AutoTokenizer.from_pretrained(self._model_name)
+        self._tokenizer = transformers.AutoTokenizer.from_pretrained(self._name)
         init_cfg = self._config_init
         if "device" in init_cfg:
             self._device = init_cfg.pop("device")
         model = transformers.AutoModelForCausalLM.from_pretrained(
-            self._model_name, **init_cfg
+            self._name, **init_cfg
         )
 
         if self._device:
             model.to(self._device)
 
         return model
 
@@ -49,46 +56,36 @@
             self._tokenizer.decode(
                 self._model.generate(input_ids=tii, **self._config_run)[0],
             )
             for tii in tokenized_input_ids
         ]
 
     @property
-    def supported_models(self) -> Iterable[str]:
-        return SimpleFrozenList(
-            [
-                "openlm-research/open_llama_3b_350bt_preview",
-                "openlm-research/open_llama_3b_600bt_preview",
-                "openlm-research/open_llama_7b_400bt_preview",
-                "openlm-research/open_llama_7b_700bt_preview",
-            ]
-        )
+    def hf_account(self) -> str:
+        return "openlm-research"
 
     @staticmethod
     def compile_default_configs() -> Tuple[Dict[str, Any], Dict[str, Any]]:
-        default_cfg_init, default_cfg_run = HuggingFaceBackend.compile_default_configs()
+        default_cfg_init, default_cfg_run = HuggingFace.compile_default_configs()
         return (
             {
                 **default_cfg_init,
                 "torch_dtype": torch.float16,
             },
             {**default_cfg_run, "max_new_tokens": 32},
         )
 
 
-@registry.llm_backends("spacy.OpenLLaMa_HF.v1")
-def backend_openllama_hf(
-    model: str,
+@registry.llm_models("spacy.OpenLLaMA.v1")
+def openllama_hf(
+    name: OpenLLaMA.MODEL_NAMES,
     config_init: Optional[Dict[str, Any]] = SimpleFrozenDict(),
     config_run: Optional[Dict[str, Any]] = SimpleFrozenDict(),
 ) -> Callable[[Iterable[str]], Iterable[str]]:
-    """Returns Callable that can execute a set of prompts and return the raw responses.
-    model (str): Name of the HF model.
+    """Generates OpenLLaMA instance that can execute a set of prompts and return the raw responses.
+    name (Literal): Name of the OpenLLaMA model. Has to be one of OpenLLaMA.get_model_names().
     config_init (Optional[Dict[str, Any]]): HF config for initializing the model.
     config_run (Optional[Dict[str, Any]]): HF config for running the model.
-    RETURNS (Callable[[Iterable[str]], Iterable[str]]): Callable executing the prompts and returning raw responses.
+    RETURNS (Callable[[Iterable[str]], Iterable[str]]): OpenLLaMA instance that can execute a set of prompts and return
+        the raw responses.
     """
-    return OpenLLaMaBackend(
-        model=model,
-        config_init=config_init,
-        config_run=config_run,
-    )
+    return OpenLLaMA(name=name, config_init=config_init, config_run=config_run)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/backends/integration/hf/stablelm.py` & `spacy-llm-0.4.0/spacy_llm/models/hf/stablelm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,85 @@
 from typing import Any, Callable, Dict, Iterable, Optional, Tuple
 
-from spacy.util import SimpleFrozenDict, SimpleFrozenList
+from spacy.util import SimpleFrozenDict
 
-from ....compat import has_transformers, torch, transformers
-from ....registry.util import registry
-from .base import HuggingFaceBackend
+from ...compat import Literal, has_transformers, torch, transformers
+from ...registry.util import registry
+from .base import HuggingFace
 
 if has_transformers:
 
     class _StopOnTokens(transformers.StoppingCriteria):
         def __call__(
             self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs
         ) -> bool:
             stop_ids = [50278, 50279, 50277, 1, 0]
             for stop_id in stop_ids:
                 if input_ids[0][-1] == stop_id:
                     return True
             return False
 
 
-class StableLMBackend(HuggingFaceBackend):
+class StableLM(HuggingFace):
+    MODEL_NAMES = Literal[
+        "stablelm-base-alpha-3b",  # noqa: F722
+        "stablelm-base-alpha-7b",  # noqa: F722
+        "stablelm-tuned-alpha-3b",  # noqa: F722
+        "stablelm-tuned-alpha-7b",  # noqa: F722
+    ]
     _SYSTEM_PROMPT = """
 <|SYSTEM|># StableLM Tuned (Alpha version)
 - StableLM is a helpful and harmless open-source AI language model developed by StabilityAI.
 - StableLM is excited to be able to help the user, but will refuse to do anything that could be considered harmful to the user.
 - StableLM is more than just an information source, StableLM is also able to write poetry, short stories, and make jokes.
 - StableLM will refuse to participate in anything that could harm a human.
 """
 
     def __init__(
         self,
-        model: str,
+        name: str,
         config_init: Optional[Dict[str, Any]],
         config_run: Optional[Dict[str, Any]],
     ):
         self._tokenizer: Optional["transformers.AutoTokenizer"] = None
-        self._is_tuned = "tuned" in model
+        self._is_tuned = "tuned" in name
         self._device: Optional[str] = None
-        super().__init__(model=model, config_init=config_init, config_run=config_run)
+        super().__init__(name=name, config_init=config_init, config_run=config_run)
 
     def init_model(self) -> "transformers.AutoModelForCausalLM":
         """Sets up HF model and needed utilities.
         RETURNS (Any): HF model.
         """
-        # Initialize tokenizer and model.
-        self._tokenizer = transformers.AutoTokenizer.from_pretrained(self._model_name)
+        self._tokenizer = transformers.AutoTokenizer.from_pretrained(self._name)
         init_cfg = self._config_init
         if "device" in init_cfg:
             self._device = init_cfg.pop("device")
         model = transformers.AutoModelForCausalLM.from_pretrained(
-            self._model_name, **init_cfg
+            self._name, **init_cfg
         )
 
         if self._device:
             model.half().to(self._device)
 
         return model
 
+    @property
+    def hf_account(self) -> str:
+        return "stabilityai"
+
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:  # type: ignore[override]
         assert callable(self._tokenizer)
         tokenized_prompts = [
             self._tokenizer(prompt, return_tensors="pt")
             for prompt in (
                 # Add prompt formatting for tuned model.
                 prompts
                 if not self._is_tuned
                 else [
-                    f"{StableLMBackend._SYSTEM_PROMPT}<|USER|>{prompt}<|ASSISTANT|>"
+                    f"{StableLM._SYSTEM_PROMPT}<|USER|>{prompt}<|ASSISTANT|>"
                     for prompt in prompts
                 ]
             )
         ]
         if self._device:
             tokenized_prompts = [tp.to(self._device) for tp in tokenized_prompts]
 
@@ -79,49 +88,43 @@
             self._tokenizer.decode(
                 self._model.generate(**prompt, **self._config_run)[0],
                 skip_special_tokens=True,
             )
             for prompt in tokenized_prompts
         ]
 
-    @property
-    def supported_models(self) -> Iterable[str]:
-        return SimpleFrozenList(
-            [
-                "stabilityai/stablelm-base-alpha-3b",
-                "stabilityai/stablelm-base-alpha-7b",
-                "stabilityai/stablelm-tuned-alpha-3b",
-                "stabilityai/stablelm-tuned-alpha-7b",
-            ]
-        )
-
     @staticmethod
     def compile_default_configs() -> Tuple[Dict[str, Any], Dict[str, Any]]:
-        default_cfg_init, default_cfg_run = HuggingFaceBackend.compile_default_configs()
+        default_cfg_init, default_cfg_run = HuggingFace.compile_default_configs()
         return (
             default_cfg_init,
             {
                 **default_cfg_run,
                 "max_new_tokens": 64,
                 "temperature": 0.7,
                 "do_sample": True,
             },
         )
 
 
-@registry.llm_backends("spacy.StableLM_HF.v1")
-def backend_stablelm_hf(
-    model: str,
+@registry.llm_models("spacy.StableLM.v1")
+def stablelm_hf(
+    name: StableLM.MODEL_NAMES,
     config_init: Optional[Dict[str, Any]] = SimpleFrozenDict(),
     config_run: Optional[Dict[str, Any]] = SimpleFrozenDict(),
 ) -> Callable[[Iterable[str]], Iterable[str]]:
-    """Returns Callable that can execute a set of prompts and return the raw responses.
-    model (str): Name of the HF model.
+    """Generates StableLM instance that can execute a set of prompts and return the raw responses.
+    name (Literal): Name of the StableLM model. Has to be one of StableLM.get_model_names().
     config_init (Optional[Dict[str, Any]]): HF config for initializing the model.
     config_run (Optional[Dict[str, Any]]): HF config for running the model.
-    RETURNS (Callable[[Iterable[str]], Iterable[str]]): Callable executing the prompts and returning raw responses.
+    RETURNS (Callable[[Iterable[str]], Iterable[str]]): StableLM instance that can execute a set of prompts and return
+        the raw responses.
     """
-    return StableLMBackend(
-        model=model,
+    if name not in StableLM.get_model_names():
+        raise ValueError(
+            f"Expected one of {StableLM.get_model_names()}, but received {name}."
+        )
+    return StableLM(
+        name=name,
         config_init=config_init,
         config_run=config_run,
     )
```

### Comparing `spacy-llm-0.3.2/spacy_llm/backends/integration/remote/langchain.py` & `spacy-llm-0.4.0/spacy_llm/models/langchain/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,121 @@
 from typing import Any, Callable, Dict, Iterable, Optional, Type
 
 from spacy.util import SimpleFrozenDict
 
-from ....compat import has_langchain, langchain
-from ....registry import registry
-from . import RemoteBackend
+from ...compat import has_langchain, langchain
+from ...registry import registry
 
 
-def _check_installation() -> None:
-    """Checks whether `langchain` is installed. Raises an error otherwise."""
-    if not has_langchain:
-        raise ValueError(
-            "The LangChain backend requires `langchain` to be installed, which it is not. See "
-            "https://github.com/hwchase17/langchain for installation instructions."
+class LangChain:
+    def __init__(
+        self,
+        name: str,
+        api: str,
+        config: Dict[Any, Any],
+        query: Callable[
+            ["langchain.llms.base.BaseLLM", Iterable[Any]],
+            Iterable[Any],
+        ],
+    ):
+        """Initializes model instance for integration APIs.
+        name (str): Name of LangChain model to instantiate.
+        api (str): Name of class/API.
+        config (Dict[Any, Any]): Config passed on to LangChain model.
+        query (Callable[[Any, Iterable[_PromptType]], Iterable[_ResponseType]]): Callable executing LLM prompts when
+            supplied with the `integration` object.
+        """
+        self._langchain_model = LangChain.get_type_to_cls_dict()[api](
+            model_name=name, **config
         )
+        self.query = query
+        self._check_installation()
+
+    @staticmethod
+    def get_type_to_cls_dict() -> Dict[str, Type["langchain.llms.base.BaseLLM"]]:
+        """Returns langchain.llms.type_to_cls_dict.
+        RETURNS (Dict[str, Type[langchain.llms.base.BaseLLM]]): langchain.llms.type_to_cls_dict.
+        """
+        return langchain.llms.type_to_cls_dict
+
+    def __call__(self, prompts: Iterable[Any]) -> Iterable[Any]:
+        """Executes prompts on specified API.
+        prompts (Iterable[Any]): Prompts to execute.
+        RETURNS (Iterable[Any]): API responses.
+        """
+        return self.query(self._langchain_model, prompts)
+
+    @staticmethod
+    def query_langchain(
+        model: "langchain.llms.base.BaseLLM", prompts: Iterable[Any]
+    ) -> Iterable[Any]:
+        """Query LangChain model naively.
+        model (langchain.llms.base.BaseLLM): LangChain model.
+        prompts (Iterable[Any]): Prompts to execute.
+        RETURNS (Iterable[Any]): LLM responses.
+        """
+        return [model(pr) for pr in prompts]
+
+    @staticmethod
+    def _check_installation() -> None:
+        """Checks whether `langchain` is installed. Raises an error otherwise."""
+        if not has_langchain:
+            raise ValueError(
+                "The LangChain model requires `langchain` to be installed, which it is not. See "
+                "https://github.com/hwchase17/langchain for installation instructions."
+            )
+
+    @staticmethod
+    def _langchain_model_maker(class_id: str):
+        def langchain_model(
+            name: str,
+            query: Optional[
+                Callable[["langchain.llms.base.BaseLLM", Iterable[str]], Iterable[str]]
+            ] = None,
+            config: Dict[Any, Any] = SimpleFrozenDict(),
+            langchain_class_id: str = class_id,
+        ) -> Optional[Callable[[Iterable[Any]], Iterable[Any]]]:
+            try:
+                return LangChain(
+                    name=name,
+                    api=langchain_class_id,
+                    config=config,
+                    query=query_langchain() if query is None else query,
+                )
+            except ImportError as err:
+                raise ValueError(
+                    f"Failed to instantiate LangChain model {langchain_class_id}. Ensure all necessary dependencies "
+                    f"are installed."
+                ) from err
+
+        return langchain_model
+
+    @staticmethod
+    def register_models() -> None:
+        """Registers APIs supported by langchain (one API is registered as one model).
+        Doesn't attempt to register anything if LangChain isn't installed or at least one LangChain model has been
+        registered already.
+        """
+        if not has_langchain or any(
+            [
+                (handle.startswith("langchain"))
+                for handle in registry.llm_models.get_all()
+            ]
+        ):
+            return
+
+        for class_id, cls in LangChain.get_type_to_cls_dict().items():
+            registry.llm_models.register(
+                f"langchain.{cls.__name__}.v1",
+                func=LangChain._langchain_model_maker(class_id=class_id),
+            )
 
 
 @registry.llm_queries("spacy.CallLangChain.v1")
 def query_langchain() -> (
     Callable[["langchain.llms.base.BaseLLM", Iterable[Any]], Iterable[Any]]
 ):
     """Returns query Callable for LangChain.
     RETURNS (Callable[["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]:): Callable executing simple prompts on
-        the specified LangChain backend.
-    """
-    return _prompt_langchain
-
-
-def _prompt_langchain(
-    backend: "langchain.llms.base.BaseLLM", prompts: Iterable[Any]
-) -> Iterable[Any]:
-    return [backend(pr) for pr in prompts]
-
-
-@registry.llm_backends("spacy.LangChain.v1")
-def backend_langchain(
-    api: str,
-    query: Optional[
-        Callable[["langchain.llms.base.BaseLLM", Iterable[str]], Iterable[str]]
-    ] = None,
-    config: Dict[Any, Any] = SimpleFrozenDict(),
-) -> Callable[[Iterable[Any]], Iterable[Any]]:
-    """Returns Callable using MiniChain backend to prompt specified API.
-    api (str): Name of any API/class in langchain.llms.type_to_cls_dict, e. g. "openai".
-    query (Callable[["langchain.llms.BaseLLM", Iterable[str]], Iterable[str]]): Callable implementing querying this
-        API.
-    config (Dict[Any, Any]): LLM config arguments passed on to the initialization of the langchain.llms.BaseLLM
-        instance.
-    RETURNS (Callable[[Iterable[str]], Iterable[str]]]): Callable using the querying the specified API using the
-        specified backend.
+        the specified LangChain model.
     """
-    _check_installation()
-
-    if "model" not in config:
-        raise ValueError("The LLM model must be specified in the config.")
-
-    # langchain.llms.type_to_cls_dict contains all API names in lowercase, so this allows to be more forgiving and make
-    # "OpenAI" work as well "openai".
-    api = api.lower()
-    type_to_cls_dict: Dict[
-        str, Type[langchain.llms.base.BaseLLM]
-    ] = langchain.llms.type_to_cls_dict
-
-    if api in type_to_cls_dict:
-        model = config.pop("model")
-        return RemoteBackend(
-            integration=type_to_cls_dict[api](model_name=model, **config),
-            query=query_langchain() if query is None else query,
-        )
-    else:
-        raise KeyError(
-            f"The requested API {api} is not available in `langchain.llms.type_to_cls_dict`."
-        )
+    return LangChain.query_langchain
```

### Comparing `spacy-llm-0.3.2/spacy_llm/backends/rest/base.py` & `spacy-llm-0.4.0/spacy_llm/models/rest/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,91 @@
 import abc
 import time
-import warnings
 from enum import Enum
-from typing import Any, Dict, Iterable, Callable, Optional
+from typing import Any, Callable, Dict, Iterable, Optional, Tuple
 
 import requests  # type: ignore
 from requests import ConnectTimeout, ReadTimeout
 
 
 class _HTTPRetryErrorCodes(Enum):
     TOO_MANY_REQUESTS = 429
     SERVICE_UNAVAILABLE = 503
 
     @classmethod
     def has(cls, item: int):
         return item in set(item.value for item in cls)
 
 
-class Backend(abc.ABC):
+class REST(abc.ABC):
     """Queries LLMs via their REST APIs."""
 
+    DEFAULT_STRICT = True
+    DEFAULT_MAX_TRIES = 5
+    DEFAULT_INTERVAL = 1.0
+    DEFAULT_MAX_REQUEST_TIME = 30
+
     def __init__(
         self,
+        name: str,
+        endpoint: str,
         config: Dict[Any, Any],
         strict: bool,
         max_tries: int,
         interval: float,
         max_request_time: float,
     ):
-        """Initializes new Backend instance.
+        """Initializes new instance of REST-based model.
+        name (str): Model name.
+        endpoint (str): URL of API endpoint.
         config (Dict[Any, Any]): Config passed on to LLM API.
         strict (bool): If True, ValueError is raised if the LLM API returns a malformed response (i. e. any kind of JSON
             or other response object that does not conform to the expectation of how a well-formed response object from
             this API should look like). If False, the API error responses are returned by __call__(), but no error will
             be raised.
             Note that only response object structure will be checked, not the prompt response text per se.
         max_tries (int): Max. number of tries for API request.
         interval (float): Time interval (in seconds) for API retries in seconds. We implement a base 2 exponential
             backoff at each retry.
         max_request_time (float): Max. time (in seconds) to wait for request to terminate before raising an exception.
         """
+        self._name = name
+        self._endpoint = endpoint
         self._config = config
         self._strict = strict
         self._max_tries = max_tries
         self._interval = interval
         self._max_request_time = max_request_time
-        self._url = self._config.pop("url") if "url" in self._config else None
         self._credentials = self.credentials
 
-        if "model" not in config:
-            raise ValueError("The LLM model must be specified in the config.")
-        self._check_api_endpoint_compatibility()
-
         assert self._max_tries >= 1
         assert self._interval > 0
         assert self._max_request_time > 0
 
+        self._check_model()
+
+    def _check_model(self) -> None:
+        """Checks whether model is supported. Raises if it isn't."""
+        if self._name not in self.get_model_names():
+            raise ValueError(
+                f"Model '{self._name}' is not supported - select one of {self.get_model_names()} instead"
+            )
+
     @abc.abstractmethod
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         """Executes prompts on specified API.
         prompts (Iterable[str]): Prompts to execute.
         RETURNS (Iterable[str]): API responses.
         """
 
-    @property
+    @classmethod
     @abc.abstractmethod
-    def supported_models(self) -> Dict[str, str]:
-        """Returns supported models with their endpoints.
-        RETURNS (Dict[str, str]): Supported models with their endpoints.
+    def get_model_names(cls) -> Tuple[str, ...]:
+        """Names of supported models.
+        RETURNS (Tuple[str]): Names of supported models.
         """
 
     @property
     @abc.abstractmethod
     def credentials(self) -> Dict[str, str]:
         """Get credentials for the LLM API.
         RETURNS (Dict[str, str]): Credentials.
@@ -123,27 +137,12 @@
             # Increase timeout everytime you retry
             interval = interval * 2
 
         assert isinstance(response, requests.Response)
         if _HTTPRetryErrorCodes.has(response.status_code):
             raise ConnectionError(
                 f"API could not be reached after {(time.time() - start_time):.3f} seconds in total and attempting to "
-                f"connect {self._max_tries} times. Check your network connection and the API's availability."
+                f"connect {self._max_tries} times. Check your network connection and the API's availability.\n"
+                f"{response.status_code}\t{response.reason}"
             )
 
         return response
-
-    def _check_api_endpoint_compatibility(self):
-        """Checks whether specified model supports the supported API endpoint."""
-        supported_models = self.supported_models
-        if self._config["model"] not in supported_models:
-            raise ValueError(
-                f"Requested model '{self._config['model']}' is not one of the supported models: "
-                f"{', '.join(sorted(list(supported_models.keys())))}."
-            )
-
-        model_endpoint = supported_models[self._config["model"]]
-        if self._url and self._url != model_endpoint:
-            warnings.warn(
-                f"Configured endpoint {self._url} diverges from expected endpoint {model_endpoint} for selected "
-                f"model '{self._config['model']}'. Please ensure that this endpoint supports your model."
-            )
```

### Comparing `spacy-llm-0.3.2/spacy_llm/backends/rest/cohere.py` & `spacy-llm-0.4.0/spacy_llm/models/rest/cohere/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,50 @@
 import os
 from enum import Enum
-from typing import Any, Dict, Iterable, List, Sized
+from typing import Any, Dict, Iterable, List, Sized, Tuple
 
 import requests  # type: ignore[import]
 import srsly  # type: ignore[import]
 from requests import HTTPError
 
-from .base import Backend
+from ..base import REST
 
 
 class Endpoints(str, Enum):
     COMPLETION = "https://api.cohere.ai/v1/generate"
 
 
-class CohereBackend(Backend):
-    @property
-    def supported_models(self) -> Dict[str, str]:
-        """Returns supported models with their endpoints.
-        RETURNS (Dict[str, str]): Supported models with their endpoints.
-        """
-        return {
-            "command": Endpoints.COMPLETION.value,
-            "command-nightly": Endpoints.COMPLETION.value,
-            "command-light": Endpoints.COMPLETION.value,
-            "command-light-nightly": Endpoints.COMPLETION.value,
-        }
-
+class Cohere(REST):
     @property
     def credentials(self) -> Dict[str, str]:
         api_key = os.getenv("CO_API_KEY")
         if api_key is None:
             raise ValueError(
                 "Could not find the API key to access the Cohere API. Ensure you have an API key "
                 "set up via https://dashboard.cohere.ai/api-keys, then make it available as "
                 "an environment variable 'CO_API_KEY'."
             )
-
-        model = self._config["model"]
-        if model not in self.supported_models:
-            raise ValueError(
-                f"The specified model '{model}' is not supported by the /v1/generate endpoint. "
-                f"Choices are: {sorted(list(self.supported_models))}. "
-                "(See Cohere API documentation: https://docs.cohere.com/reference/generate)"
-            )
-
         headers = {"Authorization": f"Bearer {api_key}"}
         assert api_key is not None
         return headers
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         headers = {
             **self._credentials,
             "Content-Type": "application/json",
             "Accept": "application/json",
         }
 
         api_responses: List[str] = []
         prompts = list(prompts)
-        url = self._url if self._url else self.supported_models[self._config["model"]]
 
         def _request(json_data: Dict[str, Any]) -> Dict[str, Any]:
             r = self.retry(
                 call_method=requests.post,
-                url=url,
+                url=self._endpoint,
                 headers=headers,
                 json={**json_data, **self._config},
                 timeout=self._max_request_time,
             )
             try:
                 r.raise_for_status()
             except HTTPError as ex:
@@ -100,7 +78,11 @@
                     # In this case, we will just return the very first output.
                     api_responses.append(result["text"])
                     break
                 else:
                     api_responses.append(srsly.json_dumps(response))
 
         return api_responses
+
+    @classmethod
+    def get_model_names(cls) -> Tuple[str, ...]:
+        return "command", "command-light", "command-light-nightly", "command-nightly"
```

### Comparing `spacy-llm-0.3.2/spacy_llm/backends/rest/noop.py` & `spacy-llm-0.4.0/spacy_llm/models/rest/noop/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 import time
-from typing import Dict, Iterable
+from typing import Dict, Iterable, Tuple
 
-from .base import Backend
+from ..base import REST
 
 _NOOP_RESPONSE = ""
 
 
-class NoOpBackend(Backend):
-    """NoOp backend. Used for tests."""
+class NoOpModel(REST):
+    """NoOp model. Used for tests only."""
 
     _CALL_TIMEOUT = 0.01
 
-    @property
-    def supported_models(self) -> Dict[str, str]:
-        return {"NoOp": ""}
+    def __init__(self):
+        super().__init__(
+            name="NoOp",
+            endpoint="NoOp",
+            config={},
+            strict=True,
+            max_tries=1,
+            interval=1,
+            max_request_time=1,
+        )
 
     @property
     def credentials(self) -> Dict[str, str]:
         return {}
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         # Assume time penalty for API calls.
-        time.sleep(NoOpBackend._CALL_TIMEOUT)
+        time.sleep(NoOpModel._CALL_TIMEOUT)
         return [_NOOP_RESPONSE] * len(list(prompts))
+
+    @classmethod
+    def get_model_names(cls) -> Tuple[str, ...]:
+        return ("NoOp",)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/backends/rest/openai.py` & `spacy-llm-0.4.0/spacy_llm/models/rest/openai/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,26 @@
 import os
 from enum import Enum
-from typing import Any, Dict, Iterable, List, Sized
+from typing import Any, Dict, Iterable, List, Sized, Tuple
 
 import requests  # type: ignore[import]
 import srsly  # type: ignore[import]
 from requests import HTTPError
 
-from .base import Backend
+from ..base import REST
 
 
 class Endpoints(str, Enum):
     CHAT = "https://api.openai.com/v1/chat/completions"
     NON_CHAT = "https://api.openai.com/v1/completions"
 
 
-class OpenAIBackend(Backend):
-    @property
-    def supported_models(self) -> Dict[str, str]:
-        """Returns supported models with their endpoints.
-        RETURNS (Dict[str, str]): Supported models with their endpoints.
-        """
-        return {
-            "gpt-4": Endpoints.CHAT.value,
-            "gpt-4-0314": Endpoints.CHAT.value,
-            "gpt-4-32k": Endpoints.CHAT.value,
-            "gpt-4-32k-0314": Endpoints.CHAT.value,
-            "gpt-3.5-turbo": Endpoints.CHAT.value,
-            "gpt-3.5-turbo-0301": Endpoints.CHAT.value,
-            "text-davinci-003": Endpoints.NON_CHAT.value,
-            "text-davinci-002": Endpoints.NON_CHAT.value,
-            "text-curie-001": Endpoints.NON_CHAT.value,
-            "text-babbage-001": Endpoints.NON_CHAT.value,
-            "text-ada-001": Endpoints.NON_CHAT.value,
-            "davinci": Endpoints.NON_CHAT.value,
-            "curie": Endpoints.NON_CHAT.value,
-            "babbage": Endpoints.NON_CHAT.value,
-            "ada": Endpoints.NON_CHAT.value,
-        }
-
+class OpenAI(REST):
     @property
     def credentials(self) -> Dict[str, str]:
-        model = self._config["model"]
         # Fetch and check the key
         api_key = os.getenv("OPENAI_API_KEY")
         api_org = os.getenv("OPENAI_API_ORG")
         if api_key is None:
             raise ValueError(
                 "Could not find the API key to access the OpenAI API. Ensure you have an API key "
                 "set up via https://platform.openai.com/account/api-keys, then make it available as "
@@ -72,51 +48,42 @@
         elif r.status_code != 200:
             raise ValueError(
                 f"Error accessing api.openai.com ({r.status_code}): {r.text}"
             )
 
         response = r.json()["data"]
         models = [response[i]["id"] for i in range(len(response))]
-        if model not in models:
-            raise ValueError(
-                f"The specified model '{model}' is not available. Choices are: {sorted(set(models))}"
-            )
-
-        if model not in self.supported_models:
+        if self._name not in models:
             raise ValueError(
-                f"The specified model '{model}' is not supported by the /v1/completions endpoint. "
-                f"Choices are: {sorted(list(self.supported_models))} ."
-                "(See OpenAI API documentation: https://platform.openai.com/docs/models/)"
+                f"The specified model '{self._name}' is not available. Choices are: {sorted(set(models))}"
             )
 
         # Ensure endpoint is supported.
-        url = self._url if self._url else self.supported_models[self._config["model"]]
-        if url not in (Endpoints.NON_CHAT, Endpoints.CHAT):
+        if self._endpoint not in (Endpoints.NON_CHAT, Endpoints.CHAT):
             raise ValueError(
-                f"Endpoint {url} isn't supported. Please use one of: {Endpoints.CHAT}, {Endpoints.NON_CHAT}."
+                f"Endpoint {self._endpoint} isn't supported. Please use one of: {Endpoints.CHAT}, {Endpoints.NON_CHAT}."
             )
 
         assert api_key is not None
         return headers
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         headers = {
             **self._credentials,
             "Content-Type": "application/json",
         }
         api_responses: List[str] = []
         prompts = list(prompts)
-        url = self._url if self._url else self.supported_models[self._config["model"]]
 
         def _request(json_data: Dict[str, Any]) -> Dict[str, Any]:
             r = self.retry(
                 call_method=requests.post,
-                url=url,
+                url=self._endpoint,
                 headers=headers,
-                json={**json_data, **self._config},
+                json={**json_data, **self._config, "model": self._name},
                 timeout=self._max_request_time,
             )
             try:
                 r.raise_for_status()
             except HTTPError as ex:
                 res_content = srsly.json_loads(r.content.decode("utf-8"))
                 # Include specific error message in exception.
@@ -130,15 +97,15 @@
                     raise ValueError(f"API call failed: {responses}.")
                 else:
                     assert isinstance(prompts, Sized)
                     return {"error": [srsly.json_dumps(responses)] * len(prompts)}
 
             return responses
 
-        if url == Endpoints.CHAT:
+        if self._endpoint == Endpoints.CHAT:
             # The OpenAI API doesn't support batching for /chat/completions yet, so we have to send individual requests.
             for prompt in prompts:
                 responses = _request(
                     {"messages": [{"role": "user", "content": prompt}]}
                 )
                 if "error" in responses:
                     return responses["error"]
@@ -148,20 +115,47 @@
                 response = responses["choices"][0]
                 api_responses.append(
                     response.get("message", {}).get(
                         "content", srsly.json_dumps(response)
                     )
                 )
 
-        elif url == Endpoints.NON_CHAT:
+        elif self._endpoint == Endpoints.NON_CHAT:
             responses = _request({"prompt": prompts})
             if "error" in responses:
                 return responses["error"]
             assert len(responses["choices"]) == len(prompts)
 
             for response in responses["choices"]:
                 if "text" in response:
                     api_responses.append(response["text"])
                 else:
                     api_responses.append(srsly.json_dumps(response))
 
         return api_responses
+
+    @classmethod
+    def get_model_names(cls) -> Tuple[str, ...]:
+        return (
+            # gpt-4
+            "gpt-4",
+            "gpt-4-0314",
+            "gpt-4-32k",
+            "gpt-4-32k-0314",
+            # gpt-3.5
+            "gpt-3.5-turbo",
+            "gpt-3.5-turbo-16k",
+            "gpt-3.5-turbo-0613",
+            "gpt-3.5-turbo-0613-16k",
+            # text-davinci
+            "text-davinci-002",
+            "text-davinci-003",
+            # others
+            "code-davinci-002",
+            "text-curie-001",
+            "text-babbage-001",
+            "text-ada-001",
+            "davinci",
+            "curie",
+            "babbage",
+            "ada",
+        )
```

### Comparing `spacy-llm-0.3.2/spacy_llm/compat.py` & `spacy-llm-0.4.0/spacy_llm/compat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # mypy: ignore-errors
 import sys
 
 if sys.version_info[:2] >= (3, 8):  # Python 3.8+
-    from typing import Protocol, runtime_checkable, Literal
+    from typing import Literal, Protocol, runtime_checkable
 else:
-    from typing_extensions import Protocol, runtime_checkable, Literal  # noqa: F401
+    from typing_extensions import Literal, Protocol, runtime_checkable  # noqa: F401
 
 if sys.version_info[:2] >= (3, 9):  # Python 3.8+
     from typing import TypedDict  # noqa: F401
 else:
     from typing_extensions import TypedDict  # noqa: F401
 
 try:
@@ -16,22 +16,14 @@
 
     has_langchain = True
 except (ImportError, AttributeError):
     langchain = None
     has_langchain = False
 
 try:
-    import minichain
-
-    has_minichain = True
-except (ImportError, AttributeError):
-    minichain = None
-    has_minichain = False
-
-try:
     import torch
 
     has_torch = True
 except ImportError:
     torch = None
     has_torch = False
```

### Comparing `spacy-llm-0.3.2/spacy_llm/pipeline/llm.py` & `spacy-llm-0.4.0/spacy_llm/pipeline/llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,18 +30,16 @@
 
 @Language.factory(
     "llm",
     requires=[],
     assigns=[],
     default_config={
         "task": None,
-        "backend": {
-            "@llm_backends": "spacy.REST.v1",
-            "api": "OpenAI",
-            "config": {"model": "gpt-3.5-turbo"},
+        "model": {
+            "@llm_models": "spacy.GPT-3-5.v1",
             "strict": True,
         },
         "cache": {
             "@llm_misc": "spacy.BatchCache.v1",
             "path": None,
             "batch_size": 64,
             "max_batches_in_mem": 4,
@@ -50,80 +48,80 @@
         "validate_types": True,
     },
 )
 def make_llm(
     nlp: Language,
     name: str,
     task: Optional[LLMTask],
-    backend: PromptExecutor,
+    model: PromptExecutor,
     cache: Cache,
     save_io: bool,
     validate_types: bool,
 ) -> "LLMWrapper":
     """Construct an LLM component.
 
     nlp (Language): Pipeline.
     name (str): The component instance name, used to add entries to the
         losses during training.
     task (Optional[LLMTask]): An LLMTask can generate prompts for given docs, and can parse the LLM's responses into
         structured information and set that back on the docs.
-    backend (Callable[[Iterable[Any]], Iterable[Any]]]): Callable querying the specified LLM API.
+    model (Callable[[Iterable[Any]], Iterable[Any]]]): Callable querying the specified LLM API.
     cache (Cache): Cache to use for caching prompts and responses per doc (batch).
     save_io (bool): Whether to save LLM I/O (prompts and responses) in the `Doc._.llm_io` custom extension.
     validate_types (bool): Whether to check if signatures of configured backend and task are consistent.
     """
     if task is None:
         raise ValueError(
             "Argument `task` has not been specified, but is required (e. g. {'@llm_tasks': "
             "'spacy.NER.v2'})."
         )
     if validate_types:
-        validate_type_consistency(task, backend)
+        validate_type_consistency(task, model)
 
     return LLMWrapper(
         name=name,
         task=task,
         save_io=save_io,
-        backend=backend,
+        model=model,
         cache=cache,
         vocab=nlp.vocab,
     )
 
 
 class LLMWrapper(Pipe):
     """Pipeline component for wrapping LLMs."""
 
     def __init__(
         self,
         name: str = "LLMWrapper",
         *,
         vocab: Vocab,
         task: LLMTask,
-        backend: PromptExecutor,
+        model: PromptExecutor,
         cache: Cache,
         save_io: bool,
     ) -> None:
         """
         Component managing execution of prompts to LLM APIs and mapping responses back to Doc/Span instances.
 
         name (str): The component instance name, used to add entries to the
             losses during training.
         vocab (Vocab): Pipeline vocabulary.
         task (Optional[LLMTask]): An LLMTask can generate prompts for given docs, and can parse the LLM's responses into
             structured information and set that back on the docs.
-        backend (Callable[[Iterable[Any]], Iterable[Any]]]): Callable querying the specified LLM API.
+        model (Callable[[Iterable[Any]], Iterable[Any]]]): Callable querying the specified LLM API.
         cache (Cache): Cache to use for caching prompts and responses per doc (batch).
         save_io (bool): Whether to save LLM I/O (prompts and responses) in the `Doc._.llm_io` custom extension.
         """
         self._name = name
         self._task = task
-        self._backend = backend
+        self._model = model
         self._cache = cache
-        self._cache.vocab = vocab
         self._save_io = save_io
+        self._cache.initialize(vocab, self._task)
 
         # This is done this way because spaCy's `validate_init_settings` function
         # does not support `**kwargs: Any`.
         # See https://github.com/explosion/spaCy/blob/master/spacy/schemas.py#L111
         if isinstance(self._task, Initializable):
             self.initialize = self._task.initialize
 
@@ -173,16 +171,16 @@
         for doc_batch in spacy.util.minibatch(stream, batch_size):
             try:
                 yield from iter(self._process_docs(doc_batch))
             except Exception as e:
                 error_handler(self._name, self, doc_batch, e)
 
     def _process_docs(self, docs: List[Doc]) -> List[Doc]:
-        """Process a batch of docs with the configured LLM backend and task.
-        If a cache is configured, only sends prompts to backend for docs not found in cache.
+        """Process a batch of docs with the configured LLM model and task.
+        If a cache is configured, only sends prompts to model for docs not found in cache.
 
         docs (List[Doc]): Input batch of docs
         RETURNS (List[Doc]): Processed batch of docs with task annotations set
         """
         is_cached = [doc in self._cache for doc in docs]
         noncached_doc_batch = [doc for i, doc in enumerate(docs) if not is_cached[i]]
         if len(noncached_doc_batch) < len(docs):
@@ -194,15 +192,15 @@
 
         modified_docs: Iterator[Doc] = iter(())
         if len(noncached_doc_batch) > 0:
             n_iters = 3 if self._save_io else 2
             prompts_iters = tee(
                 self._task.generate_prompts(noncached_doc_batch), n_iters
             )
-            responses_iters = tee(self._backend(prompts_iters[0]), n_iters)
+            responses_iters = tee(self._model(prompts_iters[0]), n_iters)
             for prompt, response, doc in zip(
                 prompts_iters[1], responses_iters[1], noncached_doc_batch
             ):
                 logger.debug("Generated prompt for doc: %s\n%s", doc.text, prompt)
                 logger.debug("LLM response for doc: %s\n%s", doc.text, response)
 
             modified_docs = iter(
@@ -244,16 +242,16 @@
         RETURNS (bytes): The serialized object.
         """
 
         serialize = {}
 
         if isinstance(self._task, Serializable):
             serialize["task"] = lambda: self._task.to_bytes(exclude=exclude)  # type: ignore[attr-defined]
-        if isinstance(self._backend, Serializable):
-            serialize["backend"] = lambda: self._backend.to_bytes(exclude=exclude)  # type: ignore[attr-defined]
+        if isinstance(self._model, Serializable):
+            serialize["model"] = lambda: self._model.to_bytes(exclude=exclude)  # type: ignore[attr-defined]
 
         return util.to_bytes(serialize, exclude)
 
     def from_bytes(
         self,
         bytes_data: bytes,
         *,
@@ -266,16 +264,16 @@
         RETURNS (LLMWrapper): Modified LLMWrapper instance.
         """
 
         deserialize = {}
 
         if isinstance(self._task, Serializable):
             deserialize["task"] = lambda b: self._task.from_bytes(b, exclude=exclude)  # type: ignore[attr-defined]
-        if isinstance(self._backend, Serializable):
-            deserialize["backend"] = lambda b: self._backend.from_bytes(b, exclude=exclude)  # type: ignore[attr-defined]
+        if isinstance(self._model, Serializable):
+            deserialize["model"] = lambda b: self._model.from_bytes(b, exclude=exclude)  # type: ignore[attr-defined]
 
         util.from_bytes(bytes_data, deserialize, exclude)
         return self
 
     def to_disk(
         self, path: Path, *, exclude: Tuple[str] = cast(Tuple[str], tuple())
     ) -> None:
@@ -284,30 +282,30 @@
         exclude (Tuple): Names of properties to exclude from serialization.
         """
 
         serialize = {}
 
         if isinstance(self._task, Serializable):
             serialize["task"] = lambda p: self._task.to_disk(p, exclude=exclude)  # type: ignore[attr-defined]
-        if isinstance(self._backend, Serializable):
-            serialize["backend"] = lambda p: self._backend.to_disk(p, exclude=exclude)  # type: ignore[attr-defined]
+        if isinstance(self._model, Serializable):
+            serialize["model"] = lambda p: self._model.to_disk(p, exclude=exclude)  # type: ignore[attr-defined]
 
-        return util.to_disk(path, serialize, exclude)
+        util.to_disk(path, serialize, exclude)
 
     def from_disk(
         self, path: Path, *, exclude: Tuple[str] = cast(Tuple[str], tuple())
     ) -> "LLMWrapper":
         """Load the LLMWrapper from disk.
         path (Path): A path (currently unused).
         exclude (Tuple): Names of properties to exclude from deserialization.
         RETURNS (LLMWrapper): Modified LLMWrapper instance.
         """
 
         serialize = {}
 
         if isinstance(self._task, Serializable):
             serialize["task"] = lambda p: self._task.from_disk(p, exclude=exclude)  # type: ignore[attr-defined]
-        if isinstance(self._backend, Serializable):
-            serialize["backend"] = lambda p: self._backend.from_disk(p, exclude=exclude)  # type: ignore[attr-defined]
+        if isinstance(self._model, Serializable):
+            serialize["model"] = lambda p: self._model.from_disk(p, exclude=exclude)  # type: ignore[attr-defined]
 
         util.from_disk(path, serialize, exclude)
         return self
```

### Comparing `spacy-llm-0.3.2/spacy_llm/registry/normalizer.py` & `spacy-llm-0.4.0/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/__init__.py` & `spacy-llm-0.4.0/spacy_llm/tasks/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from .lemma import LemmaTask, make_lemma_task
 from .ner import NERTask, make_ner_task, make_ner_task_v2
 from .noop import NoopTask, make_noop_task
 from .rel import RELTask, make_rel_task
+from .sentiment import SentimentTask, make_sentiment_task
 from .spancat import SpanCatTask, make_spancat_task, make_spancat_task_v2
+from .summarization import SummarizationTask, make_summarization_task
 from .textcat import TextCatTask, make_textcat_task
 
 __all__ = [
     "make_lemma_task",
     "make_ner_task",
     "make_ner_task_v2",
     "make_noop_task",
     "make_rel_task",
+    "make_sentiment_task",
     "make_spancat_task",
     "make_spancat_task_v2",
+    "make_summarization_task",
     "make_textcat_task",
     "LemmaTask",
     "NERTask",
     "NoopTask",
     "RELTask",
+    "SentimentTask",
     "SpanCatTask",
+    "SummarizationTask",
     "TextCatTask",
 ]
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/lemma.py` & `spacy-llm-0.4.0/spacy_llm/tasks/lemma.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from typing import Any, Callable, Dict, Iterable, List, Optional, Type
 
 import jinja2
+from pydantic import BaseModel
 from spacy.language import Language
 from spacy.scorer import Scorer
 from spacy.tokens import Doc
 from spacy.training import Example
 
 from ..registry import registry
 from ..ty import ExamplesConfigType
 from .templates import read_template
 from .util import SerializableTask
-from .util.examples import LemmaExample
-from .util.serialization import ExampleType
 
 _DEFAULT_LEMMA_TEMPLATE_V1 = read_template("lemma")
 
 
+class LemmaExample(BaseModel):
+    text: str
+    lemmas: List[Dict[str, str]]
+
+
 @registry.llm_tasks("spacy.Lemma.v1")
 def make_lemma_task(
     template: str = _DEFAULT_LEMMA_TEMPLATE_V1,
     examples: ExamplesConfigType = None,
 ):
     """Lemma.v1 task factory.
 
     template (str): Prompt template passed to the model.
     examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
         reads a file containing task examples for few-shot learning. If None is
         passed, then zero-shot learning will be used.
     """
     raw_examples = examples() if callable(examples) else examples
-    span_examples = (
+    lemma_examples = (
         [LemmaExample(**eg) for eg in raw_examples] if raw_examples else None
     )
 
-    return LemmaTask(template=template, examples=span_examples)
+    return LemmaTask(template=template, examples=lemma_examples)
 
 
 class LemmaTask(SerializableTask[LemmaExample]):
     def __init__(
         self,
         template: str = _DEFAULT_LEMMA_TEMPLATE_V1,
         examples: Optional[List[LemmaExample]] = None,
@@ -46,36 +50,45 @@
 
         template (str): Prompt template passed to the model.
         examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
             reads a file containing task examples for few-shot learning. If None is
             passed, then zero-shot learning will be used.
         """
         self._template = template
-        self._examples = examples
+        self._prompt_examples = examples or []
 
     def initialize(
         self,
         get_examples: Callable[[], Iterable["Example"]],
         nlp: Language,
+        n_prompt_examples: int = 0,
         **kwargs: Any,
     ) -> None:
-        """Nothing to initialize for the LEMMA task.
+        """Initializes prompt examples from Doc examples.
         get_examples (Callable[[], Iterable["Example"]]): Callable that provides examples
             for initialization.
         nlp (Language): Language instance.
-        labels (List[str]): Optional list of labels.
+        n_prompt_examples (int): How many prompt examples to infer from the provided Example objects.
+            0 by default. Takes all examples if set to -1.
         """
+        for eg in get_examples():
+            if n_prompt_examples < 0 or len(self._prompt_examples) < n_prompt_examples:
+                self._prompt_examples.append(self._create_prompt_example(eg))
+
+    @property
+    def prompt_template(self) -> str:
+        return self._template
 
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=doc.text,
-                examples=self._examples,
+                examples=self._prompt_examples,
             )
             yield prompt
 
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[str]
     ) -> Iterable[Doc]:
         for doc, prompt_response in zip(docs, responses):
@@ -110,9 +123,14 @@
         return Scorer.score_token_attr(examples, "pos")
 
     @property
     def _cfg_keys(self) -> List[str]:
         return ["_template"]
 
     @property
-    def _Example(self) -> Type[ExampleType]:
+    def _Example(self) -> Type[LemmaExample]:
         return LemmaExample
+
+    def _create_prompt_example(self, example: Example) -> LemmaExample:
+        """Create a lemma prompt example from a spaCy example."""
+        lemma_dict = [{t.text: t.lemma_} for t in example.reference]
+        return LemmaExample(text=example.reference.text, lemmas=lemma_dict)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/ner.py` & `spacy-llm-0.4.0/spacy_llm/tasks/spancat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,198 +1,227 @@
+from collections import defaultdict
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 from spacy.language import Language
-from spacy.scorer import get_ner_prf
+from spacy.pipeline.spancat import spancat_score
 from spacy.tokens import Doc, Span
 from spacy.training import Example
-from spacy.util import filter_spans
 
 from ..compat import Literal
 from ..registry import registry
 from ..ty import ExamplesConfigType
 from ..util import split_labels
+from .span import SpanExample, SpanTask
 from .templates import read_template
-from .util import SpanExample, SpanTask
 
-_DEFAULT_NER_TEMPLATE_V1 = read_template("ner")
-_DEFAULT_NER_TEMPLATE_V2 = read_template("ner.v2")
+_DEFAULT_SPANCAT_TEMPLATE_V1 = read_template("spancat")
+_DEFAULT_SPANCAT_TEMPLATE_V2 = read_template("spancat.v2")
 
 
-@registry.llm_tasks("spacy.NER.v1")
-def make_ner_task(
+@registry.llm_tasks("spacy.SpanCat.v1")
+def make_spancat_task(
     labels: str = "",
     examples: Optional[Callable[[], Iterable[Any]]] = None,
     normalizer: Optional[Callable[[str], str]] = None,
     alignment_mode: Literal["strict", "contract", "expand"] = "contract",
     case_sensitive_matching: bool = False,
     single_match: bool = False,
 ):
-    """NER.v1 task factory.
+    """SpanCat.v1 task factory.
 
     labels (str): Comma-separated list of labels to pass to the template.
         Leave empty to populate it at initialization time (only if examples are provided).
     template (str): Prompt template passed to the model.
     label_definitions (Optional[Dict[str, str]]): Map of label -> description
         of the label to help the language model output the entities wanted.
         It is usually easier to provide these definitions rather than
         full examples, although both can be provided.
+    spans_key (str): Key of the `Doc.spans` dict to save under.
     examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
         reads a file containing task examples for few-shot learning. If None is
         passed, then zero-shot learning will be used.
     normalizer (Optional[Callable[[str], str]]): optional normalizer function.
     alignment_mode (str): "strict", "contract" or "expand".
     case_sensitive: Whether to search without case sensitivity.
     single_match (bool): If False, allow one substring to match multiple times in
         the text. If True, returns the first hit.
     """
     labels_list = split_labels(labels)
-
     span_examples = (
         [SpanExample(**eg) for eg in examples()] if callable(examples) else examples
     )
-    return NERTask(
+    return SpanCatTask(
         labels=labels_list,
-        template=_DEFAULT_NER_TEMPLATE_V1,
-        examples=span_examples,
+        template=_DEFAULT_SPANCAT_TEMPLATE_V1,
+        prompt_examples=span_examples,
         normalizer=normalizer,
         alignment_mode=alignment_mode,
         case_sensitive_matching=case_sensitive_matching,
         single_match=single_match,
     )
 
 
-@registry.llm_tasks("spacy.NER.v2")
-def make_ner_task_v2(
+@registry.llm_tasks("spacy.SpanCat.v2")
+def make_spancat_task_v2(
     labels: Union[List[str], str] = [],
-    template: str = _DEFAULT_NER_TEMPLATE_V2,
+    template: str = _DEFAULT_SPANCAT_TEMPLATE_V2,
     label_definitions: Optional[Dict[str, str]] = None,
     examples: ExamplesConfigType = None,
     normalizer: Optional[Callable[[str], str]] = None,
     alignment_mode: Literal["strict", "contract", "expand"] = "contract",
     case_sensitive_matching: bool = False,
     single_match: bool = False,
 ):
-    """NER.v2 task factory.
+    """SpanCat.v2 task factory.
 
     labels (Union[str, List[str]]): List of labels to pass to the template,
         either an actual list or a comma-separated string.
         Leave empty to populate it at initialization time (only if examples are provided).
     template (str): Prompt template passed to the model.
     label_definitions (Optional[Dict[str, str]]): Map of label -> description
         of the label to help the language model output the entities wanted.
         It is usually easier to provide these definitions rather than
         full examples, although both can be provided.
+    spans_key (str): Key of the `Doc.spans` dict to save under.
     examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
         reads a file containing task examples for few-shot learning. If None is
         passed, then zero-shot learning will be used.
     normalizer (Optional[Callable[[str], str]]): optional normalizer function.
     alignment_mode (str): "strict", "contract" or "expand".
     case_sensitive: Whether to search without case sensitivity.
     single_match (bool): If False, allow one substring to match multiple times in
         the text. If True, returns the first hit.
     """
     labels_list = split_labels(labels)
     raw_examples = examples() if callable(examples) else examples
     span_examples = [SpanExample(**eg) for eg in raw_examples] if raw_examples else None
-
-    return NERTask(
+    return SpanCatTask(
         labels=labels_list,
         template=template,
         label_definitions=label_definitions,
-        examples=span_examples,
+        prompt_examples=span_examples,
         normalizer=normalizer,
         alignment_mode=alignment_mode,
         case_sensitive_matching=case_sensitive_matching,
         single_match=single_match,
     )
 
 
-class NERTask(SpanTask):
+class SpanCatTask(SpanTask):
     def __init__(
         self,
         labels: List[str] = [],
-        template: str = _DEFAULT_NER_TEMPLATE_V2,
+        template: str = _DEFAULT_SPANCAT_TEMPLATE_V2,
         label_definitions: Optional[Dict[str, str]] = None,
-        examples: Optional[List[SpanExample]] = None,
+        spans_key: str = "sc",
+        prompt_examples: Optional[List[SpanExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
         alignment_mode: Literal["strict", "contract", "expand"] = "contract",
         case_sensitive_matching: bool = False,
         single_match: bool = False,
     ):
-        """Default NER task.
+        """Default SpanCat task.
 
         labels (List[str]): List of labels to pass to the template.
             Leave empty to populate it at initialization time (only if examples are provided).
         template (str): Prompt template passed to the model.
         label_definitions (Optional[Dict[str, str]]): Map of label -> description
             of the label to help the language model output the entities wanted.
             It is usually easier to provide these definitions rather than
             full examples, although both can be provided.
-        examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
+        spans_key (str): Key of the `Doc.spans` dict to save under.
+        prompt_examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
             reads a file containing task examples for few-shot learning. If None is
             passed, then zero-shot learning will be used.
         normalizer (Optional[Callable[[str], str]]): optional normalizer function.
         alignment_mode (str): "strict", "contract" or "expand".
         case_sensitive: Whether to search without case sensitivity.
         single_match (bool): If False, allow one substring to match multiple times in
             the text. If True, returns the first hit.
         """
-        super().__init__(
+        super(SpanCatTask, self).__init__(
             labels=labels,
             template=template,
             label_definitions=label_definitions,
-            examples=examples,
+            prompt_examples=prompt_examples,
             normalizer=normalizer,
             alignment_mode=alignment_mode,
             case_sensitive_matching=case_sensitive_matching,
             single_match=single_match,
         )
+        self._spans_key = spans_key
+
+    def assign_spans(
+        self,
+        doc: Doc,
+        spans: List[Span],
+    ) -> None:
+        """Assign spans to the document."""
+        doc.spans[self._spans_key] = sorted(spans)  # type: ignore [type-var]
+
+    def scorer(
+        self,
+        examples: Iterable[Example],
+    ) -> Dict[str, Any]:
+        return spancat_score(
+            examples,
+            spans_key=self._spans_key,
+            allow_overlap=True,
+        )
 
     def initialize(
         self,
         get_examples: Callable[[], Iterable["Example"]],
         nlp: Language,
         labels: List[str] = [],
+        n_prompt_examples: int = 0,
         **kwargs: Any,
     ) -> None:
-        """Initialize the NER task, by auto-discovering labels.
+        """Initialize the SpanCat task, by auto-discovering labels.
 
         Labels can be set through, by order of precedence:
 
         - the `[initialize]` section of the pipeline configuration
         - the `labels` argument supplied to the task factory
         - the labels found in the examples
 
         get_examples (Callable[[], Iterable["Example"]]): Callable that provides examples
             for initialization.
         nlp (Language): Language instance.
         labels (List[str]): Optional list of labels.
+        n_prompt_examples (int): How many prompt examples to infer from the Example objects.
+            0 by default. Takes all examples if set to -1.
         """
-
-        examples = get_examples()
-
         if not labels:
             labels = list(self._label_dict.values())
+        infer_labels = not labels
 
-        if not labels:
-            label_set = set()
-
-            for eg in examples:
-                for ent in eg.reference.ents:
-                    label_set.add(ent.label_)
-            labels = list(label_set)
-
-        self._label_dict = {self._normalizer(label): label for label in labels}
+        for eg in get_examples():
+            if infer_labels:
+                for span in eg.reference.spans.get(self._spans_key, []):
+                    labels.append(span.label_)
+            if n_prompt_examples < 0 or len(self._prompt_examples) < n_prompt_examples:
+                self._prompt_examples.append(self._create_prompt_example(eg))
+
+        self._label_dict = {
+            self._normalizer(label): label for label in sorted(set(labels))
+        }
+
+    @property
+    def _cfg_keys(self) -> List[str]:
+        return [
+            "_spans_key",
+            "_label_dict",
+            "_template",
+            "_label_definitions",
+            "_alignment_mode",
+            "_case_sensitive_matching",
+            "_single_match",
+        ]
+
+    def _create_prompt_example(self, example: Example) -> SpanExample:
+        """Create a spancat prompt example from a spaCy example."""
+        entities = defaultdict(list)
+        for span in example.reference.spans[self._spans_key]:
+            entities[span.label_].append(span.text)
 
-    def assign_spans(
-        self,
-        doc: Doc,
-        spans: List[Span],
-    ) -> None:
-        """Assign spans to the document."""
-        doc.set_ents(filter_spans(spans))
-
-    def scorer(
-        self,
-        examples: Iterable[Example],
-    ) -> Dict[str, Any]:
-        return get_ner_prf(examples)
+        return SpanExample(text=example.reference.text, entities=entities)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/rel.py` & `spacy-llm-0.4.0/spacy_llm/tasks/rel.py`

 * *Files 19% similar despite different names*

```diff
@@ -89,71 +89,77 @@
     labels_list = split_labels(labels)
     raw_examples = examples() if callable(examples) else examples
     rel_examples = [RELExample(**eg) for eg in raw_examples] if raw_examples else None
     return RELTask(
         labels=labels_list,
         template=template,
         label_definitions=label_definitions,
-        examples=rel_examples,
+        prompt_examples=rel_examples,
         normalizer=normalizer,
         verbose=verbose,
     )
 
 
 class RELTask(SerializableTask[RELExample]):
     def __init__(
         self,
         labels: List[str] = [],
         template: str = _DEFAULT_REL_TEMPLATE,
         label_definitions: Optional[Dict[str, str]] = None,
-        examples: Optional[List[RELExample]] = None,
+        prompt_examples: Optional[List[RELExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
         verbose: bool = False,
     ):
         """Default REL task. Populates a `Doc._.rel` custom attribute.
 
         labels (List[str]): List of labels to pass to the template.
             Leave empty to populate it at initialization time (only if examples are provided).
         template (str): Prompt template passed to the model.
         label_definitions (Optional[Dict[str, str]]): Map of label -> description
             of the label to help the language model output the entities wanted.
             It is usually easier to provide these definitions rather than
             full examples, although both can be provided.
-        examples (Optional[Callable[[], List[RELExample]]]): Optional callable that
+        prompt_examples (Optional[Callable[[], List[RELExample]]]): Optional callable that
             reads a file containing task examples for few-shot learning. If None is
             passed, then zero-shot learning will be used.
         normalizer (Optional[Callable[[str], str]]): Optional normalizer function.
         verbose (bool): Controls the verbosity of the task.
         """
         self._normalizer = normalizer if normalizer else lowercase_normalizer()
-        self._label_dict = {self._normalizer(label): label for label in labels}
+        self._label_dict = {
+            self._normalizer(label): label for label in sorted(set(labels))
+        }
         self._template = template
         self._label_definitions = label_definitions
-        self._examples = examples
+        self._prompt_examples = prompt_examples or []
         self._verbose = verbose
 
     @classmethod
-    def _check_rel_extention(cls):
+    def _check_rel_extension(cls):
         """Add `rel` extension if need be."""
         if not Doc.has_extension("rel"):
             Doc.set_extension("rel", default=[])
 
     @property
     def labels(self) -> Tuple[str, ...]:
         return tuple(self._label_dict.values())
 
+    @property
+    def prompt_template(self) -> str:
+        return self._template
+
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=_preannotate(doc),
                 labels=list(self._label_dict.values()),
                 label_definitions=self._label_definitions,
-                examples=self._examples,
+                examples=self._prompt_examples,
                 preannotate=_preannotate,
             )
             yield prompt
 
     def _format_response(self, response: str) -> List[RelationItem]:
         """Parse raw string response into a structured format"""
         relations = []
@@ -167,63 +173,87 @@
                     show=self._verbose,
                 )
         return relations
 
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[str]
     ) -> Iterable[Doc]:
-        self._check_rel_extention()
+        self._check_rel_extension()
 
         for doc, prompt_response in zip(docs, responses):
             rels = self._format_response(prompt_response)
             doc._.rel = rels
             yield doc
 
     def initialize(
         self,
         get_examples: Callable[[], Iterable["Example"]],
         nlp: Language,
         labels: List[str] = [],
+        n_prompt_examples: int = 0,
     ) -> None:
         """Initialize the SpanCat task, by auto-discovering labels.
 
         Labels can be set through, by order of precedence:
 
         - the `[initialize]` section of the pipeline configuration
         - the `labels` argument supplied to the task factory
         - the labels found in the examples
 
         get_examples (Callable[[], Iterable["Example"]]): Callable that provides examples
             for initialization.
         nlp (Language): Language instance.
         labels (List[str]): Optional list of labels.
+        n_prompt_examples (int): How many prompt examples to infer from the Example objects.
+            0 by default. Takes all examples if set to -1.
         """
-        self._check_rel_extention()
-
-        examples = get_examples()
+        self._check_rel_extension()
 
         if not labels:
             labels = list(self._label_dict.values())
+        infer_labels = not labels
 
-        if not labels:
-            label_set = set()
+        if infer_labels:
+            labels = []
 
-            for eg in examples:
+        for eg in get_examples():
+            if infer_labels:
                 rels: List[RelationItem] = eg.reference._.rel
                 for rel in rels:
-                    label_set.add(rel.relation)
-            labels = list(label_set)
-
-        self._label_dict = {self._normalizer(label): label for label in labels}
+                    labels.append(rel.relation)
+            if n_prompt_examples < 0 or len(self._prompt_examples) < n_prompt_examples:
+                self._prompt_examples.append(self._create_prompt_example(eg))
+
+        self._label_dict = {
+            self._normalizer(label): label for label in sorted(set(labels))
+        }
 
     @property
     def _cfg_keys(self) -> List[str]:
         return [
             "_label_dict",
             "_template",
             "_label_definitions",
             "_verbose",
         ]
 
     @property
     def _Example(self) -> Type[RELExample]:
         return RELExample
+
+    def _create_prompt_example(self, example: Example) -> RELExample:
+        """Create a REL prompt example from a spaCy example."""
+        entities = [
+            EntityItem(
+                start_char=ent.start_char,
+                end_char=ent.end_char,
+                label=ent.label_,
+            )
+            for ent in example.reference.ents
+        ]
+
+        rel_example = RELExample(
+            text=example.reference.text,
+            ents=entities,
+            relations=example.reference._.rel,
+        )
+        return rel_example
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/spancat.py` & `spacy-llm-0.4.0/spacy_llm/tasks/ner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,215 +1,212 @@
+from collections import defaultdict
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 from spacy.language import Language
-from spacy.pipeline.spancat import spancat_score
+from spacy.scorer import get_ner_prf
 from spacy.tokens import Doc, Span
 from spacy.training import Example
+from spacy.util import filter_spans
 
 from ..compat import Literal
 from ..registry import registry
 from ..ty import ExamplesConfigType
 from ..util import split_labels
+from .span import SpanExample, SpanTask
 from .templates import read_template
-from .util import SpanExample, SpanTask
 
-_DEFAULT_SPANCAT_TEMPLATE_V1 = read_template("spancat")
-_DEFAULT_SPANCAT_TEMPLATE_V2 = read_template("spancat.v2")
+_DEFAULT_NER_TEMPLATE_V1 = read_template("ner")
+_DEFAULT_NER_TEMPLATE_V2 = read_template("ner.v2")
 
 
-@registry.llm_tasks("spacy.SpanCat.v1")
-def make_spancat_task(
+@registry.llm_tasks("spacy.NER.v1")
+def make_ner_task(
     labels: str = "",
     examples: Optional[Callable[[], Iterable[Any]]] = None,
     normalizer: Optional[Callable[[str], str]] = None,
     alignment_mode: Literal["strict", "contract", "expand"] = "contract",
     case_sensitive_matching: bool = False,
     single_match: bool = False,
 ):
-    """SpanCat.v1 task factory.
+    """NER.v1 task factory.
 
     labels (str): Comma-separated list of labels to pass to the template.
         Leave empty to populate it at initialization time (only if examples are provided).
     template (str): Prompt template passed to the model.
     label_definitions (Optional[Dict[str, str]]): Map of label -> description
         of the label to help the language model output the entities wanted.
         It is usually easier to provide these definitions rather than
         full examples, although both can be provided.
-    spans_key (str): Key of the `Doc.spans` dict to save under.
     examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
         reads a file containing task examples for few-shot learning. If None is
         passed, then zero-shot learning will be used.
     normalizer (Optional[Callable[[str], str]]): optional normalizer function.
     alignment_mode (str): "strict", "contract" or "expand".
     case_sensitive: Whether to search without case sensitivity.
     single_match (bool): If False, allow one substring to match multiple times in
         the text. If True, returns the first hit.
     """
     labels_list = split_labels(labels)
+
     span_examples = (
         [SpanExample(**eg) for eg in examples()] if callable(examples) else examples
     )
-    return SpanCatTask(
+    return NERTask(
         labels=labels_list,
-        template=_DEFAULT_SPANCAT_TEMPLATE_V1,
-        examples=span_examples,
+        template=_DEFAULT_NER_TEMPLATE_V1,
+        prompt_examples=span_examples,
         normalizer=normalizer,
         alignment_mode=alignment_mode,
         case_sensitive_matching=case_sensitive_matching,
         single_match=single_match,
     )
 
 
-@registry.llm_tasks("spacy.SpanCat.v2")
-def make_spancat_task_v2(
+@registry.llm_tasks("spacy.NER.v2")
+def make_ner_task_v2(
     labels: Union[List[str], str] = [],
-    template: str = _DEFAULT_SPANCAT_TEMPLATE_V2,
+    template: str = _DEFAULT_NER_TEMPLATE_V2,
     label_definitions: Optional[Dict[str, str]] = None,
     examples: ExamplesConfigType = None,
     normalizer: Optional[Callable[[str], str]] = None,
     alignment_mode: Literal["strict", "contract", "expand"] = "contract",
     case_sensitive_matching: bool = False,
     single_match: bool = False,
 ):
-    """SpanCat.v2 task factory.
+    """NER.v2 task factory.
 
     labels (Union[str, List[str]]): List of labels to pass to the template,
         either an actual list or a comma-separated string.
         Leave empty to populate it at initialization time (only if examples are provided).
     template (str): Prompt template passed to the model.
     label_definitions (Optional[Dict[str, str]]): Map of label -> description
         of the label to help the language model output the entities wanted.
         It is usually easier to provide these definitions rather than
         full examples, although both can be provided.
-    spans_key (str): Key of the `Doc.spans` dict to save under.
     examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
         reads a file containing task examples for few-shot learning. If None is
         passed, then zero-shot learning will be used.
     normalizer (Optional[Callable[[str], str]]): optional normalizer function.
     alignment_mode (str): "strict", "contract" or "expand".
     case_sensitive: Whether to search without case sensitivity.
     single_match (bool): If False, allow one substring to match multiple times in
         the text. If True, returns the first hit.
     """
     labels_list = split_labels(labels)
     raw_examples = examples() if callable(examples) else examples
     span_examples = [SpanExample(**eg) for eg in raw_examples] if raw_examples else None
-    return SpanCatTask(
+
+    return NERTask(
         labels=labels_list,
         template=template,
         label_definitions=label_definitions,
-        examples=span_examples,
+        prompt_examples=span_examples,
         normalizer=normalizer,
         alignment_mode=alignment_mode,
         case_sensitive_matching=case_sensitive_matching,
         single_match=single_match,
     )
 
 
-class SpanCatTask(SpanTask):
+class NERTask(SpanTask):
     def __init__(
         self,
         labels: List[str] = [],
-        template: str = _DEFAULT_SPANCAT_TEMPLATE_V2,
+        template: str = _DEFAULT_NER_TEMPLATE_V2,
         label_definitions: Optional[Dict[str, str]] = None,
-        spans_key: str = "sc",
-        examples: Optional[List[SpanExample]] = None,
+        prompt_examples: Optional[List[SpanExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
         alignment_mode: Literal["strict", "contract", "expand"] = "contract",
         case_sensitive_matching: bool = False,
         single_match: bool = False,
     ):
-        """Default SpanCat task.
+        """Default NER task.
 
         labels (List[str]): List of labels to pass to the template.
             Leave empty to populate it at initialization time (only if examples are provided).
         template (str): Prompt template passed to the model.
         label_definitions (Optional[Dict[str, str]]): Map of label -> description
             of the label to help the language model output the entities wanted.
             It is usually easier to provide these definitions rather than
             full examples, although both can be provided.
-        spans_key (str): Key of the `Doc.spans` dict to save under.
         examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
             reads a file containing task examples for few-shot learning. If None is
             passed, then zero-shot learning will be used.
         normalizer (Optional[Callable[[str], str]]): optional normalizer function.
         alignment_mode (str): "strict", "contract" or "expand".
         case_sensitive: Whether to search without case sensitivity.
         single_match (bool): If False, allow one substring to match multiple times in
             the text. If True, returns the first hit.
         """
-        super(SpanCatTask, self).__init__(
+        super().__init__(
             labels=labels,
             template=template,
             label_definitions=label_definitions,
-            examples=examples,
+            prompt_examples=prompt_examples,
             normalizer=normalizer,
             alignment_mode=alignment_mode,
             case_sensitive_matching=case_sensitive_matching,
             single_match=single_match,
         )
-        self._spans_key = spans_key
-
-    def assign_spans(
-        self,
-        doc: Doc,
-        spans: List[Span],
-    ) -> None:
-        """Assign spans to the document."""
-        doc.spans[self._spans_key] = sorted(spans)  # type: ignore [type-var]
-
-    def scorer(
-        self,
-        examples: Iterable[Example],
-    ) -> Dict[str, Any]:
-        return spancat_score(
-            examples,
-            spans_key=self._spans_key,
-            allow_overlap=True,
-        )
 
     def initialize(
         self,
         get_examples: Callable[[], Iterable["Example"]],
         nlp: Language,
         labels: List[str] = [],
+        n_prompt_examples: int = 0,
         **kwargs: Any,
     ) -> None:
-        """Initialize the SpanCat task, by auto-discovering labels.
+        """Initialize the NER task, by auto-discovering labels.
 
         Labels can be set through, by order of precedence:
 
         - the `[initialize]` section of the pipeline configuration
         - the `labels` argument supplied to the task factory
         - the labels found in the examples
 
         get_examples (Callable[[], Iterable["Example"]]): Callable that provides examples
             for initialization.
         nlp (Language): Language instance.
         labels (List[str]): Optional list of labels.
+        n_prompt_examples (int): How many prompt examples to infer from the Example objects.
+            0 by default. Takes all examples if set to -1.
         """
-        examples = get_examples()
-
         if not labels:
             labels = list(self._label_dict.values())
+        infer_labels = not labels
 
-        if not labels:
-            label_set = set()
+        if infer_labels:
+            labels = []
+
+        for eg in get_examples():
+            if infer_labels:
+                for ent in eg.reference.ents:
+                    labels.append(ent.label_)
+            if n_prompt_examples < 0 or len(self._prompt_examples) < n_prompt_examples:
+                self._prompt_examples.append(self._create_prompt_example(eg))
+
+        self._label_dict = {
+            self._normalizer(label): label for label in sorted(set(labels))
+        }
+
+    def assign_spans(
+        self,
+        doc: Doc,
+        spans: List[Span],
+    ) -> None:
+        """Assign spans to the document."""
+        doc.set_ents(filter_spans(spans))
+
+    def scorer(
+        self,
+        examples: Iterable[Example],
+    ) -> Dict[str, Any]:
+        return get_ner_prf(examples)
+
+    def _create_prompt_example(self, example: Example) -> SpanExample:
+        """Create an NER prompt example from a spaCy example."""
+        entities = defaultdict(list)
+        for ent in example.reference.ents:
+            entities[ent.label_].append(ent.text)
 
-            for eg in examples:
-                for span in eg.reference.spans.get(self._spans_key, []):
-                    label_set.add(span.label_)
-            labels = list(label_set)
-
-        self._label_dict = {self._normalizer(label): label for label in labels}
-
-    @property
-    def _cfg_keys(self) -> List[str]:
-        return [
-            "_spans_key",
-            "_label_dict",
-            "_template",
-            "_label_definitions",
-            "_alignment_mode",
-            "_case_sensitive_matching",
-            "_single_match",
-        ]
+        return SpanExample(text=example.reference.text, entities=entities)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/templates/lemma.jinja` & `spacy-llm-0.4.0/spacy_llm/tasks/templates/lemma.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/templates/ner.jinja` & `spacy-llm-0.4.0/spacy_llm/tasks/templates/ner.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/templates/ner.v2.jinja` & `spacy-llm-0.4.0/spacy_llm/tasks/templates/ner.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/templates/rel.jinja` & `spacy-llm-0.4.0/spacy_llm/tasks/templates/rel.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/templates/spancat.jinja` & `spacy-llm-0.4.0/spacy_llm/tasks/templates/spancat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/templates/spancat.v2.jinja` & `spacy-llm-0.4.0/spacy_llm/tasks/templates/spancat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.jinja` & `spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.v2.jinja` & `spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.v3.jinja` & `spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/textcat.py` & `spacy-llm-0.4.0/spacy_llm/tasks/textcat.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     raw_examples = examples() if callable(examples) else examples
     textcat_examples = (
         [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
     )
     return TextCatTask(
         labels=labels_list,
         template=_DEFAULT_TEXTCAT_TEMPLATE_V1,
-        examples=textcat_examples,
+        prompt_examples=textcat_examples,
         normalizer=normalizer,
         exclusive_classes=exclusive_classes,
         allow_none=allow_none,
         verbose=verbose,
     )
 
 
@@ -118,15 +118,15 @@
     raw_examples = examples() if callable(examples) else examples
     textcat_examples = (
         [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
     )
     return TextCatTask(
         labels=labels_list,
         template=template,
-        examples=textcat_examples,
+        prompt_examples=textcat_examples,
         normalizer=normalizer,
         exclusive_classes=exclusive_classes,
         allow_none=allow_none,
         verbose=verbose,
     )
 
 
@@ -178,29 +178,29 @@
         [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
     )
 
     return TextCatTask(
         labels=labels_list,
         template=template,
         label_definitions=label_definitions,
-        examples=textcat_examples,
+        prompt_examples=textcat_examples,
         normalizer=normalizer,
         exclusive_classes=exclusive_classes,
         allow_none=allow_none,
         verbose=verbose,
     )
 
 
 class TextCatTask(SerializableTask[TextCatExample]):
     def __init__(
         self,
         labels: List[str] = [],
         template: str = _DEFAULT_TEXTCAT_TEMPLATE_V3,
         label_definitions: Optional[Dict[str, str]] = None,
-        examples: Optional[List[TextCatExample]] = None,
+        prompt_examples: Optional[List[TextCatExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
         exclusive_classes: bool = False,
         allow_none: bool = True,
         verbose: bool = False,
     ):
         """Default TextCat task.
 
@@ -218,28 +218,30 @@
 
         labels (List[str]): List of labels to pass to the template. This task
             assumes binary classification if a single label is provided.
             Leave empty to populate it at initialization time (only if examples are provided).
         template (str): Prompt template passed to the model.
         label_definitions (Optional[Dict[str, str]]): Optional dict mapping a label to a description of that label.
             These descriptions are added to the prompt to help instruct the LLM on what to extract.
-        examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
+        prompt_examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
             reads a file containing task examples for few-shot learning. If None is
             passed, then zero-shot learning will be used.
         normalizer (Optional[Callable[[str], str]]): Optional normalizer function.
         exclusive_classes (bool): If True, require the language model to suggest only one
             label per class. This is automatically set when using binary classification.
         allow_none (bool): if True, there might be cases where no label is applicable.
         verbose (bool): If True, show extra information.
         """
         self._template = template
         self._normalizer = normalizer if normalizer else lowercase_normalizer()
-        self._label_dict = {self._normalizer(label): label for label in labels}
+        self._label_dict = {
+            self._normalizer(label): label for label in sorted(set(labels))
+        }
         self._label_definitions = label_definitions
-        self._examples = examples
+        self._prompt_examples = prompt_examples or []
         # Textcat configuration
         self._use_binary = True if len(self._label_dict) == 1 else False
         self._exclusive_classes = exclusive_classes
         self._allow_none = allow_none
         self._verbose = verbose
 
         if self._use_binary and not self._exclusive_classes:
@@ -249,23 +251,27 @@
             )
             self._exclusive_classes = True
 
     @property
     def labels(self) -> Tuple[str, ...]:
         return tuple(self._label_dict.values())
 
+    @property
+    def prompt_template(self) -> str:
+        return self._template
+
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=doc.text,
                 labels=list(self._label_dict.values()),
                 label_definitions=self._label_definitions,
-                examples=self._examples,
+                examples=self._prompt_examples,
                 exclusive_classes=self._exclusive_classes,
                 allow_none=self._allow_none,
             )
             yield prompt
 
     def _format_response(self, response: str) -> Dict[str, float]:
         """Parse raw string response into a structured format
@@ -320,43 +326,49 @@
         )
 
     def initialize(
         self,
         get_examples: Callable[[], Iterable["Example"]],
         nlp: Language,
         labels: List[str] = [],
+        n_prompt_examples: int = 0,
         **kwargs: Any,
     ) -> None:
         """Initialize the TextCat task, by auto-discovering labels.
 
         Labels can be set through, by order of precedence:
 
         - the `[initialize]` section of the pipeline configuration
         - the `labels` argument supplied to the task factory
         - the labels found in the examples
 
         get_examples (Callable[[], Iterable["Example"]]): Callable that provides examples
             for initialization.
         nlp (Language): Language instance.
         labels (List[str]): Optional list of labels.
+        n_prompt_examples (int): How many prompt examples to infer from the Example objects.
+            0 by default. Takes all examples if set to -1.
         """
-        examples = get_examples()
-
         if not labels:
             labels = list(self._label_dict.values())
+        infer_labels = not labels
 
-        if not labels:
-            label_set = set()
+        if infer_labels:
+            labels = []
 
-            for eg in examples:
+        for eg in get_examples():
+            if infer_labels:
                 for cat in eg.reference.cats.keys():
-                    label_set.add(cat)
-            labels = list(label_set)
-
-        self._label_dict = {self._normalizer(label): label for label in labels}
+                    labels.append(cat)
+            if n_prompt_examples < 0 or len(self._prompt_examples) < n_prompt_examples:
+                self._prompt_examples.append(self._create_prompt_example(eg))
+
+        self._label_dict = {
+            self._normalizer(label): label for label in sorted(set(labels))
+        }
 
     @property
     def _cfg_keys(self) -> List[str]:
         return [
             "_template",
             "_label_dict",
             "_label_definitions",
@@ -365,7 +377,30 @@
             "_allow_none",
             "_verbose",
         ]
 
     @property
     def _Example(self) -> Type[TextCatExample]:
         return TextCatExample
+
+    def _create_prompt_example(self, example: Example) -> TextCatExample:
+        """Create a textcat prompt example from a spaCy example."""
+        if self._use_binary:
+            answer = (
+                "POS"
+                if example.reference.cats[list(self._label_dict.values())[0]] == 1.0
+                else "NEG"
+            )
+        else:
+            answer = ",".join(
+                [
+                    label
+                    for label, score in example.reference.cats.items()
+                    if score == 1.0
+                ]
+            )
+
+        textcat_example = TextCatExample(
+            text=example.reference.text,
+            answer=answer,
+        )
+        return textcat_example
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/util/parsing.py` & `spacy-llm-0.4.0/spacy_llm/tasks/util/parsing.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/util/serialization.py` & `spacy-llm-0.4.0/spacy_llm/tasks/util/serialization.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import abc
 from pathlib import Path
-from typing import Any, Dict, Generic, List, Optional, Tuple, Type, TypeVar, cast
+from typing import Any, Dict, Generic, List, Tuple, Type, TypeVar, cast
 
 import srsly
 from pydantic import BaseModel
 from spacy import util
 
 ExampleType = TypeVar("ExampleType", bound=BaseModel)
 
 
 class SerializableTask(abc.ABC, Generic[ExampleType]):
     """A task that can be serialized and deserialized."""
 
-    _examples: Optional[List[ExampleType]]
+    _prompt_examples: List[ExampleType]
 
     @property
     @abc.abstractmethod
     def _cfg_keys(self) -> List[str]:
         """A list of configuration attributes to serialize."""
         pass
 
@@ -35,43 +35,40 @@
         """Deserialize the task's configuration attributes.
 
         cfg (Dict[str, Any]): dictionary containing configuration attributes.
         """
         for key, value in cfg.items():
             setattr(self, key, value)
 
-    def get_examples(self) -> Optional[List[Dict[str, Any]]]:
+    def _get_prompt_examples(self) -> List[Dict[str, Any]]:
         """Serialize examples."""
-        if self._examples is not None:
-            examples = [eg.dict() for eg in self._examples]
-            return examples
-        return None
+        examples = [eg.dict() for eg in self._prompt_examples]
+        return examples
 
-    def set_examples(self, examples: Optional[List[Dict[str, Any]]]) -> None:
+    def _set_prompt_examples(self, examples: List[Dict[str, Any]]) -> None:
         """Deserialize examples from bytes.
 
-        examples (Optional[List[Dict[str, Any]]]): serialized examples.
+        examples (List[Dict[str, Any]]): serialized examples.
         """
-        if examples is not None:
-            self._examples = [self._Example.parse_obj(eg) for eg in examples]
+        self._prompt_examples = [self._Example.parse_obj(eg) for eg in examples]
 
     def to_bytes(
         self,
         *,
         exclude: Tuple[str] = cast(Tuple[str], tuple()),
     ) -> bytes:
         """Serialize the LLMWrapper to a bytestring.
 
         exclude (Tuple): Names of properties to exclude from serialization.
         RETURNS (bytes): The serialized object.
         """
 
         serialize = {
             "cfg": lambda: srsly.json_dumps(self.get_cfg()),
-            "examples": lambda: srsly.msgpack_dumps(self.get_examples()),
+            "prompt_examples": lambda: srsly.msgpack_dumps(self._get_prompt_examples()),
         }
 
         return util.to_bytes(serialize, exclude)
 
     def from_bytes(
         self,
         bytes_data: bytes,
@@ -83,15 +80,17 @@
         bytes_data (bytes): The data to load.
         exclude (Tuple[str]): Names of properties to exclude from deserialization.
         RETURNS (SpanTask): Modified SpanTask instance.
         """
 
         deserialize = {
             "cfg": lambda b: self.set_cfg(srsly.json_loads(b)),
-            "examples": lambda b: self.set_examples(srsly.msgpack_loads(b)),
+            "prompt_examples": lambda b: self._set_prompt_examples(
+                srsly.msgpack_loads(b)
+            ),
         }
 
         util.from_bytes(bytes_data, deserialize, exclude)
         return self
 
     def to_disk(
         self,
@@ -103,15 +102,17 @@
 
         path (Path): A path (currently unused).
         exclude (Tuple): Names of properties to exclude from serialization.
         """
 
         serialize = {
             "cfg": lambda p: srsly.write_json(p, self.get_cfg()),
-            "examples": lambda p: srsly.write_msgpack(p, self.get_examples()),
+            "prompt_examples": lambda p: srsly.write_msgpack(
+                p, self._get_prompt_examples()
+            ),
         }
 
         util.to_disk(path, serialize, exclude)
 
     def from_disk(
         self,
         path: Path,
@@ -122,12 +123,14 @@
 
         path (Path): A path (currently unused).
         exclude (Tuple): Names of properties to exclude from serialization.
         """
 
         deserialize = {
             "cfg": lambda p: self.set_cfg(srsly.read_json(p)),
-            "examples": lambda p: self.set_examples(srsly.read_msgpack(p)),
+            "prompt_examples": lambda p: self._set_prompt_examples(
+                srsly.read_msgpack(p)
+            ),
         }
 
         util.from_disk(path, deserialize, exclude)
         return self
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tasks/util/span.py` & `spacy-llm-0.4.0/spacy_llm/tasks/span.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,112 @@
+import warnings
 from typing import Callable, Dict, Iterable, List, Optional, Tuple, Type
 
 import jinja2
+from pydantic import BaseModel
 from spacy.tokens import Doc, Span
 
-from ...compat import Literal
-from ...registry import lowercase_normalizer
-from .examples import SpanExample
-from .parsing import find_substrings
-from .serialization import SerializableTask
+from ..compat import Literal
+from ..registry import lowercase_normalizer
+from .util.parsing import find_substrings
+from .util.serialization import SerializableTask
+
+
+class SpanExample(BaseModel):
+    text: str
+    entities: Dict[str, List[str]]
 
 
 class SpanTask(SerializableTask[SpanExample]):
     """Base class for Span-related tasks, eg NER and SpanCat."""
 
     def __init__(
         self,
         labels: List[str],
         template: str,
         label_definitions: Optional[Dict[str, str]] = {},
-        examples: Optional[List[SpanExample]] = None,
+        prompt_examples: Optional[List[SpanExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
         alignment_mode: Literal[
             "strict", "contract", "expand"  # noqa: F821
         ] = "contract",
         case_sensitive_matching: bool = False,
         single_match: bool = False,
     ):
         self._normalizer = normalizer if normalizer else lowercase_normalizer()
-        self._label_dict = {self._normalizer(label): label for label in labels}
+        self._label_dict = {
+            self._normalizer(label): label for label in sorted(set(labels))
+        }
         self._template = template
         self._label_definitions = label_definitions
-        self._examples = examples
+        self._prompt_examples = prompt_examples or []
         self._validate_alignment(alignment_mode)
         self._alignment_mode = alignment_mode
         self._case_sensitive_matching = case_sensitive_matching
         self._single_match = single_match
 
+        if self._prompt_examples:
+            self._prompt_examples = self._check_label_consistency()
+
+    def _check_label_consistency(self) -> List[SpanExample]:
+        """Checks consistency of labels between examples and defined labels. Emits warning on inconsistency.
+        RETURNS (List[SpanExample]): List of SpanExamples with valid labels.
+        """
+        assert self._prompt_examples
+        example_labels = {
+            self._normalizer(key): key
+            for example in self._prompt_examples
+            for key in example.entities
+        }
+        unspecified_labels = {
+            example_labels[key]
+            for key in (set(example_labels.keys()) - set(self._label_dict.keys()))
+        }
+        if not set(example_labels.keys()) <= set(self._label_dict.keys()):
+            warnings.warn(
+                f"Examples contain labels that are not specified in the task configuration. The latter contains the "
+                f"following labels: {sorted(list(set(self._label_dict.values())))}. Labels in examples missing from "
+                f"the task configuration: {sorted(list(unspecified_labels))}. Please ensure your label specification "
+                f"and example labels are consistent."
+            )
+
+        # Return examples without non-declared labels. If an example only has undeclared labels, it is discarded.
+        return [
+            example
+            for example in [
+                SpanExample(
+                    text=example.text,
+                    entities={
+                        label: entities
+                        for label, entities in example.entities.items()
+                        if self._normalizer(label) in self._label_dict
+                    },
+                )
+                for example in self._prompt_examples
+            ]
+            if len(example.entities)
+        ]
+
     @property
     def labels(self) -> Tuple[str, ...]:
         return tuple(self._label_dict.values())
 
+    @property
+    def prompt_template(self) -> str:
+        return self._template
+
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=doc.text,
                 labels=list(self._label_dict.values()),
                 label_definitions=self._label_definitions,
-                examples=self._examples,
+                examples=self._prompt_examples,
             )
             yield prompt
 
     def _format_response(self, response: str) -> Iterable[Tuple[str, Iterable[str]]]:
         """Parse raw string response into a structured format"""
         output = []
         assert self._normalizer is not None
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/backends/test_anthropic.py` & `spacy-llm-0.4.0/spacy_llm/tests/models/test_anthropic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 # mypy: ignore-errors
+import re
+
 import pytest
-from spacy_llm.backends.rest.anthropic import AnthropicBackend
+
+from spacy_llm.models.rest.anthropic import Anthropic, Endpoints
 
 from ..compat import has_anthropic_key
 
 
+@pytest.mark.external
 @pytest.mark.skipif(has_anthropic_key is False, reason="Anthropic API key unavailable")
 def test_anthropic_api_response_is_correct():
     """Check if we're getting the expected response and we're parsing it properly"""
-    anthropic = AnthropicBackend(
-        config={"model": "claude-instant-1", "max_tokens_to_sample": 10},
+    anthropic = Anthropic(
+        name="claude-instant-1",
+        endpoint=Endpoints.COMPLETIONS.value,
+        config={"max_tokens_to_sample": 10},
         strict=False,
         max_tries=10,
         interval=5.0,
         max_request_time=20,
     )
 
     prompt = "Count the number of characters in this string: hello"
     num_prompts = 3
     responses = anthropic(prompts=[prompt] * num_prompts)
     for response in responses:
         assert isinstance(response, str)
 
 
+@pytest.mark.external
 @pytest.mark.skipif(has_anthropic_key is False, reason="Anthropic API key unavailable")
 def test_anthropic_api_response_when_error():
     """Check if error message shows up properly given incorrect config"""
     # Incorrect config c.f. https://console.anthropic.com/docs/api/reference
     incorrect_temperature = "one"  # should be an int
-    anthropic = AnthropicBackend(
+    anthropic = Anthropic(
+        name="claude-instant-1",
+        endpoint=Endpoints.COMPLETIONS.value,
         config={
-            "model": "claude-instant-1",
             "max_tokens_to_sample": 10,
             "temperature": incorrect_temperature,
         },
         strict=False,
         max_tries=10,
         interval=5.0,
         max_request_time=20,
@@ -43,20 +51,24 @@
     prompt = "Count the number of characters in this string: hello"
     with pytest.raises(ValueError) as err:
         anthropic(prompts=[prompt])
     assert "invalid_request_error" in str(err.value)
     assert "temperature: value is not a valid float" in str(err.value)
 
 
+@pytest.mark.external
 @pytest.mark.skipif(has_anthropic_key is False, reason="Anthropic API key unavailable")
 def test_anthropic_error_unsupported_model():
     """Ensure graceful handling of error when model is not supported"""
     incorrect_model = "x-gpt-3.5-turbo"
-    with pytest.raises(ValueError) as err:
-        AnthropicBackend(
-            config={"model": incorrect_model, "max_tokens_to_sample": 10},
+    with pytest.raises(
+        ValueError, match=re.escape("Model 'x-gpt-3.5-turbo' is not supported")
+    ):
+        Anthropic(
+            name=incorrect_model,
+            endpoint=Endpoints.COMPLETIONS.value,
+            config={"max_tokens_to_sample": 10},
             strict=False,
             max_tries=10,
             interval=5.0,
             max_request_time=20,
         )
-    assert "The specified model 'x-gpt-3.5-turbo' is not supported" in str(err.value)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/backends/test_cohere.py` & `spacy-llm-0.4.0/spacy_llm/tests/models/test_cohere.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 # mypy: ignore-errors
 import pytest
-from spacy_llm.backends.rest.cohere import CohereBackend
+
+from spacy_llm.models.rest.cohere import Cohere, Endpoints
 
 from ..compat import has_cohere_key
 
 
 @pytest.mark.skipif(has_cohere_key is False, reason="Cohere API key not available")
 def test_cohere_api_response_is_correct():
     """Check if we're getting the response from the correct structure"""
-    cohere = CohereBackend(
-        config={"model": "command"},
+    cohere = Cohere(
+        name="command",
+        endpoint=Endpoints.COMPLETION.value,
+        config={},
         strict=False,
         max_tries=10,
         interval=5.0,
         max_request_time=20,
     )
     prompt = "Count the number of characters in this string: hello"
     num_prompts = 3  # arbitrary number to check multiple inputs
     responses = cohere(prompts=[prompt] * num_prompts)
     for response in responses:
         assert isinstance(response, str)
 
 
 @pytest.mark.skipif(has_cohere_key is False, reason="Cohere API key not available")
 def test_cohere_api_response_n_generations():
-    """Test how the backend handles more than 1 generation of output
+    """Test how the model handles more than 1 generation of output
 
     Users can configure Cohere to return more than 1 output for a single prompt
-    The current backend doesn't support that and the implementation only returns
+    The current model doesn't support that and the implementation only returns
     the very first output.
     """
     num_generations = 3
-    cohere = CohereBackend(
-        config={"model": "command", "num_generations": num_generations},
+    cohere = Cohere(
+        name="command",
+        endpoint=Endpoints.COMPLETION.value,
+        config={"num_generations": num_generations},
         strict=False,
         max_tries=10,
         interval=5.0,
         max_request_time=20,
     )
 
     prompt = "Count the number of characters in this string: hello"
@@ -44,20 +49,22 @@
     responses = cohere(prompts=[prompt] * num_prompts)
     for response in responses:
         assert isinstance(response, str)
 
 
 @pytest.mark.skipif(has_cohere_key is False, reason="Cohere API key not available")
 def test_cohere_api_response_when_error():
-    """Ensure graceful handling of error in the Cohere backend"""
+    """Ensure graceful handling of error in the Cohere model"""
     # Incorrect config because temperature is in incorrect range [0, 5]
     # c.f. https://docs.cohere.com/reference/generate
     incorrect_temperature = 1000  # must be between 0 and 5
-    cohere = CohereBackend(
-        config={"model": "command", "temperature": incorrect_temperature},
+    cohere = Cohere(
+        name="command",
+        endpoint=Endpoints.COMPLETION.value,
+        config={"temperature": incorrect_temperature},
         strict=False,
         max_tries=10,
         interval=5.0,
         max_request_time=20,
     )
     prompt = "Count the number of characters in this string: hello"
     num_prompts = 3  # arbitrary number to check multiple inputs
@@ -65,16 +72,17 @@
         cohere(prompts=[prompt] * num_prompts)
 
 
 @pytest.mark.skipif(has_cohere_key is False, reason="Cohere API key not available")
 def test_cohere_error_unsupported_model():
     """Ensure graceful handling of error when model is not supported"""
     incorrect_model = "x-gpt-3.5-turbo"
-    with pytest.raises(ValueError) as err:
-        CohereBackend(
-            config={"model": incorrect_model},
+    with pytest.raises(ValueError, match="Model 'x-gpt-3.5-turbo' is not supported"):
+        Cohere(
+            name=incorrect_model,
+            config={},
+            endpoint=Endpoints.COMPLETION.value,
             strict=False,
             max_tries=10,
             interval=5.0,
             max_request_time=20,
         )
-    assert "The specified model 'x-gpt-3.5-turbo' is not supported" in str(err.value)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/backends/test_openllama.py` & `spacy-llm-0.4.0/spacy_llm/tests/models/test_dolly.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,66 +2,60 @@
 
 import pytest
 import spacy
 from confection import Config  # type: ignore[import]
 from thinc.compat import has_torch_cuda_gpu
 
 _PIPE_CFG = {
-    "backend": {
-        "@llm_backends": "spacy.OpenLLaMa_HF.v1",
-        "model": "openlm-research/open_llama_3b_350bt_preview",
+    "model": {
+        "@llm_models": "spacy.Dolly.v1",
+        "name": "dolly-v2-3b",
     },
     "task": {"@llm_tasks": "spacy.NoOp.v1"},
 }
 
 _NLP_CONFIG = """
+
 [nlp]
 lang = "en"
 pipeline = ["llm"]
 batch_size = 128
 
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
 
-[components.llm.backend]
-@llm_backends = spacy.OpenLLaMa_HF.v1
-model = "openlm-research/open_llama_3b_350bt_preview"
+[components.llm.model]
+@llm_models = "spacy.Dolly.v1"
+name = "dolly-v2-3b"
 """
 
 
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init():
     """Test initialization and simple run."""
     nlp = spacy.blank("en")
-    nlp.add_pipe("llm", config=_PIPE_CFG)
-    nlp("This is a test.")
-
-
-@pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
-def test_init_with_set_config():
-    """Test initialization and simple run with changed config."""
-    nlp = spacy.blank("en")
     cfg = copy.deepcopy(_PIPE_CFG)
-    cfg["backend"]["config_run"] = {"max_new_tokens": 32}
+    cfg["model"]["@llm_models"] = "spacy.Dolly.v1"
     nlp.add_pipe("llm", config=cfg)
     nlp("This is a test.")
+    nlp.get_pipe("llm")._model.get_model_names()
 
 
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init_from_config():
     orig_config = Config().from_str(_NLP_CONFIG)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
 
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_invalid_model():
     orig_config = Config().from_str(_NLP_CONFIG)
     config = copy.deepcopy(orig_config)
-    config["components"]["llm"]["backend"]["model"] = "anything-else"
-    with pytest.raises(ValueError, match="is not supported"):
+    config["components"]["llm"]["model"]["name"] = "dolly-the-sheep"
+    with pytest.raises(ValueError, match="unexpected value; permitted"):
         spacy.util.load_model_from_config(config, auto_fill=True)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/backends/test_rest.py` & `spacy-llm-0.4.0/spacy_llm/tests/models/test_rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,83 +7,86 @@
 import spacy
 from spacy.tokens import Doc
 
 from ...registry import registry
 from ..compat import has_openai_key
 
 PIPE_CFG = {
-    "backend": {
-        "@llm_backends": "spacy.REST.v1",
-        "api": "OpenAI",
-        "config": {"temperature": 0.3, "model": "gpt-3.5-turbo"},
+    "model": {
+        "@llm_models": "spacy.GPT-3-5.v1",
+        "config": {"temperature": 0.3},
     },
     "task": {"@llm_tasks": "spacy.TextCat.v1", "labels": "POSITIVE,NEGATIVE"},
 }
 
 
 @registry.llm_tasks("spacy.Count.v1")
 class _CountTask:
+    _PROMPT_TEMPLATE = "Count the number of characters in this string: '{text}'."
+
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         for doc in docs:
-            yield f"Count the number of characters in this string: '{doc.text}'."
+            yield _CountTask._PROMPT_TEMPLATE.format(text=doc.text)
 
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[str]
     ) -> Iterable[Doc]:
         return docs
 
+    @property
+    def prompt_template(self) -> str:
+        return _CountTask._PROMPT_TEMPLATE
+
 
 def test_initialization():
     """Test initialization and simple run"""
     nlp = spacy.blank("en")
     cfg = copy.deepcopy(PIPE_CFG)
-    cfg["backend"]["api"] = "NoOp"
-    cfg["backend"]["config"] = {"model": "NoOp"}
+    cfg["model"] = {"@llm_models": "spacy.NoOp.v1"}
     nlp.add_pipe("llm", config=cfg)
     nlp("This is a test.")
 
 
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.external
 def test_model_error_handling():
     """Test error handling for wrong model."""
     nlp = spacy.blank("en")
-    with pytest.raises(ValueError) as err:
+    with pytest.raises(ValueError, match="Could not find function 'spacy.gpt-3.5x.v1'"):
         nlp.add_pipe(
             "llm",
             config={
                 "task": {"@llm_tasks": "spacy.NoOp.v1"},
-                "backend": {"config": {"model": "x-gpt-3.5-turbo"}},
+                "model": {"@llm_models": "spacy.gpt-3.5x.v1"},
             },
         )
-    assert "The specified model 'x-gpt-3.5-turbo' is not available." in str(err.value)
 
 
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.external
 def test_doc_length_error_handling():
     """Test error handling for excessive doc length."""
     nlp = spacy.blank("en")
     nlp.add_pipe(
         "llm",
         config={
             # Not using the NoOp task is necessary here, as the NoOp task sends a fixed-size prompt.
             "task": {"@llm_tasks": "spacy.Count.v1"},
-            "backend": {"config": {"model": "ada"}},
+            "model": {"config": {"model": "ada"}},
         },
     )
     # Call with an overly long document to elicit error.
     with pytest.raises(
         ValueError,
         match=re.escape(
-            "Request to OpenAI API failed: This model's maximum context length is 2049 tokens, however you requested "
-            "2527 tokens (2511 in your prompt; 16 for the completion). Please reduce your prompt; or completion length."
+            "Request to OpenAI API failed: This model's maximum context length is 4097 tokens. However, your messages "
+            "resulted in 5018 tokens. Please reduce the length of the messages."
         ),
     ):
-        nlp("n" * 5000)
+        nlp("n" * 10000)
 
 
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.external
 def test_max_time_error_handling():
     """Test error handling for exceeding max. time."""
     nlp = spacy.blank("en")
@@ -91,15 +94,15 @@
         TimeoutError,
         match="Request time out. Check your network connection and the API's availability.",
     ):
         nlp.add_pipe(
             "llm",
             config={
                 "task": {"@llm_tasks": "spacy.Count.v1"},
-                "backend": {
+                "model": {
                     "config": {"model": "ada"},
                     "max_request_time": 0.001,
                     "max_tries": 1,
                     "interval": 0.001,
                 },
             },
         )
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/backends/test_stablelm.py` & `spacy-llm-0.4.0/spacy_llm/tests/models/test_falcon.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,74 +2,58 @@
 
 import pytest
 import spacy
 from confection import Config  # type: ignore[import]
 from thinc.compat import has_torch_cuda_gpu
 
 _PIPE_CFG = {
-    "backend": {
-        "@llm_backends": "spacy.StableLM_HF.v1",
-        "model": "stabilityai/stablelm-base-alpha-3b",
+    "model": {
+        "@llm_models": "spacy.Falcon.v1",
+        "name": "falcon-rw-1b",
     },
     "task": {"@llm_tasks": "spacy.NoOp.v1"},
 }
 
 _NLP_CONFIG = """
+
 [nlp]
 lang = "en"
 pipeline = ["llm"]
 batch_size = 128
 
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
 
-[components.llm.backend]
-@llm_backends = "spacy.StableLM_HF.v1"
-model = "stabilityai/stablelm-base-alpha-3b"
+[components.llm.model]
+@llm_models = "spacy.Falcon.v1"
+name = "falcon-rw-1b"
 """
 
 
-@pytest.mark.parametrize(
-    "model",
-    ("stabilityai/stablelm-base-alpha-3b", "stabilityai/stablelm-tuned-alpha-3b"),
-)
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
-def test_init(model: str):
-    """Test initialization and simple run.
-    model (str): Name of model to run.
-    """
+def test_init():
+    """Test initialization and simple run."""
     nlp = spacy.blank("en")
     cfg = copy.deepcopy(_PIPE_CFG)
-    cfg["backend"]["model"] = model
     nlp.add_pipe("llm", config=cfg)
     nlp("This is a test.")
 
 
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init_from_config():
     orig_config = Config().from_str(_NLP_CONFIG)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
 
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
-def test_init_with_set_config():
-    """Test initialization and simple run with changed config."""
-    nlp = spacy.blank("en")
-    cfg = copy.deepcopy(_PIPE_CFG)
-    cfg["backend"]["config_run"] = {"temperature": 0.3}
-    nlp.add_pipe("llm", config=cfg)
-    nlp("This is a test.")
-
-
-@pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_invalid_model():
     orig_config = Config().from_str(_NLP_CONFIG)
     config = copy.deepcopy(orig_config)
-    config["components"]["llm"]["backend"]["model"] = "anything-else"
-    with pytest.raises(ValueError, match="is not supported"):
+    config["components"]["llm"]["model"]["name"] = "x"
+    with pytest.raises(ValueError, match="unexpected value; permitted"):
         spacy.util.load_model_from_config(config, auto_fill=True)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/conftest.py` & `spacy-llm-0.4.0/spacy_llm/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 
     skip_external = pytest.mark.skip(reason="need --external option to run")
     for item in items:
         if "external" in item.keywords:
             item.add_marker(skip_external)
 
 
-@registry.llm_backends("test.NoOpBackend.v1")
+@registry.llm_models("test.NoOpModel.v1")
 def noop_factory(output: str = ""):
     def noop(prompts: Iterable[str]) -> Iterable[str]:
         return [output] * len(list(prompts))
 
     return noop
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/pipeline/test_llm.py` & `spacy-llm-0.4.0/spacy_llm/tests/pipeline/test_llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,43 @@
 import sys
 import warnings
 from pathlib import Path
 from typing import Any, Dict, Iterable
 
 import pytest
 import spacy
+import srsly
 from confection import Config
 from spacy.language import Language
 from spacy.tokens import Doc
+from spacy.util import make_tempdir
 from thinc.api import NumpyOps, get_current_ops
 
 import spacy_llm
-from spacy_llm.backends.rest.noop import _NOOP_RESPONSE
+from spacy_llm.models.rest.noop import _NOOP_RESPONSE
 from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.registry import registry
 from spacy_llm.tasks import make_noop_task
 from spacy_llm.tasks.noop import _NOOP_PROMPT
 
 from ...cache import BatchCache
+from ...registry.reader import fewshot_reader
 from ...util import assemble_from_config
 from ..compat import has_openai_key
 
 
 @pytest.fixture
 def noop_config() -> Dict[str, Any]:
     """Returns NoOp config.
     RETURNS (Dict[str, Any]): NoOp config.
     """
     return {
         "save_io": True,
         "task": {"@llm_tasks": "spacy.NoOp.v1"},
-        "backend": {"api": "NoOp", "config": {"model": "NoOp"}},
+        "model": {"@llm_models": "spacy.NoOp.v1"},
     }
 
 
 @pytest.fixture
 def nlp(noop_config) -> Language:
     nlp = spacy.blank("en")
     nlp.add_pipe("llm", config=noop_config)
@@ -72,15 +75,15 @@
     if not isinstance(ops, NumpyOps) and n_process != 1:
         pytest.skip("Only test multiple processes on CPU")
 
     path = tmp_path / "cache"
 
     config = {
         "task": {"@llm_tasks": "spacy.NoOp.v1"},
-        "backend": {"api": "NoOp", "config": {"model": "NoOp"}},
+        "model": {"@llm_models": "spacy.NoOp.v1"},
         "cache": {
             "path": str(path),
             "batch_size": 1,  # Eager caching
             "max_batches_in_mem": 10,
         },
     }
 
@@ -109,26 +112,26 @@
     assert list(nlp.pipe(texts=[])) == []
 
 
 def test_llm_serialize_bytes():
     llm = LLMWrapper(
         task=make_noop_task(),
         save_io=False,
-        backend=None,  # type: ignore
+        model=None,  # type: ignore
         cache=BatchCache(path=None, batch_size=0, max_batches_in_mem=0),
         vocab=None,  # type: ignore
     )
     llm.from_bytes(llm.to_bytes())
 
 
 def test_llm_serialize_disk():
     llm = LLMWrapper(
         task=make_noop_task(),
         save_io=False,
-        backend=None,  # type: ignore
+        model=None,  # type: ignore
         cache=BatchCache(path=None, batch_size=0, max_batches_in_mem=0),
         vocab=None,  # type: ignore
     )
 
     with spacy.util.make_tempdir() as tmp_dir:
         llm.to_disk(tmp_dir / "llm")
         llm.from_disk(tmp_dir / "llm")
@@ -165,19 +168,19 @@
     with pytest.warns(UserWarning) as record:
         noop_config["task"] = {"@llm_tasks": "IncorrectTypes.v1"}
         nlp.add_pipe("llm", config=noop_config)
     assert len(record) == 2
     assert (
         str(record[0].message)
         == "Type returned from `task.generate_prompts()` (`typing.Iterable[int]`) doesn't match type "
-        "expected by `backend` (`typing.Iterable[str]`)."
+        "expected by `model` (`typing.Iterable[str]`)."
     )
     assert (
         str(record[1].message)
-        == "Type returned from `backend` (`typing.Iterable[str]`) doesn't match type "
+        == "Type returned from `model` (`typing.Iterable[str]`) doesn't match type "
         "expected by `task.parse_responses()` (`typing.Iterable[float]`)."
     )
 
     # Run with disabled type consistency validation.
     nlp = spacy.blank("en")
     noop_config["validate_types"] = False
     nlp.add_pipe("llm", config=noop_config)
@@ -207,16 +210,15 @@
 
     assert f"Generated prompt for doc: {doc.text}" in caplog.text
     assert "Don't do anything" in caplog.text
     assert f"LLM response for doc: {doc.text}" in caplog.text
 
 
 def test_llm_logs_default_null_handler(nlp: Language, capsys: pytest.CaptureFixture):
-
-    doc = nlp("This is a test")
+    nlp("This is a test")
 
     captured = capsys.readouterr()
     assert captured.out == ""
     assert captured.err == ""
 
     # Add a basic Stream Handler
     stream_handler = logging.StreamHandler(sys.stdout)
@@ -235,14 +237,32 @@
     doc = nlp("This is a test with no handler")
     captured = capsys.readouterr()
     assert f"Generated prompt for doc: {doc.text}" not in captured.out
     assert "Don't do anything" not in captured.out
     assert f"LLM response for doc: {doc.text}" not in captured.out
 
 
+def test_fewshot_reader_file_format_handling():
+    """Test if fewshot reader copes with file formats as expected."""
+    example = [
+        {
+            "text": "Circe lived on Aeaea.",
+            "entities": {"PER": ["Circe"], "LOC": ["Aeaea"]},
+        }
+    ]
+    with make_tempdir() as tmpdir:
+        srsly.write_yaml(tmpdir / "example.yml", example)
+        srsly.write_yaml(tmpdir / "example.json", example)
+        srsly.write_yaml(tmpdir / "example.foo", example)
+
+        fewshot_reader(tmpdir / "example.yml")
+        fewshot_reader(tmpdir / "example.json")
+        fewshot_reader(tmpdir / "example.foo")
+
+
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 def test_pipe_labels():
     """Test pipe labels with serde."""
 
     cfg_string = """
     [nlp]
@@ -254,18 +274,17 @@
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
     @llm_tasks = "spacy.TextCat.v2"
     labels = ["COMPLIMENT", "INSULT"]
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
+    config = {"temperature": 0.3}
     """
 
     config = Config().from_str(cfg_string)
     nlp = assemble_from_config(config)
 
     with spacy.util.make_tempdir() as tmpdir:
         nlp.to_disk(tmpdir / "tst.nlp")
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.json` & `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.jsonl` & `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.yml` & `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/rel_examples.jsonl` & `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/rel.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_lemma.py` & `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_sentiment.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 import spacy
 from confection import Config
 from spacy.util import make_tempdir
 
 from spacy_llm.registry import fewshot_reader, file_reader
 
-from ...tasks import make_lemma_task
+from ...tasks import make_sentiment_task
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 TEMPLATES_DIR = Path(__file__).parent / "templates"
 
 
 @pytest.fixture
@@ -24,19 +24,18 @@
 
     [components]
 
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
-    @llm_tasks = "spacy.Lemma.v1"
+    @llm_tasks = "spacy.Sentiment.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     config = {"temperature": 0}
     """
 
 
 @pytest.fixture
 def fewshot_cfg_string():
     return f"""
@@ -47,23 +46,22 @@
 
     [components]
 
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
-    @llm_tasks = "spacy.Lemma.v1"
+    @llm_tasks = "spacy.Sentiment.v1"
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
-    path = {str((Path(__file__).parent / "examples" / "lemma_examples.yml"))}
+    path = {str((Path(__file__).parent / "examples" / "sentiment.yml"))}
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     config = {{"temperature": 0}}
     """
 
 
 @pytest.fixture
 def ext_template_cfg_string():
     """Simple zero-shot config with an external template"""
@@ -75,38 +73,37 @@
     batch_size = 128
 
     [components]
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
-    @llm_tasks = "spacy.Lemma.v1"
+    @llm_tasks = "spacy.Sentiment.v1"
 
     [components.llm.task.template]
     @misc = "spacy.FileReader.v1"
-    path = {str((Path(__file__).parent / "templates" / "lemma_template.jinja2"))}
+    path = {str((Path(__file__).parent / "templates" / "sentiment.jinja2"))}
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {{}}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
+    config = {{"temperature": 0}}
     """
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize(
     "cfg_string",
     [
         "zeroshot_cfg_string",
         "fewshot_cfg_string",
         "ext_template_cfg_string",
     ],
 )
-def test_lemma_config(cfg_string, request):
+def test_sentiment_config(cfg_string, request):
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
     # also test nlp config from a dict in add_pipe
     component_cfg = dict(orig_config["components"]["llm"])
@@ -123,197 +120,149 @@
     "cfg_string",
     [
         "zeroshot_cfg_string",
         "fewshot_cfg_string",
         "ext_template_cfg_string",
     ],
 )
-def test_lemma_predict(cfg_string, request):
-    """Use OpenAI to get zero-shot LEMMA results.
+def test_sentiment_predict(cfg_string, request):
+    """Use OpenAI to get zero-shot sentiment results.
     Note that this test may fail randomly, as the LLM's output is unguaranteed to be consistent/predictable
     """
     cfg = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
-    lemmas = [str(token.lemma_) for token in nlp("I've watered the plants.")]
-    # Compare lemmas for correctness, if we are not using the external dummy template.
     if cfg_string != "ext_template_cfg_string":
-        assert lemmas == ["I", "have", "water", "the", "plant", "."]
+        assert nlp("This is horrible.")._.sentiment == 0
+        assert 0 < nlp("This is meh.")._.sentiment <= 0.5
+        assert nlp("This is perfect.")._.sentiment == 1
 
 
 @pytest.mark.external
+@pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize(
-    "cfg_string",
+    "cfg_string_field",
     [
-        "zeroshot_cfg_string",
-        "fewshot_cfg_string",
+        ("zeroshot_cfg_string", None),
+        ("fewshot_cfg_string", None),
+        ("zeroshot_cfg_string", "sentiment_x"),
     ],
 )
-def test_lemma_io(cfg_string, request):
+def test_lemma_io(cfg_string_field, request):
+    cfg_string, field = cfg_string_field
     cfg = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg)
+    if field:
+        orig_config["components"]["llm"]["task"]["field"] = field
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
     # ensure you can save a pipeline to disk and run it after loading
     with make_tempdir() as tmpdir:
         nlp.to_disk(tmpdir)
         nlp2 = spacy.load(tmpdir)
     assert nlp2.pipe_names == ["llm"]
-    lemmas = [str(token.lemma_) for token in nlp2("I've watered the plants.")]
+    score = getattr(nlp2("This is perfect.")._, field if field else "sentiment")
     if cfg_string != "ext_template_cfg_string":
-        assert lemmas == ["I", "have", "water", "the", "plant", "."]
+        assert score == 1
 
 
 def test_jinja_template_rendering_without_examples():
     """Test if jinja template renders as we expected
 
     We apply the .strip() method for each prompt so that we don't have to deal
     with annoying newlines and spaces at the edge of the text.
     """
     nlp = spacy.blank("xx")
-    text = "Alice and Bob went to the supermarket"
+    text = "They're indifferent."
     doc = nlp.make_doc(text)
 
-    lemma_task = make_lemma_task(examples=None)
-    prompt = list(lemma_task.generate_prompts([doc]))[0]
+    sentiment_task = make_sentiment_task(examples=None)
+    prompt = list(sentiment_task.generate_prompts([doc]))[0]
 
     assert (
         prompt.strip()
         == f"""
-You are an expert lemmatization system. Your task is to accept Text as input and identify the lemma for every token in the Text.
-Consider that contractions represent multiple words. Each word in a contraction should be annotated with its lemma separately.
-Output each original word on a new line, followed by a colon and the word's lemma - like this:
-'''
-Word1: Lemma of Word1
-Word2: Lemma of Word2
-'''
-Include the final punctuation token in this list.
-Prefix with your output with "Lemmatized text".
-
+Analyse whether the text surrounded by ''' is positive or negative. Respond with a float value between 0 and 1. 1 represents an exclusively positive sentiment, 0 an exclusively negative sentiment.
 
-Here is the text that needs to be lemmatized:
+Text:
 '''
 {text}
 '''
-""".strip()
+Answer:""".strip()
     )
 
 
 @pytest.mark.parametrize(
     "examples_path",
     [
-        str(EXAMPLES_DIR / "lemma_examples.json"),
-        str(EXAMPLES_DIR / "lemma_examples.yml"),
-        str(EXAMPLES_DIR / "lemma_examples.jsonl"),
+        str(EXAMPLES_DIR / "sentiment.json"),
+        str(EXAMPLES_DIR / "sentiment.yml"),
+        str(EXAMPLES_DIR / "sentiment.jsonl"),
     ],
 )
 def test_jinja_template_rendering_with_examples(examples_path):
     """Test if jinja2 template renders as expected
 
     We apply the .strip() method for each prompt so that we don't have to deal
     with annoying newlines and spaces at the edge of the text.
     """
     nlp = spacy.blank("xx")
-    text = "Alice and Bob went to the supermarket."
+    text = "It was the happiest day of her life."
     doc = nlp.make_doc(text)
 
-    lemma_task = make_lemma_task(examples=fewshot_reader(examples_path))
-    prompt = list(lemma_task.generate_prompts([doc]))[0]
+    sentiment_task = make_sentiment_task(examples=fewshot_reader(examples_path))
+    prompt = list(sentiment_task.generate_prompts([doc]))[0]
 
     assert (
         prompt.strip()
-        == f"""
-You are an expert lemmatization system. Your task is to accept Text as input and identify the lemma for every token in the Text.
-Consider that contractions represent multiple words. Each word in a contraction should be annotated with its lemma separately.
-Output each original word on a new line, followed by a colon and the word's lemma - like this:
-'''
-Word1: Lemma of Word1
-Word2: Lemma of Word2
-'''
-Include the final punctuation token in this list.
-Prefix with your output with "Lemmatized text".
-
+        == """
+Analyse whether the text surrounded by ''' is positive or negative. Respond with a float value between 0 and 1. 1 represents an exclusively positive sentiment, 0 an exclusively negative sentiment.
 Below are some examples (only use these as a guide):
 
 Text:
 '''
-The arc of the moral universe is long, but it bends toward justice.
-'''
-Lemmas:
-'''
-The: The
-arc: arc
-of: of
-the: the
-moral: moral
-universe: universe
-is: be
-long: long
-,: ,
-but: but
-it: it
-bends: bend
-toward: toward
-justice: justice
-.: .
+This is horrifying.
 '''
+Answer: 0.0
 
 Text:
 '''
-Life can only be understood backwards; but it must be lived forwards.
-'''
-Lemmas:
-'''
-Life: Life
-can: can
-only: only
-be: be
-understood: understand
-backwards: backwards
-;: ;
-but: but
-it: it
-must: must
-be: be
-lived: lived
-forwards: forwards
-.: .
+This is underwhelming.
 '''
+Answer: 0.25
 
 Text:
 '''
-I'm buying ice cream.
+This is ok.
 '''
-Lemmas:
+Answer: 0.5
+
+Text:
 '''
-I: I
-'m: be
-buying: buy
-ice: ice
-cream: cream
-.: .
+I'm looking forward to this!
 '''
+Answer: 1.0
 
-Here is the text that needs to be lemmatized:
+Text:
 '''
-{text}
+It was the happiest day of her life.
 '''
-""".strip()
+Answer:""".strip()
     )
 
 
 def test_external_template_actually_loads():
-    template_path = str(TEMPLATES_DIR / "lemma_template.jinja2")
+    template_path = str(TEMPLATES_DIR / "sentiment.jinja2")
     template = file_reader(template_path)
-    text = "Alice and Bob went to the supermarket"
+    text = "There is a silver lining."
     nlp = spacy.blank("xx")
     doc = nlp.make_doc(text)
 
-    lemma_task = make_lemma_task(template=template)
-    prompt = list(lemma_task.generate_prompts([doc]))[0]
+    sentiment_task = make_sentiment_task(template=template)
+    prompt = list(sentiment_task.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == f"""
-This is a test LEMMA template.
-Here is the text: {text}
+Text: {text}
+Sentiment:
 """.strip()
     )
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_ner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
+import re
 from pathlib import Path
 
 import pytest
 import spacy
 import srsly
 from confection import Config
-from pydantic import ValidationError
 from spacy.tokens import Span
 from spacy.training import Example
 from spacy.util import make_tempdir
 
 from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.registry import fewshot_reader, file_reader, lowercase_normalizer
 from spacy_llm.registry import strip_normalizer
@@ -40,18 +40,16 @@
     [components.llm.task]
     @llm_tasks = "spacy.NER.v1"
     labels = PER,ORG,LOC
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.fixture
 def zeroshot_cfg_string_v2_lds():
     return """
     [nlp]
@@ -72,18 +70,16 @@
     PER = "Any named individual in the text"
     ORG = "Any named organization in the text"
     LOC = "The name of any politically or geographically defined location"
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.fixture
 def fewshot_cfg_string():
     return f"""
     [nlp]
@@ -98,23 +94,21 @@
 
     [components.llm.task]
     @llm_tasks = "spacy.NER.v1"
     labels = PER,ORG,LOC
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
-    path = {str((Path(__file__).parent / "examples" / "ner_examples.yml"))}
+    path = {str((Path(__file__).parent / "examples" / "ner.yml"))}
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config: {{}}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.fixture
 def fewshot_cfg_string_v2():
     return f"""
     [nlp]
@@ -129,23 +123,21 @@
 
     [components.llm.task]
     @llm_tasks = "spacy.NER.v2"
     labels = ["PER", "ORG", "LOC"]
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
-    path = {str((Path(__file__).parent / "examples" / "ner_examples.yml"))}
+    path = {str((Path(__file__).parent / "examples" / "ner.yml"))}
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config: {{}}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.fixture
 def ext_template_cfg_string():
     """Simple zero-shot config with an external template"""
 
@@ -161,23 +153,21 @@
 
     [components.llm.task]
     @llm_tasks = "spacy.NER.v2"
     labels = PER,ORG,LOC
 
     [components.llm.task.template]
     @misc = "spacy.FileReader.v1"
-    path = {str((Path(__file__).parent / "templates" / "ner_template.jinja2"))}
+    path = {str((Path(__file__).parent / "templates" / "ner.jinja2"))}
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {{}}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize(
     "cfg_string",
@@ -207,15 +197,15 @@
     assert isinstance(pipe, LLMWrapper)
     assert isinstance(pipe.task, LLMTask)
 
     labels = orig_config["components"]["llm"]["task"]["labels"]
     labels = split_labels(labels)
     task = pipe.task
     assert isinstance(task, Labeled)
-    assert task.labels == tuple(labels)
+    assert sorted(task.labels) == sorted(tuple(labels))
     assert pipe.labels == task.labels
     assert nlp.pipe_labels["llm"] == list(task.labels)
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize(
@@ -228,22 +218,25 @@
         "ext_template_cfg_string",
     ],
 )
 def test_ner_predict(cfg_string, request):
     """Use OpenAI to get zero-shot NER results.
     Note that this test may fail randomly, as the LLM's output is unguaranteed to be consistent/predictable
     """
+    orig_cfg_string = cfg_string
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     text = "Marc and Bob both live in Ireland."
     doc = nlp(text)
-    assert len(doc.ents) > 0
-    for ent in doc.ents:
-        assert ent.label_ in ["PER", "ORG", "LOC"]
+
+    if orig_cfg_string != "ext_template_cfg_string":
+        assert len(doc.ents) > 0
+        for ent in doc.ents:
+            assert ent.label_ in ["PER", "ORG", "LOC"]
 
 
 @pytest.mark.external
 @pytest.mark.parametrize(
     "cfg_string",
     [
         "zeroshot_cfg_string",
@@ -515,17 +508,17 @@
 
     assert (
         prompt.strip()
         == """
 You are an expert Named Entity Recognition (NER) system. Your task is to accept Text as input and extract named entities for the set of predefined entity labels.
 From the Text input provided, extract named entities for each label in the following format:
 
-PER: <comma delimited list of strings>
-ORG: <comma delimited list of strings>
 LOC: <comma delimited list of strings>
+ORG: <comma delimited list of strings>
+PER: <comma delimited list of strings>
 
 
 Here is the text that needs labeling:
 
 Text:
 '''
 Alice and Bob went to the supermarket
@@ -533,17 +526,17 @@
 """.strip()
     )
 
 
 @pytest.mark.parametrize(
     "examples_path",
     [
-        str(EXAMPLES_DIR / "ner_examples.json"),
-        str(EXAMPLES_DIR / "ner_examples.yml"),
-        str(EXAMPLES_DIR / "ner_examples.jsonl"),
+        str(EXAMPLES_DIR / "ner.json"),
+        str(EXAMPLES_DIR / "ner.yml"),
+        str(EXAMPLES_DIR / "ner.jsonl"),
     ],
 )
 def test_jinja_template_rendering_with_examples(examples_path):
     """Test if jinja2 template renders as expected
 
     We apply the .strip() method for each prompt so that we don't have to deal
     with annoying newlines and spaces at the edge of the text.
@@ -558,17 +551,17 @@
 
     assert (
         prompt.strip()
         == """
 You are an expert Named Entity Recognition (NER) system. Your task is to accept Text as input and extract named entities for the set of predefined entity labels.
 From the Text input provided, extract named entities for each label in the following format:
 
-PER: <comma delimited list of strings>
-ORG: <comma delimited list of strings>
 LOC: <comma delimited list of strings>
+ORG: <comma delimited list of strings>
+PER: <comma delimited list of strings>
 
 
 Below are some examples (only use these as a guide):
 
 Text:
 '''
 Jack and Jill went up the hill.
@@ -622,17 +615,17 @@
 
     assert (
         prompt.strip()
         == """
 You are an expert Named Entity Recognition (NER) system. Your task is to accept Text as input and extract named entities for the set of predefined entity labels.
 From the Text input provided, extract named entities for each label in the following format:
 
-PER: <comma delimited list of strings>
-ORG: <comma delimited list of strings>
 LOC: <comma delimited list of strings>
+ORG: <comma delimited list of strings>
+PER: <comma delimited list of strings>
 
 Below are definitions of each label to help aid you in what kinds of named entities to extract for each label.
 Assume these definitions are written by an expert and follow them closely.
 
 PER: Person definition
 ORG: Organization definition
 LOC: Location definition
@@ -655,34 +648,34 @@
             "entities": [("PER", ("Entities")), ("ORG", ("dict", "list"))],
         }
     ]
     with make_tempdir() as tmpdir:
         tmp_path = tmpdir / "wrong_example.yml"
         srsly.write_yaml(tmp_path, wrong_example)
 
-        with pytest.raises(ValidationError):
+        with pytest.raises(ValueError):
             make_ner_task_v2(labels="PER,ORG,LOC", examples=fewshot_reader(tmp_path))
 
 
 def test_external_template_actually_loads():
-    template_path = str(TEMPLATES_DIR / "ner_template.jinja2")
+    template_path = str(TEMPLATES_DIR / "ner.jinja2")
     template = file_reader(template_path)
     labels = "PER,ORG,LOC"
     nlp = spacy.blank("xx")
     doc = nlp.make_doc("Alice and Bob went to the supermarket")
 
     llm_ner = make_ner_task_v2(labels=labels, template=template)
     prompt = list(llm_ner.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
 This is a test NER template. Here are the labels
-PER
-ORG
 LOC
+ORG
+PER
 
 Here is the text: Alice and Bob went to the supermarket
 """.strip()
     )
 
 
 @pytest.fixture
@@ -701,23 +694,22 @@
     [components.llm.task]
     @llm_tasks = "spacy.NER.v2"
     labels = PER,ORG,LOC
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "test.NoOpBackend.v1"
+    [components.llm.model]
+    @llm_models = "test.NoOpModel.v1"
     output = "PER: Alice,Bob"
     """
 
 
 @pytest.mark.parametrize("n_detections", [0, 1, 2])
 def test_ner_scoring(noop_config, n_detections):
-
     config = Config().from_str(noop_config)
     nlp = assemble_from_config(config)
 
     examples = []
 
     for text in ["Alice works with Bob.", "Bob lives with Alice."]:
         predicted = nlp.make_doc(text)
@@ -731,18 +723,19 @@
         examples.append(Example(predicted, reference))
 
     scores = nlp.evaluate(examples)
 
     assert scores["ents_p"] == n_detections / 2
 
 
-def test_ner_init(noop_config):
-
+@pytest.mark.parametrize("n_prompt_examples", [-1, 0, 1, 2])
+def test_ner_init(noop_config, n_prompt_examples: int):
     config = Config().from_str(noop_config)
     del config["components"]["llm"]["task"]["labels"]
+
     nlp = assemble_from_config(config)
 
     examples = []
 
     for text in [
         "Alice works with Bob in London.",
         "Bob lives with Alice in Manchester.",
@@ -758,20 +751,33 @@
 
         examples.append(Example(predicted, reference))
 
     _, llm = nlp.pipeline[0]
     task: NERTask = llm._task
 
     assert set(task._label_dict.values()) == set()
+    assert not task._prompt_examples
+
+    nlp.config["initialize"]["components"]["llm"] = {
+        "n_prompt_examples": n_prompt_examples
+    }
     nlp.initialize(lambda: examples)
+
     assert set(task._label_dict.values()) == {"PER", "LOC"}
+    if n_prompt_examples >= 0:
+        assert len(task._prompt_examples) == n_prompt_examples
+    else:
+        assert len(task._prompt_examples) == len(examples)
+
+    if n_prompt_examples > 0:
+        for eg in task._prompt_examples:
+            assert set(eg.entities.keys()) == {"PER", "LOC"}
 
 
 def test_ner_serde(noop_config):
-
     config = Config().from_str(noop_config)
     del config["components"]["llm"]["task"]["labels"]
 
     nlp1 = assemble_from_config(config)
     nlp2 = assemble_from_config(config)
 
     labels = {"loc": "LOC", "per": "PER"}
@@ -788,15 +794,14 @@
     b = nlp1.to_bytes()
     nlp2.from_bytes(b)
 
     assert task1._label_dict == task2._label_dict == labels
 
 
 def test_ner_to_disk(noop_config, tmp_path: Path):
-
     config = Config().from_str(noop_config)
     del config["components"]["llm"]["task"]["labels"]
 
     nlp1 = assemble_from_config(config)
     nlp2 = assemble_from_config(config)
 
     labels = {"loc": "LOC", "per": "PER"}
@@ -819,7 +824,59 @@
 
     cfg = json.loads(cfgs[0].read_text())
     assert cfg["_label_dict"] == labels
 
     nlp2.from_disk(path)
 
     assert task1._label_dict == task2._label_dict == labels
+
+
+def test_label_inconsistency():
+    """Test whether inconsistency between specified labels and labels in examples is detected."""
+    cfg = f"""
+    [nlp]
+    lang = "en"
+    pipeline = ["llm"]
+
+    [components]
+
+    [components.llm]
+    factory = "llm"
+
+    [components.llm.task]
+    @llm_tasks = "spacy.NER.v2"
+    labels = ["PERSON", "LOCATION"]
+
+    [components.llm.task.examples]
+    @misc = "spacy.FewShotReader.v1"
+    path = {str((Path(__file__).parent / "examples" / "ner_inconsistent.yml"))}
+
+    [components.llm.model]
+    @llm_models = "test.NoOpModel.v1"
+    """
+
+    config = Config().from_str(cfg)
+    with pytest.warns(
+        UserWarning,
+        match=re.escape(
+            "Examples contain labels that are not specified in the task configuration. The latter contains the "
+            "following labels: ['LOCATION', 'PERSON']. Labels in examples missing from the task configuration: "
+            "['TECH']. Please ensure your label specification and example labels are consistent."
+        ),
+    ):
+        nlp = assemble_from_config(config)
+
+    prompt_examples = nlp.get_pipe("llm")._task._prompt_examples
+    assert len(prompt_examples) == 2
+    assert prompt_examples[0].text == "Jack and Jill went up the hill."
+    assert prompt_examples[0].entities == {
+        "LOCATION": ["hill"],
+        "PERSON": ["Jack", "Jill"],
+    }
+    assert (
+        prompt_examples[1].text
+        == "Jack and Jill went up the hill and spaCy is a great tool."
+    )
+    assert prompt_examples[1].entities == {
+        "LOCATION": ["hill"],
+        "PERSON": ["Jack", "Jill"],
+    }
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_rel.py` & `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_rel.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,17 +33,16 @@
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
     @llm_tasks = "spacy.REL.v1"
     labels = "LivesIn,Visits"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
 
     [initialize]
     vectors = "en_core_web_md"
     """
 
 
 @pytest.fixture
@@ -64,19 +63,18 @@
 
     [components.llm.task]
     @llm_tasks = "spacy.REL.v1"
     labels = ["LivesIn", "Visits"]
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
-    path = {str(EXAMPLES_DIR / "rel_examples.jsonl")}
+    path = {str(EXAMPLES_DIR / "rel.jsonl")}
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
 
     [initialize]
     vectors = "en_core_web_md"
     """
 
 
 @pytest.fixture
@@ -95,16 +93,16 @@
     [components.llm.task]
     @llm_tasks = "spacy.REL.v1"
     labels = ["LivesIn", "Visits"]
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "test.NoOpBackend.v1"
+    [components.llm.model]
+    @llm_models = "test.NoOpModel.v1"
     """
 
 
 @pytest.fixture
 def task():
     text = "Joey rents a place in New York City."
     gold_relations = [RelationItem(dep=0, dest=1, relation="LivesIn")]
@@ -125,21 +123,21 @@
     assert isinstance(pipe.task, LLMTask)
 
     task = pipe.task
     labels = orig_config["components"]["llm"]["task"]["labels"]
     labels = split_labels(labels)
     assert isinstance(task, Labeled)
     assert task.labels == tuple(labels)
-    assert pipe.labels == task.labels
+    assert set(pipe.labels) == set(task.labels)
     assert nlp.pipe_labels["llm"] == list(task.labels)
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
-@pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
+@pytest.mark.parametrize("cfg_string", ["fewshot_cfg_string"])  # "zeroshot_cfg_string",
 def test_rel_predict(task, cfg_string, request):
     """Use OpenAI to get REL results.
     Note that this test may fail randomly, as the LLM's output is unguaranteed to be consistent/predictable
     """
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string)
     nlp = assemble_from_config(orig_config)
@@ -147,17 +145,17 @@
     text, _ = task
     doc = nlp(text)
 
     assert doc.ents
     assert doc._.rel
 
 
-def test_rel_init(noop_config):
-
-    RELTask._check_rel_extention()
+@pytest.mark.parametrize("n_prompt_examples", [-1, 0, 1, 2])
+def test_rel_init(noop_config, n_prompt_examples: int):
+    RELTask._check_rel_extension()
 
     config = Config().from_str(noop_config)
     del config["components"]["llm"]["task"]["labels"]
     nlp = assemble_from_config(config)
 
     examples = []
 
@@ -175,23 +173,33 @@
         ]
 
         reference._.rel = [RelationItem(dep=0, dest=1, relation=rel)]
 
         examples.append(Example(predicted, reference))
 
     _, llm = nlp.pipeline[0]
-    task: RELTask = llm._task
+    task: RELTask = llm._task  # type: ignore[annotation-unchecked]
 
     assert set(task._label_dict.values()) == set()
+    assert not task._prompt_examples
+
+    nlp.config["initialize"]["components"]["llm"] = {
+        "n_prompt_examples": n_prompt_examples
+    }
     nlp.initialize(lambda: examples)
+
     assert set(task._label_dict.values()) == {"LivesIn", "Visits"}
 
+    if n_prompt_examples >= 0:
+        assert len(task._prompt_examples) == n_prompt_examples
+    else:
+        assert len(task._prompt_examples) == len(examples)
 
-def test_rel_serde(noop_config, tmp_path: Path):
 
+def test_rel_serde(noop_config, tmp_path: Path):
     config = Config().from_str(noop_config)
     del config["components"]["llm"]["task"]["labels"]
 
     nlp1 = assemble_from_config(config)
     nlp2 = assemble_from_config(config)
     nlp3 = assemble_from_config(config)
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_spancat.py` & `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_spancat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 
 import pytest
 import spacy
 import srsly
 from confection import Config
-from pydantic import ValidationError
 from spacy.tokens import Span
 from spacy.training import Example
 from spacy.util import make_tempdir
 
 from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.registry import fewshot_reader, lowercase_normalizer, strip_normalizer
 from spacy_llm.tasks import make_spancat_task_v2
@@ -38,18 +37,16 @@
     [components.llm.task]
     @llm_tasks = "spacy.SpanCat.v2"
     labels = PER,ORG,LOC
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.fixture
 def fewshot_cfg_string():
     return f"""
     [nlp]
@@ -64,23 +61,21 @@
 
     [components.llm.task]
     @llm_tasks = "spacy.SpanCat.v2"
     labels = ["PER", "ORG", "LOC"]
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
-    path = {str((Path(__file__).parent / "examples" / "ner_examples.yml"))}
+    path = {str((Path(__file__).parent / "examples" / "ner.yml"))}
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config: {{}}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize("cfg_string", ["fewshot_cfg_string", "zeroshot_cfg_string"])
 def test_spancat_config(cfg_string, request):
@@ -93,15 +88,15 @@
     assert isinstance(pipe, LLMWrapper)
     assert isinstance(pipe.task, LLMTask)
 
     labels = orig_config["components"]["llm"]["task"]["labels"]
     labels = split_labels(labels)
     task = pipe.task
     assert isinstance(task, Labeled)
-    assert task.labels == tuple(labels)
+    assert sorted(task.labels) == sorted(tuple(labels))
     assert pipe.labels == task.labels
     assert nlp.pipe_labels["llm"] == list(task.labels)
 
 
 @pytest.mark.external
 @pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
 def test_spancat_predict(cfg_string, request):
@@ -387,17 +382,17 @@
     assert (
         prompt.strip()
         == """
 You are an expert Named Entity Recognition (NER) system. Your task is to accept Text as input and extract named entities for the set of predefined entity labels.
 The entities you extract for each label can overlap with each other.
 From the Text input provided, extract named entities for each label in the following format:
 
-PER: <comma delimited list of strings>
-ORG: <comma delimited list of strings>
 LOC: <comma delimited list of strings>
+ORG: <comma delimited list of strings>
+PER: <comma delimited list of strings>
 
 
 Here is the text that needs labeling:
 
 Text:
 '''
 Alice and Bob went to the supermarket
@@ -405,17 +400,17 @@
 """.strip()
     )
 
 
 @pytest.mark.parametrize(
     "examples_path",
     [
-        str(EXAMPLES_DIR / "ner_examples.json"),
-        str(EXAMPLES_DIR / "ner_examples.yml"),
-        str(EXAMPLES_DIR / "ner_examples.jsonl"),
+        str(EXAMPLES_DIR / "ner.json"),
+        str(EXAMPLES_DIR / "ner.yml"),
+        str(EXAMPLES_DIR / "ner.jsonl"),
     ],
 )
 def test_jinja_template_rendering_with_examples(examples_path):
     """Test if jinja2 template renders as expected
 
     We apply the .strip() method for each prompt so that we don't have to deal
     with annoying newlines and spaces at the edge of the text.
@@ -431,17 +426,17 @@
     assert (
         prompt.strip()
         == """
 You are an expert Named Entity Recognition (NER) system. Your task is to accept Text as input and extract named entities for the set of predefined entity labels.
 The entities you extract for each label can overlap with each other.
 From the Text input provided, extract named entities for each label in the following format:
 
-PER: <comma delimited list of strings>
-ORG: <comma delimited list of strings>
 LOC: <comma delimited list of strings>
+ORG: <comma delimited list of strings>
+PER: <comma delimited list of strings>
 
 
 Below are some examples (only use these as a guide):
 
 Text:
 '''
 Jack and Jill went up the hill.
@@ -482,18 +477,16 @@
             "entities": [("PER", ("Entities")), ("ORG", ("dict", "list"))],
         }
     ]
     with make_tempdir() as tmpdir:
         tmp_path = tmpdir / "wrong_example.yml"
         srsly.write_yaml(tmp_path, wrong_example)
 
-        with pytest.raises(ValidationError):
-            make_spancat_task_v2(
-                labels="PER,ORG,LOC", examples=fewshot_reader(tmp_path)
-            )
+    with pytest.raises(ValueError):
+        make_spancat_task_v2(labels="PER,ORG,LOC", examples=fewshot_reader(tmp_path))
 
 
 @pytest.fixture
 def noop_config():
     return """
     [nlp]
     lang = "en"
@@ -508,23 +501,22 @@
     [components.llm.task]
     @llm_tasks = "spacy.SpanCat.v2"
     labels = ["PER", "ORG", "LOC"]
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "test.NoOpBackend.v1"
+    [components.llm.model]
+    @llm_models = "test.NoOpModel.v1"
     output = "PER: Bob,Alice"
     """
 
 
 @pytest.mark.parametrize("n_detections", [0, 1, 2])
 def test_spancat_scoring(noop_config, n_detections):
-
     config = Config().from_str(noop_config)
     nlp = assemble_from_config(config)
 
     examples = []
 
     for text in ["Alice works with Bob.", "Bob lives with Alice."]:
         predicted = nlp.make_doc(text)
@@ -538,16 +530,16 @@
         examples.append(Example(predicted, reference))
 
     scores = nlp.evaluate(examples)
 
     assert scores["spans_sc_p"] == n_detections / 2
 
 
-def test_spancat_init(noop_config):
-
+@pytest.mark.parametrize("n_prompt_examples", [-1, 0, 1, 2])
+def test_spancat_init(noop_config, n_prompt_examples: bool):
     config = Config().from_str(noop_config)
     del config["components"]["llm"]["task"]["labels"]
     nlp = assemble_from_config(config)
 
     examples = []
 
     for text in [
@@ -565,20 +557,34 @@
 
         examples.append(Example(predicted, reference))
 
     _, llm = nlp.pipeline[0]
     task: SpanCatTask = llm._task
 
     assert set(task._label_dict.values()) == set()
+    assert not task._prompt_examples
+
+    nlp.config["initialize"]["components"]["llm"] = {
+        "n_prompt_examples": n_prompt_examples
+    }
+
     nlp.initialize(lambda: examples)
+
     assert set(task._label_dict.values()) == {"PER", "LOC"}
+    if n_prompt_examples >= 0:
+        assert len(task._prompt_examples) == n_prompt_examples
+    else:
+        assert len(task._prompt_examples) == len(examples)
+
+    if n_prompt_examples > 0:
+        for eg in task._prompt_examples:
+            assert set(eg.entities.keys()) == {"PER", "LOC"}
 
 
 def test_spancat_serde(noop_config):
-
     config = Config().from_str(noop_config)
     del config["components"]["llm"]["task"]["labels"]
 
     nlp1 = assemble_from_config(config)
     nlp2 = assemble_from_config(config)
 
     labels = {"loc": "LOC", "per": "PER"}
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_textcat.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from pathlib import Path
 from typing import Iterable
 
 import pytest
 import spacy
 import srsly
 from confection import Config
-from pydantic import ValidationError
 from spacy.training import Example
 from spacy.util import make_tempdir
 
 from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.registry import fewshot_reader, file_reader, lowercase_normalizer
 from spacy_llm.registry import registry
 from spacy_llm.tasks.textcat import TextCatTask, make_textcat_task_v3
@@ -40,18 +39,16 @@
     @llm_tasks = "spacy.TextCat.v1"
     labels = "Recipe"
     exclusive_classes = true
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.fixture
 def fewshot_cfg_string():
     return f"""
     [nlp]
@@ -67,23 +64,21 @@
     [components.llm.task]
     @llm_tasks = "spacy.TextCat.v1"
     labels = "Recipe"
     exclusive_classes = true
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
-    path = {str(EXAMPLES_DIR / "textcat_examples.yml")}
+    path = {str(EXAMPLES_DIR / "textcat.yml")}
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {{}}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.fixture
 def ext_template_cfg_string():
     """Simple zero-shot config with an external template"""
 
@@ -101,23 +96,21 @@
     [components.llm.task]
     @llm_tasks = "spacy.TextCat.v2"
     labels = ["Recipe"]
     exclusive_classes = true
 
     [components.llm.task.template]
     @misc = "spacy.FileReader.v1"
-    path = {str((Path(__file__).parent / "templates" / "textcat_template.jinja2"))}
+    path = {str((Path(__file__).parent / "templates" / "textcat.jinja2"))}
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {{}}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.fixture
 def zeroshot_cfg_string_v3_lds():
     return """
     [nlp]
@@ -137,48 +130,46 @@
 
     [components.llm.task.label_definitions]
     Recipe = "A recipe is a set of instructions for preparing a meal, including a list of the ingredients required."
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "spacy.REST.v1"
-    api = "OpenAI"
-    config = {}
+    [components.llm.model]
+    @llm_models = "spacy.GPT-3-5.v1"
     """
 
 
 @pytest.fixture
 def binary():
     text = "Get 1 cup of sugar, half a cup of butter, and mix them together to make a cream"
     labels = "Recipe"
     gold_cats = ["Recipe"]
     exclusive_classes = True
-    examples_path = str(EXAMPLES_DIR / "textcat_binary_examples.yml")
+    examples_path = str(EXAMPLES_DIR / "textcat_binary.yml")
     return text, labels, gold_cats, exclusive_classes, examples_path
 
 
 @pytest.fixture
 def multilabel_excl():
     text = "You need to increase the temperature when baking, it looks undercooked."
     labels = "Recipe,Feedback,Comment"
     gold_cats = ["Recipe", "Feedback", "Comment"]
     exclusive_classes = True
-    examples_path = str(EXAMPLES_DIR / "textcat_multi_excl_examples.yml")
+    examples_path = str(EXAMPLES_DIR / "textcat_multi_excl.yml")
     return text, labels, gold_cats, exclusive_classes, examples_path
 
 
 @pytest.fixture
 def multilabel_nonexcl():
     text = "I suggest you add some bananas. Mix 3 pieces of banana to your batter before baking."
     labels = "Recipe,Feedback,Comment"
     gold_cats = ["Recipe", "Feedback", "Comment"]
     exclusive_classes = False
-    examples_path = str(EXAMPLES_DIR / "textcat_multi_nonexcl_examples.yml")
+    examples_path = str(EXAMPLES_DIR / "textcat_multi_nonexcl.yml")
     return text, labels, gold_cats, exclusive_classes, examples_path
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize(
     "task",
@@ -214,15 +205,15 @@
     pipe = nlp.get_pipe("llm")
     assert isinstance(pipe, LLMWrapper)
     assert isinstance(pipe.task, LLMTask)
 
     labels = split_labels(labels)
     task = pipe.task
     assert isinstance(task, Labeled)
-    assert task.labels == tuple(labels)
+    assert sorted(task.labels) == sorted(tuple(labels))
     assert pipe.labels == task.labels
     assert nlp.pipe_labels["llm"] == list(task.labels)
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize("task", ["binary", "multilabel_nonexcl", "multilabel_excl"])
@@ -358,23 +349,23 @@
         normalizer=lowercase_normalizer(),
     )
     nlp = spacy.blank("xx")
     doc = nlp.make_doc(text)
     pred = list(llm_textcat.parse_responses([doc], [response]))[0]
     # Take only those that have scores
     pred_cats = [cat for cat, score in pred.cats.items() if score == 1.0]
-    assert pred_cats == expected
+    assert set(pred_cats) == set(expected)
 
 
 @pytest.mark.parametrize(
     "examples_path",
     [
-        str(EXAMPLES_DIR / "textcat_binary_examples.json"),
-        str(EXAMPLES_DIR / "textcat_binary_examples.yml"),
-        str(EXAMPLES_DIR / "textcat_binary_examples.jsonl"),
+        str(EXAMPLES_DIR / "textcat_binary.json"),
+        str(EXAMPLES_DIR / "textcat_binary.yml"),
+        str(EXAMPLES_DIR / "textcat_binary.jsonl"),
     ],
 )
 def test_jinja_template_rendering_with_examples_for_binary(examples_path, binary):
     """Test if jinja2 template renders as expected
 
     We apply the .strip() method for each prompt so that we don't have to deal
     with annoying newlines and spaces at the edge of the text.
@@ -433,17 +424,17 @@
 '''""".strip()
     )
 
 
 @pytest.mark.parametrize(
     "examples_path",
     [
-        str(EXAMPLES_DIR / "textcat_multi_excl_examples.json"),
-        str(EXAMPLES_DIR / "textcat_multi_excl_examples.yml"),
-        str(EXAMPLES_DIR / "textcat_multi_excl_examples.jsonl"),
+        str(EXAMPLES_DIR / "textcat_multi_excl.json"),
+        str(EXAMPLES_DIR / "textcat_multi_excl.yml"),
+        str(EXAMPLES_DIR / "textcat_multi_excl.jsonl"),
     ],
 )
 def test_jinja_template_rendering_with_examples_for_multilabel_exclusive(
     examples_path, multilabel_excl
 ):
     text, labels, _, exclusive_classes, _ = multilabel_excl
     nlp = spacy.blank("xx")
@@ -458,15 +449,15 @@
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
 You are an expert Text Classification system. Your task is to accept Text as input
 and provide a category for the text based on the predefined labels.
 
-Classify the text below to any of the following labels: Recipe, Feedback, Comment
+Classify the text below to any of the following labels: Comment, Feedback, Recipe
 
 The task is exclusive, so only choose one label from what I provided.
 Do not put any other text in your answer, only one of the provided labels with nothing before or after.
 Below are some examples (only use these as a guide):
 
 
 Text:
@@ -500,17 +491,17 @@
 '''""".strip()
     )
 
 
 @pytest.mark.parametrize(
     "examples_path",
     [
-        str(EXAMPLES_DIR / "textcat_multi_nonexcl_examples.json"),
-        str(EXAMPLES_DIR / "textcat_multi_nonexcl_examples.yml"),
-        str(EXAMPLES_DIR / "textcat_multi_nonexcl_examples.jsonl"),
+        str(EXAMPLES_DIR / "textcat_multi_nonexcl.json"),
+        str(EXAMPLES_DIR / "textcat_multi_nonexcl.yml"),
+        str(EXAMPLES_DIR / "textcat_multi_nonexcl.jsonl"),
     ],
 )
 def test_jinja_template_rendering_with_examples_for_multilabel_nonexclusive(
     examples_path, multilabel_nonexcl
 ):
     text, labels, _, exclusive_classes, _ = multilabel_nonexcl
     nlp = spacy.blank("xx")
@@ -525,15 +516,15 @@
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
 You are an expert Text Classification system. Your task is to accept Text as input
 and provide a category for the text based on the predefined labels.
 
-Classify the text below to any of the following labels: Recipe, Feedback, Comment
+Classify the text below to any of the following labels: Comment, Feedback, Recipe
 
 The task is non-exclusive, so you can provide more than one label as long as
 they're comma-delimited. For example: Label1, Label2, Label3.
 Do not put any other text in your answer, only one or more of the provided labels with nothing before or after.
 If the text cannot be classified into any of the provided labels, answer `==NONE==`.
 Below are some examples (only use these as a guide):
 
@@ -581,24 +572,24 @@
     ],
 )
 def test_example_not_following_basemodel(wrong_example, labels, exclusive_classes):
     with make_tempdir() as tmpdir:
         tmp_path = tmpdir / "wrong_example.yml"
         srsly.write_yaml(tmp_path, wrong_example)
 
-        with pytest.raises(ValidationError):
+        with pytest.raises(ValueError):
             make_textcat_task_v3(
                 labels=labels,
                 examples=fewshot_reader(tmp_path),
                 exclusive_classes=exclusive_classes,
             )
 
 
 def test_external_template_actually_loads():
-    template_path = str(TEMPLATES_DIR / "textcat_template.jinja2")
+    template_path = str(TEMPLATES_DIR / "textcat.jinja2")
     template = file_reader(template_path)
     labels = "Recipe"
     nlp = spacy.blank("xx")
     doc = nlp.make_doc("Combine 2 cloves of garlic with soy sauce")
 
     llm_textcat = make_textcat_task_v3(labels=labels, template=template)
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
@@ -639,24 +630,24 @@
     "Nincompoop!",
     "Shipwreckers!",
 ]
 
 
 @pytest.mark.parametrize("n_insults", range(len(INSULTS) + 1))
 def test_textcat_scoring(zeroshot_cfg_string, n_insults):
-    @registry.llm_backends("Dummy")
+    @registry.llm_models("Dummy")
     def factory():
         def b(prompts: Iterable[str]) -> Iterable[str]:
             for _ in prompts:
                 yield "POS"
 
         return b
 
     config = Config().from_str(zeroshot_cfg_string)
-    config["components"]["llm"]["backend"] = {"@llm_backends": "Dummy"}
+    config["components"]["llm"]["model"] = {"@llm_models": "Dummy"}
     config["components"]["llm"]["task"]["labels"] = "Insult"
     nlp = assemble_from_config(config)
 
     examples = []
 
     for i, text in enumerate(INSULTS):
         predicted = nlp.make_doc(text)
@@ -692,15 +683,15 @@
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
 You are an expert Text Classification system. Your task is to accept Text as input
 and provide a category for the text based on the predefined labels.
 
-Classify the text below to any of the following labels: Recipe, Feedback, Comment
+Classify the text below to any of the following labels: Comment, Feedback, Recipe
 
 The task is exclusive, so only choose one label from what I provided.
 Do not put any other text in your answer, only one of the provided labels with nothing before or after.
 
 Below are definitions of each label to help aid you in correctly classifying the text.
 Assume these definitions are written by an expert and follow them closely.
 
@@ -734,22 +725,26 @@
 
     [components.llm.task]
     @llm_tasks = "spacy.TextCat.v1"
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
-    [components.llm.backend]
-    @llm_backends = "test.NoOpBackend.v1"
+    [components.llm.model]
+    @llm_models = "test.NoOpModel.v1"
     """
 
 
+@pytest.mark.parametrize("n_prompt_examples", [-1, 0, 1, 2])
 @pytest.mark.parametrize("init_from_config", [True, False])
-def test_textcat_init(noop_config, init_from_config: bool):
-
+def test_textcat_init(
+    noop_config,
+    init_from_config: bool,
+    n_prompt_examples: bool,
+):
     config = Config().from_str(noop_config)
     if init_from_config:
         config["initialize"] = {"components": {"llm": {"labels": ["Test"]}}}
     nlp = assemble_from_config(config)
 
     examples = []
 
@@ -768,26 +763,34 @@
     task: TextCatTask = llm._task
 
     if init_from_config:
         target = {"Test"}
     else:
         target = set()
     assert set(task._label_dict.values()) == target
+    assert not task._prompt_examples
+
+    nlp.config["initialize"]["components"]["llm"] = {
+        "n_prompt_examples": n_prompt_examples
+    }
 
     nlp.initialize(lambda: examples)
 
     if init_from_config:
         target = {"Test"}
     else:
         target = {"Insult", "Compliment"}
     assert set(task._label_dict.values()) == target
+    if n_prompt_examples >= 0:
+        assert len(task._prompt_examples) == n_prompt_examples
+    else:
+        assert len(task._prompt_examples) == len(INSULTS)
 
 
 def test_textcat_serde(noop_config, tmp_path: Path):
-
     config = Config().from_str(noop_config)
 
     nlp1 = assemble_from_config(config)
     nlp2 = assemble_from_config(config)
     nlp3 = assemble_from_config(config)
 
     labels = {"insult": "INSULT", "compliment": "COMPLIMENT"}
```

### Comparing `spacy-llm-0.3.2/spacy_llm/tests/test_combinations.py` & `spacy-llm-0.4.0/spacy_llm/tests/test_combinations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-import copy
 from typing import Any, Dict
 
 import pytest
 import spacy
-from thinc.api import get_current_ops, NumpyOps
+from thinc.api import NumpyOps, get_current_ops
 
-from spacy_llm.compat import has_minichain, has_langchain
+from spacy_llm.compat import has_langchain
 from spacy_llm.pipeline import LLMWrapper
 
-PIPE_CFG: Dict[str, Any] = {
-    "backend": {
-        "@llm_backends": None,
-        "api": "OpenAI",
-        "config": {},
-    },
-    "task": {"@llm_tasks": None},
-}
-
 
 @pytest.mark.external
-@pytest.mark.skipif(has_minichain is False, reason="MiniChain is not installed")
 @pytest.mark.skipif(has_langchain is False, reason="LangChain is not installed")
 @pytest.mark.parametrize(
-    "backend",
-    ["spacy.LangChain.v1", "spacy.MiniChain.v1", "spacy.REST.v1"],
-    ids=["langchain", "minichain", "rest"],
+    "model",
+    ["langchain.OpenAI.v1", "spacy.GPT-3-5.v1"],
+    ids=["langchain", "rest-openai"],
 )
 @pytest.mark.parametrize(
     "task",
     ["spacy.NER.v1", "spacy.NER.v2", "spacy.TextCat.v1"],
     ids=["ner.v1", "ner.v2", "textcat"],
 )
-@pytest.mark.parametrize("n_process", [1, 2])
-def test_combinations(backend: str, task: str, n_process: int):
-    """Randomly test combinations of backends and tasks."""
+@pytest.mark.parametrize("n_process", [1])  # , 2
+def test_combinations(model: str, task: str, n_process: int):
+    """Randomly test combinations of models and tasks."""
     ops = get_current_ops()
     if not isinstance(ops, NumpyOps) and n_process != 1:
         pytest.skip("Only test multiple processes on CPU")
 
-    config = copy.deepcopy(PIPE_CFG)
-    config["backend"]["@llm_backends"] = backend
-    config["backend"]["config"] = {
-        "model": "ada" if backend != "spacy.MiniChain.v1" else "gpt-3.5-turbo"
+    config: Dict[str, Any] = {
+        "model": {
+            "@llm_models": model,
+            "config": {},
+        },
+        "task": {"@llm_tasks": task},
     }
-    config["task"]["@llm_tasks"] = task
-
+    if model.startswith("langchain"):
+        config["model"]["name"] = "ada"
     # Configure task-specific settings.
     if task.startswith("spacy.NER"):
         config["task"]["labels"] = "PER,ORG,LOC"
     elif task.startswith("spacy.TextCat"):
         config["task"]["labels"] = "Recipe"
         config["task"]["exclusive_classes"] = True
```

### Comparing `spacy-llm-0.3.2/spacy_llm/ty.py` & `spacy-llm-0.4.0/spacy_llm/ty.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, Union
 from typing import cast
 
 from spacy.tokens import Doc
 from spacy.training.example import Example
 from spacy.vocab import Vocab
 
-from .backends import integration
 from .compat import Protocol, runtime_checkable
+from .models import langchain
 
 _Prompt = Any
 _Response = Any
 
 PromptExecutor = Callable[[Iterable[_Prompt]], Iterable[_Response]]
 ExamplesConfigType = Union[
     Iterable[Dict[str, Any]], Callable[[], Iterable[Dict[str, Any]]], None
@@ -73,41 +73,55 @@
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[_Response]
     ) -> Iterable[Doc]:
         ...
 
 
 @runtime_checkable
+class PromptTemplateProvider(Protocol):
+    @property
+    def prompt_template(self) -> str:
+        ...
+
+
+@runtime_checkable
 class Labeled(Protocol):
     @property
     def labels(self) -> Tuple[str, ...]:
         ...
 
 
 @runtime_checkable
 class Cache(Protocol):
     """Defines minimal set of operations a cache implementiation needs to support."""
 
-    @property
-    def vocab(self) -> Optional[Vocab]:
-        """Vocab used for deserializing docs.
-        RETURNS (Vocab): Vocab used for deserializing docs.
+    def initialize(self, vocab: Vocab, task: LLMTask) -> None:
         """
-
-    @vocab.setter
-    def vocab(self, vocab: Vocab) -> None:
-        """Set vocab to use for deserializing docs.
-        vocab (Vocab): Vocab to use for deserializing docs.
+        Initialize cache with data not available at construction time.
+        vocab (Vocab): Vocab object.
+        task (LLMTask): Task.
         """
 
     def add(self, doc: Doc) -> None:
         """Adds processed doc to cache (or to a queue that is added to the cache at a later point)
         doc (Doc): Doc to add to persistence queue.
         """
 
+    @property
+    def prompt_template(self) -> Optional[str]:
+        """Get prompt template.
+        RETURNS (Optional[str]): Prompt template string used for docs to cache/cached docs.
+        """
+
+    @prompt_template.setter
+    def prompt_template(self, prompt_template: str) -> None:
+        """Set prompt template.
+        prompt_template (str): Prompt template string used for docs to cache/cached docs.
+        """
+
     def __contains__(self, doc: Doc) -> bool:
         """Checks whether doc has been processed and cached.
         doc (Doc): Doc to check for.
         RETURNS (bool): Whether doc has been processed and cached.
         """
 
     def __getitem__(self, doc: Doc) -> Optional[Doc]:
@@ -136,54 +150,54 @@
         [
             issubclass(out_tv, in_tv) or issubclass(in_tv, out_tv)
             for out_tv, in_tv in zip(out_type_vars, in_type_vars)
         ]
     )
 
 
-def _extract_backend_call_signature(backend: PromptExecutor) -> Dict[str, Any]:
-    """Extract call signature from backend object.
-    backend (PromptExecutor): Backend object to extract call signature from.
+def _extract_model_call_signature(model: PromptExecutor) -> Dict[str, Any]:
+    """Extract call signature from model object.
+    model (PromptExecutor): Model object to extract call signature from.
     RETURNS (Dict[str, Any]): Type per argument name.
     """
-    if inspect.isfunction(backend):
-        return typing.get_type_hints(backend)
+    if inspect.isfunction(model):
+        return typing.get_type_hints(model)
 
-    if not hasattr(backend, "__call__"):
-        raise ValueError("The object supplied as backend must implement `__call__()`.")
+    if not hasattr(model, "__call__"):
+        raise ValueError("The object supplied as model must implement `__call__()`.")
 
-    # Assume that __call__() has the necessary type info - except in the case of integration.Backend, for which
+    # Assume that __call__() has the necessary type info - except in the case of integration.Model, for which
     # we know this is not the case.
-    if not isinstance(backend, integration.RemoteBackend):
-        return typing.get_type_hints(backend.__call__)
+    if not isinstance(model, langchain.LangChain):
+        return typing.get_type_hints(model.__call__)
 
-    # If this is an instance of integrations.RemoteBackend: read type information from .query() instead, only keep
+    # If this is an instance of integrations.Model: read type information from .query() instead, only keep
     # information on Iterable args.
-    signature = typing.get_type_hints(backend.query).items()
+    signature = typing.get_type_hints(model.query).items()
     to_ignore: List[str] = []
     for k, v in signature:
         if not (hasattr(v, "__origin__") and issubclass(v.__origin__, Iterable)):
             to_ignore.append(k)
 
     signature = {
         k: v
-        for k, v in typing.get_type_hints(backend.query).items()
+        for k, v in typing.get_type_hints(model.query).items()
         # In Python 3.8+ (or 3.6+ if typing_utils is installed) the check for the origin class should be done using
         # typing.get_origin().
         if k not in to_ignore
     }
     assert len(signature) == 2
     assert "return" in signature
     return signature
 
 
-def validate_type_consistency(task: LLMTask, backend: PromptExecutor) -> None:
-    """Check whether the types of the task and backend signatures match.
+def validate_type_consistency(task: LLMTask, model: PromptExecutor) -> None:
+    """Check whether the types of the task and model signatures match.
     task (LLMTask): Specified task.
-    backend (PromptExecutor): Specified backend.
+    backend (PromptExecutor): Specified model.
     """
     # Raises an error or prints a warning if something looks wrong/odd.
     if not isinstance(task, LLMTask):
         raise ValueError(
             f"A task needs to be of type 'LLMTask' but found {type(task)} instead"
         )
     if not hasattr(task, "generate_prompts"):
@@ -195,31 +209,31 @@
             "A task needs to have the following method: "
             "parse_responses(self, docs: Iterable[Doc], responses: Iterable[Any]) -> Iterable[Doc]"
         )
 
     type_hints = {
         "template": typing.get_type_hints(task.generate_prompts),
         "parse": typing.get_type_hints(task.parse_responses),
-        "backend": _extract_backend_call_signature(backend),
+        "model": _extract_model_call_signature(model),
     }
 
     parse_input: Optional[Type] = None
-    backend_input: Optional[Type] = None
-    backend_output: Optional[Type] = None
+    model_input: Optional[Type] = None
+    model_output: Optional[Type] = None
 
-    # Validate the 'backend' object
-    if not (len(type_hints["backend"]) == 2 and "return" in type_hints["backend"]):
+    # Validate the 'model' object
+    if not (len(type_hints["model"]) == 2 and "return" in type_hints["model"]):
         raise ValueError(
-            "The 'backend' Callable should have one input argument and one return value."
+            "The 'model' Callable should have one input argument and one return value."
         )
-    for k in type_hints["backend"]:
+    for k in type_hints["model"]:
         if k == "return":
-            backend_output = type_hints["backend"][k]
+            model_output = type_hints["model"][k]
         else:
-            backend_input = type_hints["backend"][k]
+            model_input = type_hints["model"][k]
 
     # validate the 'parse' object
     if not (len(type_hints["parse"]) == 3 and "return" in type_hints["parse"]):
         raise ValueError(
             "The 'task.parse_responses()' function should have two input arguments and one return value."
         )
     for k in type_hints["parse"]:
@@ -230,32 +244,32 @@
 
     template_output = type_hints["template"]["return"]
 
     # Check that all variables are Iterables.
     for var, msg in (
         (template_output, "`task.generate_prompts()` needs to return an `Iterable`."),
         (
-            backend_input,
-            "The prompts variable in the 'backend' needs to be an `Iterable`.",
+            model_input,
+            "The prompts variable in the 'model' needs to be an `Iterable`.",
         ),
-        (backend_output, "The `backend` function needs to return an `Iterable`."),
+        (model_output, "The `model` function needs to return an `Iterable`."),
         (
             parse_input,
             "`responses` in `task.parse_responses()` needs to be an `Iterable`.",
         ),
     ):
         if not var != Iterable:
             raise ValueError(msg)
 
-    # Ensure that the template returns the same type as expected by the backend
-    if not _do_args_match(template_output, backend_input):  # type: ignore[arg-type]
+    # Ensure that the template returns the same type as expected by the model
+    if not _do_args_match(template_output, model_input):  # type: ignore[arg-type]
         warnings.warn(
             f"Type returned from `task.generate_prompts()` (`{template_output}`) doesn't match type expected by "
-            f"`backend` (`{backend_input}`)."
+            f"`model` (`{model_input}`)."
         )
 
-    # Ensure that the parser expects the same type as returned by the backend
-    if not _do_args_match(backend_output, parse_input):  # type: ignore[arg-type]
+    # Ensure that the parser expects the same type as returned by the model
+    if not _do_args_match(model_output, parse_input):  # type: ignore[arg-type]
         warnings.warn(
-            f"Type returned from `backend` (`{backend_output}`) doesn't match type expected by "
+            f"Type returned from `model` (`{model_output}`) doesn't match type expected by "
             f"`task.parse_responses()` (`{parse_input}`)."
         )
```

### Comparing `spacy-llm-0.3.2/spacy_llm/util.py` & `spacy-llm-0.4.0/spacy_llm/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/usage_examples/multitask_openai/run_pipeline.py` & `spacy-llm-0.4.0/usage_examples/multitask_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/usage_examples/ner_dolly/run_pipeline.py` & `spacy-llm-0.4.0/usage_examples/ner_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/usage_examples/ner_langchain_openai/run_pipeline.py` & `spacy-llm-0.4.0/usage_examples/ner_langchain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/usage_examples/ner_minichain_openai/run_pipeline.py` & `spacy-llm-0.4.0/usage_examples/textcat_openai/run_pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import os
 from pathlib import Path
+from typing import Optional
 
 import typer
 from wasabi import msg
 
 from spacy_llm.util import assemble
 
 Arg = typer.Argument
 Opt = typer.Option
 
 
 def run_pipeline(
     # fmt: off
-    text: str = Arg("", help="Text to perform NER on."),
+    text: str = Arg("", help="Text to perform text categorization on."),
     config_path: Path = Arg(..., help="Path to the configuration file to use."),
+    examples_path: Optional[Path] = Arg(None, help="Path to the examples file to use (few-shot only)."),
     verbose: bool = Opt(False, "--verbose", "-v", help="Show extra information."),
     # fmt: on
 ):
     if not os.getenv("OPENAI_API_KEY", None):
         msg.fail(
             "OPENAI_API_KEY env variable was not found. "
             "Set it by running 'export OPENAI_API_KEY=...' and try again.",
             exits=1,
         )
 
     msg.text(f"Loading config from {config_path}", show=verbose)
-    nlp = assemble(config_path)
+    nlp = assemble(
+        config_path,
+        overrides={}
+        if examples_path is None
+        else {"paths.examples": str(examples_path)},
+    )
     doc = nlp(text)
 
     msg.text(f"Text: {doc.text}")
-    msg.text(f"Entities: {doc.ents}")
+    msg.text(f"Categories: {doc.cats}")
 
 
 if __name__ == "__main__":
     typer.run(run_pipeline)
```

### Comparing `spacy-llm-0.3.2/usage_examples/rel_openai/run_pipeline.py` & `spacy-llm-0.4.0/usage_examples/rel_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.2/usage_examples/tests/test_readme_examples.py` & `spacy-llm-0.4.0/usage_examples/tests/test_readme_examples.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Iterable, Callable
+from typing import Callable, Iterable
 
 import pytest
 import spacy
+from spacy import util
 from thinc.compat import has_torch_cuda_gpu
 
-from spacy import util
 from spacy_llm.registry import registry
 from spacy_llm.util import assemble
 
 
 @pytest.mark.external
 def test_example_1_classifier():
     with util.make_tempdir() as tmpdir:
@@ -22,18 +22,17 @@
         [components.llm]
         factory = "llm"
 
         [components.llm.task]
         @llm_tasks = "spacy.TextCat.v2"
         labels = ["COMPLIMENT", "INSULT"]
 
-        [components.llm.backend]
-        @llm_backends = "spacy.REST.v1"
-        api = "OpenAI"
-        config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
+        [components.llm.model]
+        @llm_models = "spacy.GPT-3-5.v1"
+        config = {"temperature": 0.3}
         """
 
         with open(tmpdir / "cfg", "w") as text_file:
             text_file.write(cfg_str)
 
         nlp = assemble(tmpdir / "cfg")
         doc = nlp("You look gorgeous!")
@@ -53,18 +52,18 @@
         [components.llm]
         factory = "llm"
 
         [components.llm.task]
         @llm_tasks = "spacy.NER.v2"
         labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
-        [components.llm.backend]
-        @llm_backends = "spacy.Dolly_HF.v1"
+        [components.llm.model]
+        @llm_models = "spacy.Dolly.v1"
         # For better performance, use databricks/dolly-v2-12b instead
-        model = "databricks/dolly-v2-3b"
+        name = "dolly-v2-3b"
         """
 
         with open(tmpdir / "cfg", "w") as text_file:
             text_file.write(cfg_str)
 
         nlp = assemble(tmpdir / "cfg")
         doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
@@ -77,30 +76,28 @@
     nlp.add_pipe(
         "llm",
         config={
             "task": {
                 "@llm_tasks": "spacy.NER.v2",
                 "labels": ["PERSON", "ORGANISATION", "LOCATION"],
             },
-            "backend": {
-                "@llm_backends": "spacy.REST.v1",
-                "api": "OpenAI",
-                "config": {"model": "gpt-3.5-turbo"},
+            "model": {
+                "@llm_models": "spacy.GPT-3-5.v1",
             },
         },
     )
     nlp.initialize()
     doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
     print([(ent.text, ent.label_) for ent in doc.ents])  # noqa: T201
 
 
-def test_example_4_custom_backend():
+def test_example_4_custom_model():
     import random
 
-    @registry.llm_backends("RandomClassification.v1")
+    @registry.llm_models("RandomClassification.v1")
     def random_textcat(labels: str) -> Callable[[Iterable[str]], Iterable[str]]:
         labels = labels.split(",")
 
         def _classify(prompts: Iterable[str]) -> Iterable[str]:
             for _ in prompts:
                 yield random.choice(labels)
 
@@ -117,16 +114,16 @@
         [components.llm]
         factory = "llm"
 
         [components.llm.task]
         @llm_tasks = "spacy.TextCat.v2"
         labels = ORDER,INFORMATION
 
-        [components.llm.backend]
-        @llm_backends = "RandomClassification.v1"
+        [components.llm.model]
+        @llm_models = "RandomClassification.v1"
         labels = ${components.llm.task.labels}
         """
 
         with open(tmpdir / "cfg", "w") as text_file:
             text_file.write(cfg_str)
 
         nlp = assemble(tmpdir / "cfg")
```

### Comparing `spacy-llm-0.3.2/usage_examples/tests/test_usage_examples.py` & `spacy-llm-0.4.0/usage_examples/tests/test_usage_examples.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from pathlib import Path
 
 import pytest
 from thinc.compat import has_torch_cuda_gpu
+
 from spacy_llm import cache  # noqa: F401
 
-from .. import (
-    ner_dolly,
-    textcat_openai,
-    ner_langchain_openai,
-    ner_minichain_openai,
-    multitask_openai,
-    rel_openai,
-)
+from .. import multitask_openai, ner_dolly, ner_langchain_openai, rel_openai
+from .. import textcat_openai
 
 _USAGE_EXAMPLE_PATH = Path(__file__).parent.parent
 
 
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 @pytest.mark.parametrize("config_name", ("fewshot.cfg", "zeroshot.cfg"))
 def test_ner_dolly(config_name: str):
@@ -53,22 +48,14 @@
     """Test NER LangChain OpenAI usage example."""
     ner_langchain_openai.run_pipeline(
         "text", _USAGE_EXAMPLE_PATH / "ner_langchain_openai" / "ner.cfg", False
     )
 
 
 @pytest.mark.external
-def test_ner_minichain_openai():
-    """Test NER LangChain OpenAI usage example."""
-    ner_minichain_openai.run_pipeline(
-        "text", _USAGE_EXAMPLE_PATH / "ner_minichain_openai" / "ner.cfg", False
-    )
-
-
-@pytest.mark.external
 @pytest.mark.parametrize("config_name", ("fewshot.cfg", "zeroshot.cfg"))
 def test_multitask_openai(config_name: str):
     """Test multitask OpenAI example.
     config_name (str): Name of config file to use.
     """
     path = _USAGE_EXAMPLE_PATH / "multitask_openai"
     multitask_openai.run_pipeline(
@@ -76,21 +63,21 @@
         config_path=path / config_name,
         examples_path=None if config_name == "zeroshot.cfg" else path / "examples.yml",
         verbose=False,
     )
 
 
 @pytest.mark.external
-@pytest.mark.parametrize("config_name", ("fewshot.cfg", "zeroshot.cfg"))
+@pytest.mark.parametrize("config_name", ("zeroshot.cfg", "fewshot.cfg"))
 def test_rel_openai(config_name: str):
     """Test REL OpenAI usage example.
     config_name (str): Name of config file to use.
     """
     path = _USAGE_EXAMPLE_PATH / "rel_openai"
     rel_openai.run_pipeline(
-        text="text",
+        text="Sara lives in Lisbon.",
         config_path=path / config_name,
         examples_path=None
         if config_name == "zeroshot.cfg"
         else path / "examples.jsonl",
         verbose=False,
     )
```

