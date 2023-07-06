# Comparing `tmp/llama_index-0.7.0.tar.gz` & `tmp/llama_index-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.7.0.tar", last modified: Tue Jul  4 15:28:38 2023, max compression
+gzip compressed data, was "llama_index-0.7.1.tar", last modified: Wed Jul  5 09:00:46 2023, max compression
```

## Comparing `llama_index-0.7.0.tar` & `llama_index-0.7.1.tar`

### file list

```diff
@@ -1,644 +1,645 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.479011 llama_index-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 15:28:19.000000 llama_index-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-04 15:28:19.000000 llama_index-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-04 15:28:38.479011 llama_index-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-04 15:28:19.000000 llama_index-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.411008 llama_index-0.7.0/llama_index/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.415008 llama_index-0.7.0/llama_index/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/agent/context_retriever_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/agent/openai_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/agent/retriever_openai_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.415008 llama_index-0.7.0/llama_index/bridge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/bridge/langchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.415008 llama_index-0.7.0/llama_index/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/callbacks/aim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/callbacks/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/callbacks/token_counting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/callbacks/wandb_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.415008 llama_index-0.7.0/llama_index/chat_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/chat_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/chat_engine/condense_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/chat_engine/react.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/chat_engine/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/chat_engine/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.415008 llama_index-0.7.0/llama_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.415008 llama_index-0.7.0/llama_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/data_structs/document_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/data_structs/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.419008 llama_index-0.7.0/llama_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/embeddings/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.419008 llama_index-0.7.0/llama_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/evaluation/guideline_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.419008 llama_index-0.7.0/llama_index/graph_stores/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/graph_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16582 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/graph_stores/nebulagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/graph_stores/registery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/graph_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/graph_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.419008 llama_index-0.7.0/llama_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.419008 llama_index-0.7.0/llama_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.419008 llama_index-0.7.0/llama_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.423008 llama_index-0.7.0/llama_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.423008 llama_index-0.7.0/llama_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.423008 llama_index-0.7.0/llama_index/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/document_summary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/document_summary/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.423008 llama_index-0.7.0/llama_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.423008 llama_index-0.7.0/llama_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.423008 llama_index-0.7.0/llama_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/knowledge_graph/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.423008 llama_index-0.7.0/llama_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.423008 llama_index-0.7.0/llama_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/postprocessor/cohere_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/postprocessor/llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/postprocessor/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/postprocessor/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.427008 llama_index-0.7.0/llama_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.427008 llama_index-0.7.0/llama_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/query/query_transform/feedback_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.427008 llama_index-0.7.0/llama_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/struct_store/json_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.427008 llama_index-0.7.0/llama_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/tree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.427008 llama_index-0.7.0/llama_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/vector_store/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.427008 llama_index-0.7.0/llama_index/indices/vector_store/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/vector_store/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.427008 llama_index-0.7.0/llama_index/indices/vector_store/retrievers/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/indices/vector_store/retrievers/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.431008 llama_index-0.7.0/llama_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.431008 llama_index-0.7.0/llama_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/langchain_helpers/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.431008 llama_index-0.7.0/llama_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.431008 llama_index-0.7.0/llama_index/llm_predictor/vellum/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/vellum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/vellum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/vellum/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/vellum/prompt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/vellum/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llm_predictor/vellum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.435009 llama_index-0.7.0/llama_index/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/langchain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/llms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.435009 llama_index-0.7.0/llama_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.435009 llama_index-0.7.0/llama_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/node_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.435009 llama_index-0.7.0/llama_index/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/objects/base_node_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/objects/table_node_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/objects/tool_node_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.435009 llama_index-0.7.0/llama_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/output_parsers/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/output_parsers/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/output_parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.435009 llama_index-0.7.0/llama_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.435009 llama_index-0.7.0/llama_index/program/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/base_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/guidance_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/llm_program.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/llm_prompt_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/openai_program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.435009 llama_index-0.7.0/llama_index/program/predefined/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/predefined/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/predefined/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.439009 llama_index-0.7.0/llama_index/program/predefined/evaporate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/predefined/evaporate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/predefined/evaporate/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/predefined/evaporate/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/program/predefined/evaporate/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.439009 llama_index-0.7.0/llama_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/choice_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/guidance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/prompt_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/prompts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.439009 llama_index-0.7.0/llama_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/citation_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.439009 llama_index-0.7.0/llama_index/query_engine/flare/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/flare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/flare/answer_inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/flare/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/flare/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/flare/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/pandas_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/retry_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/retry_source_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/sql_join_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/sql_vector_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/sub_question_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.443009 llama_index-0.7.0/llama_index/question_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/question_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/question_gen/guidance_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/question_gen/llm_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/question_gen/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/question_gen/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/question_gen/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.443009 llama_index-0.7.0/llama_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.447009 llama_index-0.7.0/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.447009 llama_index-0.7.0/llama_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/docs_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/epub_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/image_caption_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/image_vision_llm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/ipynb_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/markdown_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/mbox_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/slides_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/tabular_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/file/video_audio_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.447009 llama_index-0.7.0/llama_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.447009 llama_index-0.7.0/llama_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.447009 llama_index-0.7.0/llama_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/psychic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.447009 llama_index-0.7.0/llama_index/readers/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.447009 llama_index-0.7.0/llama_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.447009 llama_index-0.7.0/llama_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.447009 llama_index-0.7.0/llama_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.451010 llama_index-0.7.0/llama_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response/pprint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.451010 llama_index-0.7.0/llama_index/response_synthesizers/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/accumulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/compact_and_accumulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/compact_and_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/simple_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/tree_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/response_synthesizers/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.451010 llama_index-0.7.0/llama_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.451010 llama_index-0.7.0/llama_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/selectors/pydantic_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.451010 llama_index-0.7.0/llama_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.455010 llama_index-0.7.0/llama_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/docstore/dynamodb_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/docstore/redis_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.455010 llama_index-0.7.0/llama_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/index_store/dynamodb_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/index_store/redis_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.455010 llama_index-0.7.0/llama_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/kvstore/dynamodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/kvstore/redis_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/kvstore/s3_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.455010 llama_index-0.7.0/llama_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.455010 llama_index-0.7.0/llama_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/function_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/ondemand_loader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/query_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.455010 llama_index-0.7.0/llama_index/tools/tool_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/tool_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/tool_spec/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.459010 llama_index-0.7.0/llama_index/tools/tool_spec/notion/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/tool_spec/notion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/tool_spec/notion/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.459010 llama_index-0.7.0/llama_index/tools/tool_spec/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/tool_spec/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/tool_spec/slack/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.459010 llama_index-0.7.0/llama_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/llama_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/deeplake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/llama_index/vector_stores/docarray/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/docarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/docarray/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/docarray/hnsw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/docarray/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/lancedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/supabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/tair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/typesense.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-04 15:28:20.000000 llama_index-0.7.0/llama_index/vector_stores/weaviate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.411008 llama_index-0.7.0/llama_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-04 15:28:38.000000 llama_index-0.7.0/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20504 2023-07-04 15:28:38.000000 llama_index-0.7.0/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:28:38.000000 llama_index-0.7.0/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-04 15:28:38.000000 llama_index-0.7.0/llama_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 15:28:38.000000 llama_index-0.7.0/llama_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 15:28:20.000000 llama_index-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:28:38.479011 llama_index-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-04 15:28:20.000000 llama_index-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/callbacks/test_token_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/tests/chat_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/chat_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/chat_engine/test_condense_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/chat_engine/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/tests/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/document_summary/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/document_summary/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.463010 llama_index-0.7.0/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.467011 llama_index-0.7.0/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.467011 llama_index-0.7.0/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.467011 llama_index-0.7.0/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.467011 llama_index-0.7.0/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/postprocessor/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/postprocessor/test_llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/postprocessor/test_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.467011 llama_index-0.7.0/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.467011 llama_index-0.7.0/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/query/test_embedding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.467011 llama_index-0.7.0/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/struct_store/test_json_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.471011 llama_index-0.7.0/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.471011 llama_index-0.7.0/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.471011 llama_index-0.7.0/tests/indices/vector_store/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/auto_retriever/test_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.471011 llama_index-0.7.0/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.471011 llama_index-0.7.0/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.471011 llama_index-0.7.0/tests/llm_predictor/vellum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llm_predictor/vellum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llm_predictor/vellum/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llm_predictor/vellum/test_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llm_predictor/vellum/test_prompt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llm_predictor/vellum/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llms/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llms/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llms/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llms/test_openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/llms/test_palm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/objects/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/objects/test_node_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/output_parsers/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/output_parsers/test_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/program/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/program/test_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/program/test_llm_program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/prompts/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/prompts/test_guidance_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/question_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/question_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/question_gen/test_guidance_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/question_gen/test_llm_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.475011 llama_index-0.7.0/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.479011 llama_index-0.7.0/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.479011 llama_index-0.7.0/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.479011 llama_index-0.7.0/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/storage/docstore/test_dynamodb_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/storage/docstore/test_redis_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/storage/test_storage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.479011 llama_index-0.7.0/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.479011 llama_index-0.7.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/tools/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/tools/test_ondemand_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/tools/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.479011 llama_index-0.7.0/tests/tools/tool_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/tools/tool_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/tools/tool_spec/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:38.479011 llama_index-0.7.0/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/vector_stores/test_docarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/vector_stores/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/vector_stores/test_tair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 15:28:20.000000 llama_index-0.7.0/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.736050 llama_index-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 09:00:25.000000 llama_index-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 09:00:25.000000 llama_index-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-05 09:00:46.732050 llama_index-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-05 09:00:25.000000 llama_index-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.652049 llama_index-0.7.1/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.652049 llama_index-0.7.1/llama_index/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/agent/context_retriever_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/agent/openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/agent/retriever_openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.652049 llama_index-0.7.1/llama_index/bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/bridge/langchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.656050 llama_index-0.7.1/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/callbacks/aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/callbacks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/callbacks/token_counting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/callbacks/wandb_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.656050 llama_index-0.7.1/llama_index/chat_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/chat_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/chat_engine/condense_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/chat_engine/react.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/chat_engine/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/chat_engine/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.656050 llama_index-0.7.1/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.656050 llama_index-0.7.1/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/data_structs/document_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.656050 llama_index-0.7.1/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.656050 llama_index-0.7.1/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/evaluation/guideline_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.656050 llama_index-0.7.1/llama_index/graph_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16582 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/graph_stores/nebulagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/graph_stores/registery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/graph_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/graph_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/document_summary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/document_summary/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/knowledge_graph/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.660050 llama_index-0.7.1/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.664049 llama_index-0.7.1/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/postprocessor/llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/postprocessor/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.664049 llama_index-0.7.1/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.664049 llama_index-0.7.1/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/query/query_transform/feedback_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.664049 llama_index-0.7.1/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/struct_store/json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.664049 llama_index-0.7.1/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/tree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.664049 llama_index-0.7.1/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/vector_store/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.668049 llama_index-0.7.1/llama_index/indices/vector_store/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/vector_store/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.668049 llama_index-0.7.1/llama_index/indices/vector_store/retrievers/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/indices/vector_store/retrievers/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.668049 llama_index-0.7.1/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.668049 llama_index-0.7.1/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/langchain_helpers/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.668049 llama_index-0.7.1/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.668049 llama_index-0.7.1/llama_index/llm_predictor/vellum/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/vellum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/vellum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/vellum/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/vellum/prompt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/vellum/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llm_predictor/vellum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.672050 llama_index-0.7.1/llama_index/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/langchain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/llms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.672050 llama_index-0.7.1/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.672050 llama_index-0.7.1/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.672050 llama_index-0.7.1/llama_index/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/objects/base_node_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/objects/table_node_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/objects/tool_node_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.672050 llama_index-0.7.1/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/output_parsers/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/output_parsers/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/output_parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.672050 llama_index-0.7.1/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.672050 llama_index-0.7.1/llama_index/program/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/base_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/guidance_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/llm_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/llm_prompt_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/openai_program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.672050 llama_index-0.7.1/llama_index/program/predefined/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/predefined/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/predefined/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.676050 llama_index-0.7.1/llama_index/program/predefined/evaporate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/predefined/evaporate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/predefined/evaporate/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/predefined/evaporate/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/program/predefined/evaporate/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.676050 llama_index-0.7.1/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/guidance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/prompt_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/prompts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.676050 llama_index-0.7.1/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/citation_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.676050 llama_index-0.7.1/llama_index/query_engine/flare/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/flare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/flare/answer_inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/flare/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/flare/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/flare/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/pandas_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/retry_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/retry_source_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/sql_join_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/sql_vector_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/sub_question_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.676050 llama_index-0.7.1/llama_index/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/question_gen/guidance_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/question_gen/llm_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/question_gen/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/question_gen/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/question_gen/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.684049 llama_index-0.7.1/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.684049 llama_index-0.7.1/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/docs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/epub_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/image_caption_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/image_vision_llm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/ipynb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/markdown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/mbox_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/slides_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/tabular_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/file/video_audio_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/psychic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/readers/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response/pprint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/response_synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/compact_and_accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/compact_and_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/simple_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/tree_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/response_synthesizers/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.688050 llama_index-0.7.1/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/retrievers/recursive_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.692050 llama_index-0.7.1/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/selectors/pydantic_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.692050 llama_index-0.7.1/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.692050 llama_index-0.7.1/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/docstore/dynamodb_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/docstore/redis_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.692050 llama_index-0.7.1/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/index_store/dynamodb_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/index_store/redis_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.692050 llama_index-0.7.1/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/kvstore/dynamodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/kvstore/redis_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/kvstore/s3_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.692050 llama_index-0.7.1/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.696050 llama_index-0.7.1/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/function_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/ondemand_loader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/query_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.696050 llama_index-0.7.1/llama_index/tools/tool_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/tool_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/tool_spec/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.696050 llama_index-0.7.1/llama_index/tools/tool_spec/notion/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/tool_spec/notion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/tool_spec/notion/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.696050 llama_index-0.7.1/llama_index/tools/tool_spec/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/tool_spec/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/tool_spec/slack/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.696050 llama_index-0.7.1/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.700049 llama_index-0.7.1/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/deeplake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.700049 llama_index-0.7.1/llama_index/vector_stores/docarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/docarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/docarray/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/docarray/hnsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/docarray/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/supabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/tair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/typesense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-05 09:00:25.000000 llama_index-0.7.1/llama_index/vector_stores/weaviate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.652049 llama_index-0.7.1/llama_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-05 09:00:46.000000 llama_index-0.7.1/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20550 2023-07-05 09:00:46.000000 llama_index-0.7.1/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:00:46.000000 llama_index-0.7.1/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-05 09:00:46.000000 llama_index-0.7.1/llama_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 09:00:46.000000 llama_index-0.7.1/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-05 09:00:25.000000 llama_index-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:00:46.736050 llama_index-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-05 09:00:25.000000 llama_index-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.700049 llama_index-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.700049 llama_index-0.7.1/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/callbacks/test_token_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.700049 llama_index-0.7.1/tests/chat_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/chat_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/chat_engine/test_condense_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/chat_engine/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.700049 llama_index-0.7.1/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.704050 llama_index-0.7.1/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.704050 llama_index-0.7.1/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.704050 llama_index-0.7.1/tests/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/document_summary/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/document_summary/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.708050 llama_index-0.7.1/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.708050 llama_index-0.7.1/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.708050 llama_index-0.7.1/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.712050 llama_index-0.7.1/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.712050 llama_index-0.7.1/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/postprocessor/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/postprocessor/test_llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/postprocessor/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.716050 llama_index-0.7.1/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.716050 llama_index-0.7.1/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/query/test_embedding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.720050 llama_index-0.7.1/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/struct_store/test_json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.720050 llama_index-0.7.1/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.724050 llama_index-0.7.1/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.724050 llama_index-0.7.1/tests/indices/vector_store/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/auto_retriever/test_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/llm_predictor/vellum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llm_predictor/vellum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llm_predictor/vellum/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llm_predictor/vellum/test_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llm_predictor/vellum/test_prompt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llm_predictor/vellum/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llms/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llms/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llms/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llms/test_openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/llms/test_palm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/objects/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/objects/test_node_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/output_parsers/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/output_parsers/test_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.728050 llama_index-0.7.1/tests/program/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/program/test_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/program/test_llm_program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/prompts/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/prompts/test_guidance_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/question_gen/test_guidance_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/question_gen/test_llm_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/storage/docstore/test_dynamodb_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/storage/docstore/test_redis_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/tools/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/tools/test_ondemand_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/tools/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/tools/tool_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/tools/tool_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/tools/tool_spec/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:46.732050 llama_index-0.7.1/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/vector_stores/test_docarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/vector_stores/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/vector_stores/test_tair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 09:00:25.000000 llama_index-0.7.1/tests/vector_stores/test_weaviate.py
```

### Comparing `llama_index-0.7.0/LICENSE` & `llama_index-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/PKG-INFO` & `llama_index-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_index
-Version: 0.7.0
+Version: 0.7.1
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 Author: Jerry Liu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `llama_index-0.7.0/README.md` & `llama_index-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/__init__.py` & `llama_index-0.7.1/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/agent/context_retriever_agent.py` & `llama_index-0.7.1/llama_index/agent/context_retriever_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/agent/openai_agent.py` & `llama_index-0.7.1/llama_index/agent/openai_agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,34 @@
+import asyncio
 import json
+import queue
+import time
 from abc import abstractmethod
-from typing import Callable, List, Optional
+from threading import Thread
+from typing import (
+    AsyncGenerator,
+    Callable,
+    Generator,
+    List,
+    Tuple,
+    Optional,
+    Union,
+)
 
 from llama_index.callbacks.base import CallbackManager
 from llama_index.chat_engine.types import BaseChatEngine
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
-from llama_index.llms.base import ChatMessage, MessageRole
+from llama_index.llms.base import (
+    ChatMessage,
+    MessageRole,
+    ChatResponseGen,
+    ChatResponseAsyncGen,
+)
 from llama_index.llms.openai import OpenAI
 from llama_index.response.schema import RESPONSE_TYPE, Response
 from llama_index.schema import BaseNode, NodeWithScore
 from llama_index.tools import BaseTool
 
 DEFAULT_MAX_FUNCTION_CALLS = 5
 DEFAULT_MODEL_NAME = "gpt-3.5-turbo-0613"
@@ -49,14 +66,79 @@
         role=MessageRole.FUNCTION,
         additional_kwargs={
             "name": function_call["name"],
         },
     )
 
 
+class StreamingChatResponse:
+    """Streaming chat response to user and writing to chat history."""
+
+    def __init__(
+        self, chat_stream: Union[ChatResponseGen, ChatResponseAsyncGen]
+    ) -> None:
+        self._chat_stream = chat_stream
+        self._queue: queue.Queue = queue.Queue()
+        self._is_done = False
+        self._is_function: Optional[bool] = None
+        self.response_str = ""
+
+    def __str__(self) -> str:
+        return self.response_str
+
+    def write_response_to_history(self, chat_history: List[ChatMessage]) -> None:
+        if isinstance(self._chat_stream, AsyncGenerator):
+            raise ValueError(
+                "Cannot write to history with async generator in sync function."
+            )
+
+        final_message = None
+        for chat in self._chat_stream:
+            final_message = chat.message
+            self._is_function = (
+                final_message.additional_kwargs.get("function_call", None) is not None
+            )
+            self._queue.put_nowait(chat.delta)
+
+        if final_message is not None:
+            chat_history.append(final_message)
+
+        self._is_done = True
+
+    async def awrite_response_to_history(self, chat_history: List[ChatMessage]) -> None:
+        if isinstance(self._chat_stream, Generator):
+            raise ValueError(
+                "Cannot write to history with sync generator in async function."
+            )
+
+        final_message = None
+        async for chat in self._chat_stream:
+            final_message = chat.message
+            self._is_function = (
+                final_message.additional_kwargs.get("function_call", None) is not None
+            )
+            self._queue.put_nowait(chat.delta)
+
+        if final_message is not None:
+            chat_history.append(final_message)
+
+        self._is_done = True
+
+    @property
+    def response_gen(self) -> Generator[str, None, None]:
+        while not self._is_done or not self._queue.empty():
+            try:
+                delta = self._queue.get(block=False)
+                self.response_str += delta
+                yield delta
+            except queue.Empty:
+                # Queue is empty, but we're not done yet
+                continue
+
+
 class BaseOpenAIAgent(BaseChatEngine, BaseQueryEngine):
     """Base OpenAI Agent."""
 
     def __init__(
         self,
         llm: OpenAI,
         chat_history: List[ChatMessage],
@@ -77,29 +159,42 @@
     def reset(self) -> None:
         self._chat_history.clear()
 
     @abstractmethod
     def _get_tools(self, message: str) -> List[BaseTool]:
         """Get tools."""
 
+    def _get_latest_function_call(
+        self, chat_history: List[ChatMessage]
+    ) -> Optional[dict]:
+        """Get latest function call from chat history."""
+        return chat_history[-1].additional_kwargs.get("function_call", None)
+
+    def _init_chat(
+        self, chat_history: List[ChatMessage], message: str
+    ) -> Tuple[List[BaseTool], List[dict]]:
+        """Add user message to chat history and get tools and functions."""
+        chat_history.append(ChatMessage(content=message, role=MessageRole.USER))
+        tools = self._get_tools(message)
+        functions = [tool.metadata.to_openai_function() for tool in tools]
+        return tools, functions
+
     def chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
     ) -> RESPONSE_TYPE:
         chat_history = chat_history or self._chat_history
-        chat_history.append(ChatMessage(content=message, role="user"))
-        tools = self._get_tools(message)
-        functions = [tool.metadata.to_openai_function() for tool in tools]
+        tools, functions = self._init_chat(chat_history, message)
 
         # TODO: Support forced function call
         chat_response = self._llm.chat(chat_history, functions=functions)
         ai_message = chat_response.message
         chat_history.append(ai_message)
 
         n_function_calls = 0
-        function_call = ai_message.additional_kwargs.get("function_call", None)
+        function_call = self._get_latest_function_call(chat_history)
         while function_call is not None:
             if n_function_calls >= self._max_function_calls:
                 print(f"Exceeded max function calls: {self._max_function_calls}.")
                 break
 
             function_message = call_function(
                 tools, function_call, verbose=self._verbose
@@ -107,33 +202,98 @@
             chat_history.append(function_message)
             n_function_calls += 1
 
             # send function call & output back to get another response
             chat_response = self._llm.chat(chat_history, functions=functions)
             ai_message = chat_response.message
             chat_history.append(ai_message)
-            function_call = ai_message.additional_kwargs.get("function_call", None)
+            function_call = self._get_latest_function_call(chat_history)
 
         return Response(ai_message.content)
 
+    def stream_chat(
+        self, message: str, chat_history: Optional[List[ChatMessage]] = None
+    ) -> Generator[StreamingChatResponse, None, None]:
+        chat_history = chat_history or self._chat_history
+        tools, functions = self._init_chat(chat_history, message)
+
+        def gen(
+            chat_history: List[ChatMessage],
+        ) -> Generator[StreamingChatResponse, None, None]:
+            # TODO: Support forced function call
+            chat_stream_response = StreamingChatResponse(
+                self._llm.stream_chat(chat_history, functions=functions)
+            )
+
+            # Get the response in a separate thread so we can yield the response
+            thread = Thread(
+                target=chat_stream_response.write_response_to_history,
+                args=(chat_history,),
+            )
+            thread.start()
+            yield chat_stream_response
+
+            while chat_stream_response._is_function is None:
+                # Wait until we know if the response is a function call or not
+                time.sleep(0.05)
+                if chat_stream_response._is_function is False:
+                    return
+
+            thread.join()
+
+            n_function_calls = 0
+            function_call = self._get_latest_function_call(chat_history)
+            while function_call is not None:
+                if n_function_calls >= self._max_function_calls:
+                    print(f"Exceeded max function calls: {self._max_function_calls}.")
+                    break
+
+                function_message = call_function(
+                    tools, function_call, verbose=self._verbose
+                )
+                chat_history.append(function_message)
+                n_function_calls += 1
+
+                # send function call & output back to get another response
+                chat_stream_response = StreamingChatResponse(
+                    self._llm.stream_chat(chat_history, functions=functions)
+                )
+
+                # Get the response in a separate thread so we can yield the response
+                thread = Thread(
+                    target=chat_stream_response.write_response_to_history,
+                    args=(chat_history,),
+                )
+                thread.start()
+                yield chat_stream_response
+
+                while chat_stream_response._is_function is None:
+                    # Wait until we know if the response is a function call or not
+                    time.sleep(0.05)
+                    if chat_stream_response._is_function is False:
+                        return
+
+                thread.join()
+                function_call = self._get_latest_function_call(chat_history)
+
+        return gen(chat_history)
+
     async def achat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
     ) -> RESPONSE_TYPE:
         chat_history = chat_history or self._chat_history
-        chat_history.append(ChatMessage(content=message, role="user"))
-        tools = self._get_tools(message)
-        functions = [tool.metadata.to_openai_function() for tool in tools]
+        tools, functions = self._init_chat(chat_history, message)
 
         # TODO: Support forced function call
         chat_response = await self._llm.achat(chat_history, functions=functions)
         ai_message = chat_response.message
         chat_history.append(ai_message)
 
         n_function_calls = 0
-        function_call = ai_message.additional_kwargs.get("function_call", None)
+        function_call = self._get_latest_function_call(chat_history)
         while function_call is not None:
             if n_function_calls >= self._max_function_calls:
                 print(f"Exceeded max function calls: {self._max_function_calls}.")
                 continue
 
             function_message = call_function(
                 tools, function_call, verbose=self._verbose
@@ -141,18 +301,89 @@
             chat_history.append(function_message)
             n_function_calls += 1
 
             # send function call & output back to get another response
             response = await self._llm.achat(chat_history, functions=functions)
             ai_message = response.message
             chat_history.append(ai_message)
-            function_call = ai_message.additional_kwargs.get("function_call", None)
+            function_call = self._get_latest_function_call(chat_history)
 
         return Response(ai_message.content)
 
+    def astream_chat(
+        self, message: str, chat_history: Optional[List[ChatMessage]] = None
+    ) -> AsyncGenerator[StreamingChatResponse, None]:
+        chat_history = chat_history or self._chat_history
+        tools, functions = self._init_chat(chat_history, message)
+
+        async def gen(
+            chat_history: List[ChatMessage],
+        ) -> AsyncGenerator[StreamingChatResponse, None]:
+            # TODO: Support forced function call
+            chat_stream_response = StreamingChatResponse(
+                await self._llm.astream_chat(chat_history, functions=functions)
+            )
+
+            # Get the response in a separate thread so we can yield the response
+            thread = Thread(
+                target=lambda x: asyncio.run(
+                    chat_stream_response.awrite_response_to_history(x)
+                ),
+                args=(chat_history,),
+            )
+            thread.start()
+            yield chat_stream_response
+
+            while chat_stream_response._is_function is None:
+                # Wait until we know if the response is a function call or not
+                time.sleep(0.05)
+                if chat_stream_response._is_function is False:
+                    return
+
+            thread.join()
+
+            n_function_calls = 0
+            function_call = self._get_latest_function_call(chat_history)
+            while function_call is not None:
+                if n_function_calls >= self._max_function_calls:
+                    print(f"Exceeded max function calls: {self._max_function_calls}.")
+                    break
+
+                function_message = call_function(
+                    tools, function_call, verbose=self._verbose
+                )
+                chat_history.append(function_message)
+                n_function_calls += 1
+
+                # send function call & output back to get another response
+                chat_stream_response = StreamingChatResponse(
+                    await self._llm.astream_chat(chat_history, functions=functions)
+                )
+
+                # Get the response in a separate thread so we can yield the response
+                thread = Thread(
+                    target=lambda x: asyncio.run(
+                        chat_stream_response.awrite_response_to_history(x)
+                    ),
+                    args=(chat_history,),
+                )
+                thread.start()
+                yield chat_stream_response
+
+                while chat_stream_response._is_function is None:
+                    # Wait until we know if the response is a function call or not
+                    time.sleep(0.05)
+                    if chat_stream_response._is_function is False:
+                        return
+
+                thread.join()
+                function_call = self._get_latest_function_call(chat_history)
+
+        return gen(chat_history)
+
     # ===== Query Engine Interface =====
     def _query(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
         return self.chat(
             query_bundle.query_str,
             chat_history=[],
         )
```

### Comparing `llama_index-0.7.0/llama_index/agent/retriever_openai_agent.py` & `llama_index-0.7.1/llama_index/agent/retriever_openai_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/async_utils.py` & `llama_index-0.7.1/llama_index/async_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/bridge/langchain.py` & `llama_index-0.7.1/llama_index/bridge/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/callbacks/aim.py` & `llama_index-0.7.1/llama_index/callbacks/aim.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/callbacks/base.py` & `llama_index-0.7.1/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/callbacks/llama_debug.py` & `llama_index-0.7.1/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/callbacks/schema.py` & `llama_index-0.7.1/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/callbacks/token_counting.py` & `llama_index-0.7.1/llama_index/callbacks/token_counting.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/callbacks/wandb_callback.py` & `llama_index-0.7.1/llama_index/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/chat_engine/condense_question.py` & `llama_index-0.7.1/llama_index/chat_engine/condense_question.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/chat_engine/react.py` & `llama_index-0.7.1/llama_index/chat_engine/react.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/chat_engine/simple.py` & `llama_index-0.7.1/llama_index/chat_engine/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/chat_engine/types.py` & `llama_index-0.7.1/llama_index/chat_engine/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/composability/joint_qa_summary.py` & `llama_index-0.7.1/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/data_structs/data_structs.py` & `llama_index-0.7.1/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/data_structs/document_summary.py` & `llama_index-0.7.1/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/data_structs/registry.py` & `llama_index-0.7.1/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/data_structs/struct_type.py` & `llama_index-0.7.1/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/data_structs/table.py` & `llama_index-0.7.1/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/embeddings/base.py` & `llama_index-0.7.1/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/embeddings/google.py` & `llama_index-0.7.1/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/embeddings/langchain.py` & `llama_index-0.7.1/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/embeddings/openai.py` & `llama_index-0.7.1/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/embeddings/utils.py` & `llama_index-0.7.1/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/evaluation/base.py` & `llama_index-0.7.1/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/evaluation/dataset_generation.py` & `llama_index-0.7.1/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/evaluation/guideline_eval.py` & `llama_index-0.7.1/llama_index/evaluation/guideline_eval.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/graph_stores/nebulagraph.py` & `llama_index-0.7.1/llama_index/graph_stores/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/graph_stores/registery.py` & `llama_index-0.7.1/llama_index/graph_stores/registery.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/graph_stores/simple.py` & `llama_index-0.7.1/llama_index/graph_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/graph_stores/types.py` & `llama_index-0.7.1/llama_index/graph_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/img_utils.py` & `llama_index-0.7.1/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/__init__.py` & `llama_index-0.7.1/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/base.py` & `llama_index-0.7.1/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/base_retriever.py` & `llama_index-0.7.1/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/common/struct_store/base.py` & `llama_index-0.7.1/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.7.1/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.7.1/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/common_tree/base.py` & `llama_index-0.7.1/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/composability/graph.py` & `llama_index-0.7.1/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/document_summary/base.py` & `llama_index-0.7.1/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/document_summary/retrievers.py` & `llama_index-0.7.1/llama_index/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/empty/base.py` & `llama_index-0.7.1/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/empty/retrievers.py` & `llama_index-0.7.1/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.7.1/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/keyword_table/base.py` & `llama_index-0.7.1/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.7.1/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.7.1/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.7.1/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/keyword_table/utils.py` & `llama_index-0.7.1/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.7.1/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/knowledge_graph/retriever.py` & `llama_index-0.7.1/llama_index/indices/knowledge_graph/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/list/base.py` & `llama_index-0.7.1/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/list/retrievers.py` & `llama_index-0.7.1/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/loading.py` & `llama_index-0.7.1/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/postprocessor/__init__.py` & `llama_index-0.7.1/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/postprocessor/cohere_rerank.py` & `llama_index-0.7.1/llama_index/indices/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/postprocessor/llm_rerank.py` & `llama_index-0.7.1/llama_index/indices/postprocessor/llm_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/postprocessor/node.py` & `llama_index-0.7.1/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.7.1/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/postprocessor/optimizer.py` & `llama_index-0.7.1/llama_index/indices/postprocessor/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/postprocessor/pii.py` & `llama_index-0.7.1/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/prompt_helper.py` & `llama_index-0.7.1/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/query/base.py` & `llama_index-0.7.1/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/query/embedding_utils.py` & `llama_index-0.7.1/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/query/query_transform/base.py` & `llama_index-0.7.1/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/query/query_transform/feedback_transform.py` & `llama_index-0.7.1/llama_index/indices/query/query_transform/feedback_transform.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.7.1/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/query/schema.py` & `llama_index-0.7.1/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/registry.py` & `llama_index-0.7.1/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/service_context.py` & `llama_index-0.7.1/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/struct_store/__init__.py` & `llama_index-0.7.1/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/struct_store/base.py` & `llama_index-0.7.1/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.7.1/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/struct_store/json_query.py` & `llama_index-0.7.1/llama_index/indices/struct_store/json_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/struct_store/pandas.py` & `llama_index-0.7.1/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/struct_store/sql.py` & `llama_index-0.7.1/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.7.1/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/tree/__init__.py` & `llama_index-0.7.1/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.7.1/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/tree/base.py` & `llama_index-0.7.1/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/tree/inserter.py` & `llama_index-0.7.1/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.7.1/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.7.1/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.7.1/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/tree/utils.py` & `llama_index-0.7.1/llama_index/indices/tree/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/utils.py` & `llama_index-0.7.1/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/vector_store/base.py` & `llama_index-0.7.1/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py` & `llama_index-0.7.1/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py` & `llama_index-0.7.1/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py` & `llama_index-0.7.1/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/indices/vector_store/retrievers/retriever.py` & `llama_index-0.7.1/llama_index/indices/vector_store/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.7.1/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.7.1/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.7.1/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.7.1/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.7.1/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.7.1/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/langchain_helpers/streaming.py` & `llama_index-0.7.1/llama_index/langchain_helpers/streaming.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.7.1/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llm_predictor/base.py` & `llama_index-0.7.1/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llm_predictor/mock.py` & `llama_index-0.7.1/llama_index/llm_predictor/mock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llm_predictor/structured.py` & `llama_index-0.7.1/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llm_predictor/utils.py` & `llama_index-0.7.1/llama_index/llm_predictor/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llm_predictor/vellum/predictor.py` & `llama_index-0.7.1/llama_index/llm_predictor/vellum/predictor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llm_predictor/vellum/prompt_registry.py` & `llama_index-0.7.1/llama_index/llm_predictor/vellum/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llm_predictor/vellum/types.py` & `llama_index-0.7.1/llama_index/llm_predictor/vellum/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llms/base.py` & `llama_index-0.7.1/llama_index/llms/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llms/custom.py` & `llama_index-0.7.1/llama_index/llms/custom.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llms/generic_utils.py` & `llama_index-0.7.1/llama_index/llms/generic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llms/huggingface.py` & `llama_index-0.7.1/llama_index/llms/huggingface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llms/langchain.py` & `llama_index-0.7.1/llama_index/llms/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llms/langchain_utils.py` & `llama_index-0.7.1/llama_index/llms/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llms/mock.py` & `llama_index-0.7.1/llama_index/llms/mock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llms/openai.py` & `llama_index-0.7.1/llama_index/llms/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,22 +143,30 @@
                 content_delta = delta.get("content", "") or ""
                 content += content_delta
 
                 function_call_delta = delta.get("function_call", None)
                 if function_call_delta is not None:
                     if function_call is None:
                         function_call = function_call_delta
+
+                        ## ensure we do not add a blank function call
+                        if function_call.get("function_name", "") is None:
+                            del function_call["function_name"]
                     else:
                         function_call["arguments"] += function_call_delta["arguments"]
 
+                additional_kwargs = {}
+                if function_call is not None:
+                    additional_kwargs["function_call"] = function_call
+
                 yield ChatResponse(
                     message=ChatMessage(
                         role=role,
                         content=content,
-                        additional_kwargs={"function_call": function_call},
+                        additional_kwargs=additional_kwargs,
                     ),
                     delta=content_delta,
                     raw=response,
                 )
 
         return gen()
 
@@ -321,22 +329,30 @@
                 content_delta = delta.get("content", "") or ""
                 content += content_delta
 
                 function_call_delta = delta.get("function_call", None)
                 if function_call_delta is not None:
                     if function_call is None:
                         function_call = function_call_delta
+
+                        ## ensure we do not add a blank function call
+                        if function_call.get("function_name", "") is None:
+                            del function_call["function_name"]
                     else:
                         function_call["arguments"] += function_call_delta["arguments"]
 
+                additional_kwargs = {}
+                if function_call is not None:
+                    additional_kwargs["function_call"] = function_call
+
                 yield ChatResponse(
                     message=ChatMessage(
                         role=role,
                         content=content,
-                        additional_kwargs={"function_call": function_call},
+                        additional_kwargs=additional_kwargs,
                     ),
                     delta=content_delta,
                     raw=response,
                 )
 
         return gen()
```

### Comparing `llama_index-0.7.0/llama_index/llms/openai_utils.py` & `llama_index-0.7.1/llama_index/llms/openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/llms/palm.py` & `llama_index-0.7.1/llama_index/llms/palm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/logger/base.py` & `llama_index-0.7.1/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/node_parser/interface.py` & `llama_index-0.7.1/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/node_parser/node_utils.py` & `llama_index-0.7.1/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/node_parser/simple.py` & `llama_index-0.7.1/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/objects/__init__.py` & `llama_index-0.7.1/llama_index/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/objects/base.py` & `llama_index-0.7.1/llama_index/objects/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/objects/base_node_mapping.py` & `llama_index-0.7.1/llama_index/objects/base_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/objects/table_node_mapping.py` & `llama_index-0.7.1/llama_index/objects/table_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/objects/tool_node_mapping.py` & `llama_index-0.7.1/llama_index/objects/tool_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/output_parsers/guardrails.py` & `llama_index-0.7.1/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/output_parsers/langchain.py` & `llama_index-0.7.1/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/output_parsers/pydantic.py` & `llama_index-0.7.1/llama_index/output_parsers/pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/output_parsers/selection.py` & `llama_index-0.7.1/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/output_parsers/utils.py` & `llama_index-0.7.1/llama_index/output_parsers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/playground/base.py` & `llama_index-0.7.1/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/program/__init__.py` & `llama_index-0.7.1/llama_index/program/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/program/guidance_program.py` & `llama_index-0.7.1/llama_index/program/guidance_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/program/llm_program.py` & `llama_index-0.7.1/llama_index/program/llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/program/llm_prompt_program.py` & `llama_index-0.7.1/llama_index/program/llm_prompt_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/program/openai_program.py` & `llama_index-0.7.1/llama_index/program/openai_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/program/predefined/df.py` & `llama_index-0.7.1/llama_index/program/predefined/df.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/program/predefined/evaporate/base.py` & `llama_index-0.7.1/llama_index/program/predefined/evaporate/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/program/predefined/evaporate/extractor.py` & `llama_index-0.7.1/llama_index/program/predefined/evaporate/extractor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/program/predefined/evaporate/prompts.py` & `llama_index-0.7.1/llama_index/program/predefined/evaporate/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/base.py` & `llama_index-0.7.1/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/chat_prompts.py` & `llama_index-0.7.1/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/choice_select.py` & `llama_index-0.7.1/llama_index/prompts/choice_select.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.7.1/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/default_prompts.py` & `llama_index-0.7.1/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/guidance_utils.py` & `llama_index-0.7.1/llama_index/prompts/guidance_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/prompt_selector.py` & `llama_index-0.7.1/llama_index/prompts/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/prompt_type.py` & `llama_index-0.7.1/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/prompts.py` & `llama_index-0.7.1/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/prompts/utils.py` & `llama_index-0.7.1/llama_index/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/__init__.py` & `llama_index-0.7.1/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/citation_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/citation_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/flare/answer_inserter.py` & `llama_index-0.7.1/llama_index/query_engine/flare/answer_inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/flare/base.py` & `llama_index-0.7.1/llama_index/query_engine/flare/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/flare/output_parser.py` & `llama_index-0.7.1/llama_index/query_engine/flare/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/pandas_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/pandas_query_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     # see langchain.tools.python.tool (PythonAstREPLTool)
     try:
         tree = ast.parse(output)
         module = ast.Module(tree.body[:-1], type_ignores=[])
         exec(ast.unparse(module), {}, local_vars)  # type: ignore
         module_end = ast.Module(tree.body[-1:], type_ignores=[])
         module_end_str = ast.unparse(module_end)  # type: ignore
+        print(module_end_str)
         try:
             return str(eval(module_end_str, {}, local_vars))
         except Exception as e:
             raise e
     except Exception as e:
         err_string = (
             "There was an error running the output as Python code. "
```

### Comparing `llama_index-0.7.0/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/retry_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/retry_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/retry_source_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/retry_source_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/router_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/sql_join_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/sql_join_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/sql_vector_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/sql_vector_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/sub_question_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/sub_question_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.7.1/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/question_gen/guidance_generator.py` & `llama_index-0.7.1/llama_index/question_gen/guidance_generator.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/question_gen/llm_generators.py` & `llama_index-0.7.1/llama_index/question_gen/llm_generators.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/question_gen/output_parser.py` & `llama_index-0.7.1/llama_index/question_gen/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/question_gen/prompts.py` & `llama_index-0.7.1/llama_index/question_gen/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/question_gen/types.py` & `llama_index-0.7.1/llama_index/question_gen/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/__init__.py` & `llama_index-0.7.1/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/base.py` & `llama_index-0.7.1/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.7.1/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/chroma.py` & `llama_index-0.7.1/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/database.py` & `llama_index-0.7.1/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/deeplake.py` & `llama_index-0.7.1/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/discord_reader.py` & `llama_index-0.7.1/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/download.py` & `llama_index-0.7.1/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/elasticsearch.py` & `llama_index-0.7.1/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/faiss.py` & `llama_index-0.7.1/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/base.py` & `llama_index-0.7.1/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/docs_reader.py` & `llama_index-0.7.1/llama_index/readers/file/docs_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/epub_reader.py` & `llama_index-0.7.1/llama_index/readers/file/epub_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/image_caption_reader.py` & `llama_index-0.7.1/llama_index/readers/file/image_caption_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/image_reader.py` & `llama_index-0.7.1/llama_index/readers/file/image_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/image_vision_llm_reader.py` & `llama_index-0.7.1/llama_index/readers/file/image_vision_llm_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/ipynb_reader.py` & `llama_index-0.7.1/llama_index/readers/file/ipynb_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/markdown_reader.py` & `llama_index-0.7.1/llama_index/readers/file/markdown_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/mbox_reader.py` & `llama_index-0.7.1/llama_index/readers/file/mbox_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/slides_reader.py` & `llama_index-0.7.1/llama_index/readers/file/slides_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/tabular_reader.py` & `llama_index-0.7.1/llama_index/readers/file/tabular_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/file/video_audio_reader.py` & `llama_index-0.7.1/llama_index/readers/file/video_audio_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.7.1/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.7.1/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/github_readers/utils.py` & `llama_index-0.7.1/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.7.1/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.7.1/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/json.py` & `llama_index-0.7.1/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/make_com/wrapper.py` & `llama_index-0.7.1/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/mbox.py` & `llama_index-0.7.1/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/metal.py` & `llama_index-0.7.1/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/milvus.py` & `llama_index-0.7.1/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/mongo.py` & `llama_index-0.7.1/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/myscale.py` & `llama_index-0.7.1/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/notion.py` & `llama_index-0.7.1/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/obsidian.py` & `llama_index-0.7.1/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/pinecone.py` & `llama_index-0.7.1/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/psychic.py` & `llama_index-0.7.1/llama_index/readers/psychic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/qdrant.py` & `llama_index-0.7.1/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/redis/utils.py` & `llama_index-0.7.1/llama_index/readers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/slack.py` & `llama_index-0.7.1/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/steamship/file_reader.py` & `llama_index-0.7.1/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/string_iterable.py` & `llama_index-0.7.1/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/twitter.py` & `llama_index-0.7.1/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/weaviate/reader.py` & `llama_index-0.7.1/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/web.py` & `llama_index-0.7.1/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/wikipedia.py` & `llama_index-0.7.1/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/readers/youtube_transcript.py` & `llama_index-0.7.1/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response/notebook_utils.py` & `llama_index-0.7.1/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response/pprint_utils.py` & `llama_index-0.7.1/llama_index/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response/schema.py` & `llama_index-0.7.1/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/__init__.py` & `llama_index-0.7.1/llama_index/response_synthesizers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/accumulate.py` & `llama_index-0.7.1/llama_index/response_synthesizers/accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/base.py` & `llama_index-0.7.1/llama_index/response_synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/compact_and_accumulate.py` & `llama_index-0.7.1/llama_index/response_synthesizers/compact_and_accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/compact_and_refine.py` & `llama_index-0.7.1/llama_index/response_synthesizers/compact_and_refine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/factory.py` & `llama_index-0.7.1/llama_index/response_synthesizers/factory.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/generation.py` & `llama_index-0.7.1/llama_index/response_synthesizers/generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/refine.py` & `llama_index-0.7.1/llama_index/response_synthesizers/refine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/simple_summarize.py` & `llama_index-0.7.1/llama_index/response_synthesizers/simple_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/tree_summarize.py` & `llama_index-0.7.1/llama_index/response_synthesizers/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/response_synthesizers/type.py` & `llama_index-0.7.1/llama_index/response_synthesizers/type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/retrievers/__init__.py` & `llama_index-0.7.1/llama_index/retrievers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from llama_index.indices.tree.select_leaf_retriever import TreeSelectLeafRetriever
 from llama_index.indices.tree.tree_root_retriever import TreeRootRetriever
 from llama_index.indices.vector_store.retrievers import (
     VectorIndexAutoRetriever,
     VectorIndexRetriever,
 )
 from llama_index.retrievers.transform_retriever import TransformRetriever
+from llama_index.retrievers.recursive_retriever import RecursiveRetriever
 
 __all__ = [
     "VectorIndexRetriever",
     "VectorIndexAutoRetriever",
     "ListIndexEmbeddingRetriever",
     "ListIndexRetriever",
     "KGTableRetriever",
@@ -28,8 +29,9 @@
     "TreeAllLeafRetriever",
     "TreeSelectLeafEmbeddingRetriever",
     "TreeSelectLeafRetriever",
     "TreeRootRetriever",
     "TransformRetriever",
     "KeywordTableSimpleRetriever",
     "BaseRetriever",
+    "RecursiveRetriever",
 ]
```

### Comparing `llama_index-0.7.0/llama_index/retrievers/transform_retriever.py` & `llama_index-0.7.1/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/schema.py` & `llama_index-0.7.1/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/selectors/llm_selectors.py` & `llama_index-0.7.1/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/selectors/prompts.py` & `llama_index-0.7.1/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/selectors/pydantic_selectors.py` & `llama_index-0.7.1/llama_index/selectors/pydantic_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/selectors/types.py` & `llama_index-0.7.1/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/docstore/__init__.py` & `llama_index-0.7.1/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/docstore/dynamodb_docstore.py` & `llama_index-0.7.1/llama_index/storage/docstore/dynamodb_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.7.1/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.7.1/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/docstore/redis_docstore.py` & `llama_index-0.7.1/llama_index/storage/docstore/redis_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/docstore/registry.py` & `llama_index-0.7.1/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.7.1/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/docstore/types.py` & `llama_index-0.7.1/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/docstore/utils.py` & `llama_index-0.7.1/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/index_store/dynamodb_index_store.py` & `llama_index-0.7.1/llama_index/storage/index_store/dynamodb_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.7.1/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.7.1/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/index_store/redis_index_store.py` & `llama_index-0.7.1/llama_index/storage/index_store/redis_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.7.1/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/index_store/types.py` & `llama_index-0.7.1/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/index_store/utils.py` & `llama_index-0.7.1/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/kvstore/dynamodb_kvstore.py` & `llama_index-0.7.1/llama_index/storage/kvstore/dynamodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.7.1/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/kvstore/redis_kvstore.py` & `llama_index-0.7.1/llama_index/storage/kvstore/redis_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/kvstore/s3_kvstore.py` & `llama_index-0.7.1/llama_index/storage/kvstore/s3_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.7.1/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/kvstore/types.py` & `llama_index-0.7.1/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/storage/storage_context.py` & `llama_index-0.7.1/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.7.1/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/token_counter/utils.py` & `llama_index-0.7.1/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tools/function_tool.py` & `llama_index-0.7.1/llama_index/tools/function_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tools/ondemand_loader_tool.py` & `llama_index-0.7.1/llama_index/tools/ondemand_loader_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tools/query_engine.py` & `llama_index-0.7.1/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tools/query_plan.py` & `llama_index-0.7.1/llama_index/tools/query_plan.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tools/tool_spec/base.py` & `llama_index-0.7.1/llama_index/tools/tool_spec/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tools/tool_spec/notion/base.py` & `llama_index-0.7.1/llama_index/tools/tool_spec/notion/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tools/tool_spec/slack/base.py` & `llama_index-0.7.1/llama_index/tools/tool_spec/slack/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tools/types.py` & `llama_index-0.7.1/llama_index/tools/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tools/utils.py` & `llama_index-0.7.1/llama_index/tools/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tts/bark.py` & `llama_index-0.7.1/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tts/base.py` & `llama_index-0.7.1/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/tts/elevenlabs.py` & `llama_index-0.7.1/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/types.py` & `llama_index-0.7.1/llama_index/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/utils.py` & `llama_index-0.7.1/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/__init__.py` & `llama_index-0.7.1/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.7.1/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/chroma.py` & `llama_index-0.7.1/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/deeplake.py` & `llama_index-0.7.1/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/docarray/base.py` & `llama_index-0.7.1/llama_index/vector_stores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/docarray/hnsw.py` & `llama_index-0.7.1/llama_index/vector_stores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/docarray/in_memory.py` & `llama_index-0.7.1/llama_index/vector_stores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/dynamodb.py` & `llama_index-0.7.1/llama_index/vector_stores/dynamodb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/faiss.py` & `llama_index-0.7.1/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/lancedb.py` & `llama_index-0.7.1/llama_index/vector_stores/lancedb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/metal.py` & `llama_index-0.7.1/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/milvus.py` & `llama_index-0.7.1/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/mongodb.py` & `llama_index-0.7.1/llama_index/vector_stores/mongodb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/myscale.py` & `llama_index-0.7.1/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/opensearch.py` & `llama_index-0.7.1/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/pinecone.py` & `llama_index-0.7.1/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/postgres.py` & `llama_index-0.7.1/llama_index/vector_stores/postgres.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/qdrant.py` & `llama_index-0.7.1/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/redis.py` & `llama_index-0.7.1/llama_index/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/registry.py` & `llama_index-0.7.1/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/simple.py` & `llama_index-0.7.1/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/supabase.py` & `llama_index-0.7.1/llama_index/vector_stores/supabase.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/tair.py` & `llama_index-0.7.1/llama_index/vector_stores/tair.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/types.py` & `llama_index-0.7.1/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/typesense.py` & `llama_index-0.7.1/llama_index/vector_stores/typesense.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/utils.py` & `llama_index-0.7.1/llama_index/vector_stores/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/weaviate.py` & `llama_index-0.7.1/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index/vector_stores/weaviate_utils.py` & `llama_index-0.7.1/llama_index/vector_stores/weaviate_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/llama_index.egg-info/PKG-INFO` & `llama_index-0.7.1/llama_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index
-Version: 0.7.0
+Version: 0.7.1
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 Author: Jerry Liu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `llama_index-0.7.0/llama_index.egg-info/SOURCES.txt` & `llama_index-0.7.1/llama_index.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -303,14 +303,15 @@
 llama_index/response_synthesizers/factory.py
 llama_index/response_synthesizers/generation.py
 llama_index/response_synthesizers/refine.py
 llama_index/response_synthesizers/simple_summarize.py
 llama_index/response_synthesizers/tree_summarize.py
 llama_index/response_synthesizers/type.py
 llama_index/retrievers/__init__.py
+llama_index/retrievers/recursive_retriever.py
 llama_index/retrievers/transform_retriever.py
 llama_index/selectors/__init__.py
 llama_index/selectors/llm_selectors.py
 llama_index/selectors/prompts.py
 llama_index/selectors/pydantic_selectors.py
 llama_index/selectors/types.py
 llama_index/storage/__init__.py
```

### Comparing `llama_index-0.7.0/setup.py` & `llama_index-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/callbacks/test_llama_debug.py` & `llama_index-0.7.1/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/callbacks/test_token_counter.py` & `llama_index-0.7.1/tests/callbacks/test_token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/chat_engine/test_condense_question.py` & `llama_index-0.7.1/tests/chat_engine/test_condense_question.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/chat_engine/test_simple.py` & `llama_index-0.7.1/tests/chat_engine/test_simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/conftest.py` & `llama_index-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/embeddings/test_base.py` & `llama_index-0.7.1/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/composability/test_utils.py` & `llama_index-0.7.1/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/conftest.py` & `llama_index-0.7.1/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/document_summary/test_index.py` & `llama_index-0.7.1/tests/indices/document_summary/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/empty/test_base.py` & `llama_index-0.7.1/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/keyword_table/test_base.py` & `llama_index-0.7.1/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/keyword_table/test_retrievers.py` & `llama_index-0.7.1/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/keyword_table/test_utils.py` & `llama_index-0.7.1/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/knowledge_graph/test_base.py` & `llama_index-0.7.1/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/knowledge_graph/test_retrievers.py` & `llama_index-0.7.1/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/list/test_index.py` & `llama_index-0.7.1/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/list/test_retrievers.py` & `llama_index-0.7.1/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/postprocessor/test_base.py` & `llama_index-0.7.1/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/postprocessor/test_llm_rerank.py` & `llama_index-0.7.1/tests/indices/postprocessor/test_llm_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/postprocessor/test_optimizer.py` & `llama_index-0.7.1/tests/indices/postprocessor/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/query/conftest.py` & `llama_index-0.7.1/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/query/query_transform/test_base.py` & `llama_index-0.7.1/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/query/test_compose.py` & `llama_index-0.7.1/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/query/test_compose_vector.py` & `llama_index-0.7.1/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/query/test_embedding_utils.py` & `llama_index-0.7.1/tests/indices/query/test_embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/query/test_query_bundle.py` & `llama_index-0.7.1/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/struct_store/conftest.py` & `llama_index-0.7.1/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/struct_store/test_base.py` & `llama_index-0.7.1/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/struct_store/test_json_query.py` & `llama_index-0.7.1/tests/indices/struct_store/test_json_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/struct_store/test_sql_query.py` & `llama_index-0.7.1/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/test_loading.py` & `llama_index-0.7.1/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/test_loading_graph.py` & `llama_index-0.7.1/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/test_node_utils.py` & `llama_index-0.7.1/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/test_prompt_helper.py` & `llama_index-0.7.1/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/tree/conftest.py` & `llama_index-0.7.1/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/tree/test_embedding_retriever.py` & `llama_index-0.7.1/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/tree/test_index.py` & `llama_index-0.7.1/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/tree/test_retrievers.py` & `llama_index-0.7.1/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/auto_retriever/test_output_parser.py` & `llama_index-0.7.1/tests/indices/vector_store/auto_retriever/test_output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/conftest.py` & `llama_index-0.7.1/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/mock_faiss.py` & `llama_index-0.7.1/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/mock_services.py` & `llama_index-0.7.1/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/test_faiss.py` & `llama_index-0.7.1/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/test_myscale.py` & `llama_index-0.7.1/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/test_pinecone.py` & `llama_index-0.7.1/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/test_retrievers.py` & `llama_index-0.7.1/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/test_simple.py` & `llama_index-0.7.1/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/indices/vector_store/utils.py` & `llama_index-0.7.1/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/langchain_helpers/test_text_splitter.py` & `llama_index-0.7.1/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/llm_predictor/test_base.py` & `llama_index-0.7.1/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/llm_predictor/vellum/conftest.py` & `llama_index-0.7.1/tests/llm_predictor/vellum/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/llm_predictor/vellum/test_predictor.py` & `llama_index-0.7.1/tests/llm_predictor/vellum/test_predictor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/llm_predictor/vellum/test_prompt_registry.py` & `llama_index-0.7.1/tests/llm_predictor/vellum/test_prompt_registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/llms/test_custom.py` & `llama_index-0.7.1/tests/llms/test_custom.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/llms/test_openai.py` & `llama_index-0.7.1/tests/llms/test_openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/llms/test_openai_utils.py` & `llama_index-0.7.1/tests/llms/test_openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/llms/test_palm.py` & `llama_index-0.7.1/tests/llms/test_palm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/logger/test_base.py` & `llama_index-0.7.1/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/mock_utils/mock_predict.py` & `llama_index-0.7.1/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/mock_utils/mock_prompts.py` & `llama_index-0.7.1/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/mock_utils/mock_text_splitter.py` & `llama_index-0.7.1/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/mock_utils/mock_utils.py` & `llama_index-0.7.1/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/objects/test_base.py` & `llama_index-0.7.1/tests/objects/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/objects/test_node_mapping.py` & `llama_index-0.7.1/tests/objects/test_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/output_parsers/test_base.py` & `llama_index-0.7.1/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/output_parsers/test_pydantic.py` & `llama_index-0.7.1/tests/output_parsers/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/output_parsers/test_selection.py` & `llama_index-0.7.1/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/playground/test_base.py` & `llama_index-0.7.1/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/program/test_guidance.py` & `llama_index-0.7.1/tests/program/test_guidance.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/program/test_llm_program.py` & `llama_index-0.7.1/tests/program/test_llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/prompts/test_base.py` & `llama_index-0.7.1/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/prompts/test_guidance_utils.py` & `llama_index-0.7.1/tests/prompts/test_guidance_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/question_gen/test_guidance_generator.py` & `llama_index-0.7.1/tests/question_gen/test_guidance_generator.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/question_gen/test_llm_generators.py` & `llama_index-0.7.1/tests/question_gen/test_llm_generators.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/readers/test_file.py` & `llama_index-0.7.1/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/readers/test_json.py` & `llama_index-0.7.1/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/readers/test_mongo.py` & `llama_index-0.7.1/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/selectors/test_llm_selectors.py` & `llama_index-0.7.1/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/storage/conftest.py` & `llama_index-0.7.1/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/storage/docstore/test_dynamodb_docstore.py` & `llama_index-0.7.1/tests/storage/docstore/test_dynamodb_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/storage/docstore/test_mongo_docstore.py` & `llama_index-0.7.1/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/storage/docstore/test_redis_docstore.py` & `llama_index-0.7.1/tests/storage/docstore/test_redis_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/storage/docstore/test_simple_docstore.py` & `llama_index-0.7.1/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/storage/test_storage_context.py` & `llama_index-0.7.1/tests/storage/test_storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/test_utils.py` & `llama_index-0.7.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/token_predictor/test_base.py` & `llama_index-0.7.1/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/tools/test_base.py` & `llama_index-0.7.1/tests/tools/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/tools/test_ondemand_loader.py` & `llama_index-0.7.1/tests/tools/test_ondemand_loader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/tools/test_utils.py` & `llama_index-0.7.1/tests/tools/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/tools/tool_spec/test_base.py` & `llama_index-0.7.1/tests/tools/tool_spec/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/vector_stores/test_docarray.py` & `llama_index-0.7.1/tests/vector_stores/test_docarray.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/vector_stores/test_postgres.py` & `llama_index-0.7.1/tests/vector_stores/test_postgres.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/vector_stores/test_qdrant.py` & `llama_index-0.7.1/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/vector_stores/test_tair.py` & `llama_index-0.7.1/tests/vector_stores/test_tair.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.0/tests/vector_stores/test_weaviate.py` & `llama_index-0.7.1/tests/vector_stores/test_weaviate.py`

 * *Files identical despite different names*

