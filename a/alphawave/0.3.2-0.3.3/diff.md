# Comparing `tmp/alphawave-0.3.2.tar.gz` & `tmp/alphawave-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.3.2.tar", last modified: Tue Jul  4 21:26:32 2023, max compression
+gzip compressed data, was "alphawave-0.3.3.tar", last modified: Thu Jul  6 04:03:31 2023, max compression
```

## Comparing `alphawave-0.3.2.tar` & `alphawave-0.3.3.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 21:26:32.964718 alphawave-0.3.2/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.2/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-04 21:26:32.964718 alphawave-0.3.2/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.2/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1006 2023-07-04 21:26:22.000000 alphawave-0.3.2/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-04 21:26:32.964718 alphawave-0.3.2/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 21:26:32.960718 alphawave-0.3.2/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 21:26:32.960718 alphawave-0.3.2/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10039 2023-07-04 02:40:43.000000 alphawave-0.3.2/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.2/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.2/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8159 2023-07-04 16:10:19.000000 alphawave-0.3.2/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.2/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.3.2/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8917 2023-06-30 21:13:15.000000 alphawave-0.3.2/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.3.2/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.2/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6501 2023-07-04 18:20:06.000000 alphawave-0.3.2/src/alphawave/TOMLResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.2/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.2/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.2/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.3.2/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.2/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.2/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 21:26:32.960718 alphawave-0.3.2/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-04 21:26:32.000000 alphawave-0.3.2/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1797 2023-07-04 21:26:32.000000 alphawave-0.3.2/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-04 21:26:32.000000 alphawave-0.3.2/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      191 2023-07-04 21:26:32.000000 alphawave-0.3.2/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-04 21:26:32.000000 alphawave-0.3.2/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 21:26:32.964718 alphawave-0.3.2/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    16350 2023-07-04 18:23:32.000000 alphawave-0.3.2/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1645 2023-07-04 15:32:04.000000 alphawave-0.3.2/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7199 2023-07-04 18:19:22.000000 alphawave-0.3.2/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-06-30 18:31:20.000000 alphawave-0.3.2/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.2/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.2/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-01 22:34:34.000000 alphawave-0.3.2/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1507 2023-07-01 23:27:46.000000 alphawave-0.3.2/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3239 2023-06-30 02:09:36.000000 alphawave-0.3.2/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7943 2023-07-04 16:11:01.000000 alphawave-0.3.2/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.2/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.2/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.2/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2035 2023-07-04 17:32:53.000000 alphawave-0.3.2/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 21:26:32.964718 alphawave-0.3.2/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.2/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7792 2023-06-28 22:49:13.000000 alphawave-0.3.2/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2731 2023-07-03 19:26:44.000000 alphawave-0.3.2/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.2/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.2/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    23933 2023-06-29 21:03:58.000000 alphawave-0.3.2/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.2/src/alphawave_pyexts/handler.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 21:26:32.964718 alphawave-0.3.2/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14219 2023-07-04 18:53:15.000000 alphawave-0.3.2/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1029 2023-07-03 20:25:17.000000 alphawave-0.3.2/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.2/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.2/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6901 2023-07-03 18:25:59.000000 alphawave-0.3.2/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 21:26:32.964718 alphawave-0.3.2/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.2/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.2/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.3.2/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 04:03:31.380242 alphawave-0.3.3/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.3/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-06 04:03:31.380242 alphawave-0.3.3/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.3/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1006 2023-07-06 04:03:23.000000 alphawave-0.3.3/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-06 04:03:31.380242 alphawave-0.3.3/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 04:03:31.376242 alphawave-0.3.3/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 04:03:31.376242 alphawave-0.3.3/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10108 2023-07-05 02:11:57.000000 alphawave-0.3.3/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.3/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.3/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8186 2023-07-06 03:49:40.000000 alphawave-0.3.3/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.3/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.3.3/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8917 2023-06-30 21:13:15.000000 alphawave-0.3.3/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.3.3/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.3/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6501 2023-07-04 18:20:06.000000 alphawave-0.3.3/src/alphawave/TOMLResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.3/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.3/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.3/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.3.3/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.3/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.3/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 04:03:31.376242 alphawave-0.3.3/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-06 04:03:31.000000 alphawave-0.3.3/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1777 2023-07-06 04:03:31.000000 alphawave-0.3.3/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-06 04:03:31.000000 alphawave-0.3.3/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      191 2023-07-06 04:03:31.000000 alphawave-0.3.3/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-06 04:03:31.000000 alphawave-0.3.3/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 04:03:31.380242 alphawave-0.3.3/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    16573 2023-07-06 03:45:52.000000 alphawave-0.3.3/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1721 2023-07-05 23:26:34.000000 alphawave-0.3.3/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7208 2023-07-06 03:36:16.000000 alphawave-0.3.3/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-06-30 18:31:20.000000 alphawave-0.3.3/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.3/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.3/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-01 22:34:34.000000 alphawave-0.3.3/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-05 23:30:15.000000 alphawave-0.3.3/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3239 2023-06-30 02:09:36.000000 alphawave-0.3.3/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7944 2023-07-05 23:46:12.000000 alphawave-0.3.3/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.3/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.3/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.3/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.3/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 04:03:31.380242 alphawave-0.3.3/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.3/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6391 2023-07-05 18:56:38.000000 alphawave-0.3.3/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2731 2023-07-03 19:26:44.000000 alphawave-0.3.3/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.3/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.3/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    22234 2023-07-05 22:51:49.000000 alphawave-0.3.3/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.3/src/alphawave_pyexts/handler.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 04:03:31.380242 alphawave-0.3.3/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14219 2023-07-04 18:53:15.000000 alphawave-0.3.3/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1029 2023-07-03 20:25:17.000000 alphawave-0.3.3/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.3/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.3/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6901 2023-07-03 18:25:59.000000 alphawave-0.3.3/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 04:03:31.380242 alphawave-0.3.3/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.3/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.3/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.3.2/LICENSE` & `alphawave-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/PKG-INFO` & `alphawave-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.2
+Version: 0.3.3
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.2/README.md` & `alphawave-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/pyproject.toml` & `alphawave-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave-py - Functions for smaller Large Language Models (sLLMs)"
```

### Comparing `alphawave-0.3.2/src/alphawave/AlphaWave.py` & `alphawave-0.3.3/src/alphawave/AlphaWave.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
             if validation['valid']:
                 if 'value' in validation:
                     response['message']['content'] = validation['value']
                     #print(f"***** Alphawave post validation picking up value {response}\n note response['message']['content'] must exist!")
         
                 self.addInputToHistory(memory, history_variable, input)
                 self.addResponseToHistory(memory, history_variable, response['message'])
+                print(f"***** Alphawave added response to history ")
                 return response
 
             if self.options.logRepairs:
                 print(Colorize.title('REPAIRING RESPONSE:'))
                 print(Colorize.output(memory))
             fork = MemoryFork(memory)
             #self.addInputToHistory(fork, history_variable, input)
```

### Comparing `alphawave-0.3.2/src/alphawave/Colorize.py` & `alphawave-0.3.3/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.3.3/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/JSONResponseValidator.py` & `alphawave-0.3.3/src/alphawave/JSONResponseValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     if p:
         pass #print(json.dumps(template))
     return json.dumps(template)
 
 class JSONResponseValidator(PromptResponseValidator):
     def __init__(self, schema=None, missing_json_feedback='Invalid JSON. return valid JSON.'):
         self.schema = schema
+        print(self.schema)
         self.missing_json_feedback = missing_json_feedback
 
     def parse_dict(self, s):
         if s is None:
             return s
         # Try to parse as JSON
         # Try to repair common errors and parse again
```

### Comparing `alphawave-0.3.2/src/alphawave/MemoryFork.py` & `alphawave-0.3.3/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/OSClient.py` & `alphawave-0.3.3/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/OpenAIClient.py` & `alphawave-0.3.3/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/RepairTestClient.py` & `alphawave-0.3.3/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/Response.py` & `alphawave-0.3.3/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/TOMLResponseValidator.py` & `alphawave-0.3.3/src/alphawave/TOMLResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/TestClient.py` & `alphawave-0.3.3/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/TestClientTest.py` & `alphawave-0.3.3/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/alphawaveTypes.py` & `alphawave-0.3.3/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/internalTypes.py` & `alphawave-0.3.3/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave/jsonParser.py` & `alphawave-0.3.3/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.3.3/src/alphawave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.2
+Version: 0.3.3
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.2/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.3.3/src/alphawave.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,9 +45,8 @@
 src/alphawave_pyexts/handler.py
 src/alphawave_pyexts/modelling_RW.py
 src/alphawave_pyexts/serverUtils.py
 src/alphawave_pyexts/utilityV2.py
 src/alphawave_pyexts/llmsearch/google_search_concurrent.py
 src/alphawave_pyexts/llmsearch/search_service.py
 tests/testOSClient.py
-tests/testOpenAiClient.py
-tests/testSchema.py
+tests/testOpenAiClient.py
```

### Comparing `alphawave-0.3.2/src/alphawave_agents/Agent.py` & `alphawave-0.3.3/src/alphawave_agents/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,30 +92,46 @@
     for key, value in source.items():
         if key in instance and value is not None:
             instance[key] =  value
 
 ##
 PromptInstructionSectionJSON = TemplateSection(\
 """
-Reason about the user query following these instructions.
-If the answer is available from fact or reasoning, respond with the answer using the finalAnswer command
-Otherwise, reason step by step about the query, the available information, and the set of commands listed earlier, and select a command to perform.
-The ONLY commands available are the commands listed.
-Return a JSON object with your reasoning and the next command to perform, with arguments, using the format shown above for that command
-"""
-                                              , 'system')
+Reason step-by-step about the user task:
+1. Develop a concise plan for finding an answer and showing it to the user. Base your plan on known fact, reasoning, and the available commands.
+2. Select the first step of that plan as the next command to perform. 
+3. Respond with:
+  - your reasoning 
+  - the JSONformat shown above for that next command, instantiating actual inputs where indicated
+""", 'system')
+PromptOneShotJSON = [
+    UserMessage("What is 35 * 64?"),
+    AssistantMessage("""I will use the math command.
+{"command": "math", "inputs":{"code":"35*64"}}""")]
+
 
 PromptInstructionSectionTOML = TemplateSection(\
 """
-Reason about the user query following these instructions.
-If the answer is available from fact or reasoning, respond with the answer using the finalAnswer command.
-Otherwise, reason step by step about the query, the available information, and the set of commands listed above, and select a command to perform.
-Return your reasoning and the next command to perform, with arguments, using the format provided above for that command.
-"""
-                                              , 'system')
+Reason step-by-step about the user task:
+1. Develop a concise plan for finding an answer and showing it to the user. Base your plan on known fact, reasoning, and the available commands.
+2. Select the first step of that plan as the next command to perform. 
+3. Respond with:
+  - your reasoning 
+  - the JSONformat shown above for that next command, substituting your inputs where indicated
+""", 'system')
+
+PromptOneShotTOML = [
+    UserMessage("What is 35 * 64?"),
+    AssistantMessage("""I will use the math command.
+[RESPONSE]
+command = "math"
+inputs.code = "35*64"
+[STOP]
+""")]
+
 
 @dataclass
 class AgentCommandInput:
     agentId: str
     input: str
 
 
@@ -272,18 +288,21 @@
             history_variable = self.get_agent_history_variable(agent_id)
             try:
                 sections = [agent_prompt]
                 sections.append(AgentCommandSection(self._commands, one_shot=True, syntax=self._options['syntax']))
                 
                 if self._options['syntax'] == 'JSON':
                     pis = PromptInstructionSectionJSON
+                    pos = PromptOneShotJSON
                 else:
                     pis = PromptInstructionSectionTOML
+                    pos = PromptOneShotTOML
                     
                 sections.append(pis)
+                sections.extend(pos)
                 prompt = Prompt([
                     GroupSection(sections, 'system'),
                     ConversationHistory(history_variable, 1.0, True)
                 ])
                 if input:
                     prompt.sections.append(TextSection(input, 'user', -1, True, '\n', 'user'))
                     # Ensure input variable is set otherwise the history will be wrong.
```

### Comparing `alphawave-0.3.2/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.3.3/src/alphawave_agents/AgentCommandSection.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,24 @@
         self.tokens = tokens
         self.required = required
         self.one_shot = one_shot
         self.syntax = syntax
         
     async def renderAsMessages(self, memory: Any, functions: Any, tokenizer: Any, max_tokens: int) -> Dict[str, Any]:
         # Render commands to message content
-        content = 'commands:\n'
+        content = 'You have the following  commands available in addition to known facts and reasoning:\n'
         for command in self._commands.values():
             content += f'\t{command.title}:\n'
             content += f'\t\tuse: {command.description}\n'
-            if command.inputs:
-                content += f'\t\tinputs: {command.inputs}\n'
-            if command.output:
-                content += f'\t\toutput: {command.output}\n'
-            if self.one_shot:
-                content += command.one_shot(self.syntax)
+            #if command.inputs:
+            #    content += f'\t\tinputs: {command.inputs}\n'
+            #if command.output:
+            #    content += f'\t\toutput: {command.output}\n'
+            #if self.one_shot:
+            content += command.one_shot(self.syntax)
         # Return as system message
         result = None
         try:
             length = len(tokenizer.encode(content))
             result = self.return_messages([{'role': 'system', 'content': content}], length, tokenizer, max_tokens)
         except Exception as e:
             traceback.print_exc()
```

### Comparing `alphawave-0.3.2/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.3.3/src/alphawave_agents/AgentCommandValidator.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from promptrix.VolatileMemory import VolatileMemory
 from promptrix.Utilities import Utilities
 from alphawave.alphawaveTypes import PromptCompletionOptions
 from alphawave.JSONResponseValidator import JSONResponseValidator
 from alphawave.TOMLResponseValidator import TOMLResponseValidator
 from alphawave.Response import Response
 from alphawave.AlphaWave import AlphaWave, AlphaWaveOptions
+from alphawave.MemoryFork import MemoryFork
 from alphawave_agents.agentTypes import Command, AgentThought, AgentThoughtSchemaJSON, AgentThoughtSchemaTOML
 from alphawave_agents.MathCommand import MathCommand
 import traceback
 
 
 class AgentCommandValidator:
     def __init__(self, commands: dict[str, Command], client=None, model: str='', syntax:str='JSON',
@@ -26,18 +27,18 @@
         self._model = model
         self._client = client
         self._syntax = syntax
         self._memory=memory
         self._history_variable = history_variable
         
         if syntax == 'JSON':
-            self._input_validator = JSONResponseValidator(AgentThoughtSchemaJSON, 'No valid JSON objects were found in the response. Return a valid JSON object with reasoning, and the next command to use.')
+            self._input_validator = JSONResponseValidator(AgentThoughtSchemaJSON, 'No valid command was found in the response. Respond using a completed instance of the specified template for the next command.')
         else:
             #print(f"***** AgentCommandValidator creating TOML")
-            self._input_validator = TOMLResponseValidator(AgentThoughtSchemaTOML, 'I do not understand. return requested format with reasoning and next command to use.')
+            self._input_validator = TOMLResponseValidator(AgentThoughtSchemaTOML, 'No valid command was found. Respond using an instantiation of the specified template for the next command.')
 
         self._commands = commands
 
     async def validate_response(self, memory, functions, tokenizer, response, remaining_attempts) -> Union[AgentThought, None]:
         # Validate that the response contains a thought
         try:
           #print(f"***** AgentCommandValidator validate syntax: \n{self._syntax}\nresponse\n{response}")
@@ -68,67 +69,65 @@
                   'valid': False,
                   'feedback': f'The command {command_name} does not exist. The only commands you have are {list(self._commands.keys())}'
               }
           
           # Validate that the command input is valid
           command = self._commands[command_name]
           command_validation_result = await command.validate(thought['inputs'] or {}, memory, functions, tokenizer, syntax = self._syntax)
-          if not command_validation_result['valid']:
-              #print(f"***** AgentCommandValidator command.validate fail, trying repair {command_validation_result}")
-              try:
-                  command_validation_retry =  await self.repair_args(command, thought['inputs'] or {})
-              except Exception as e:
-                  traceback.print_exc()
-                  raise e
-              #print(f"***** AgentCommandValidator command.validate repair {command_validation_retry}")
-              if command_validation_retry['status'] == 'success':
-                  validation_result['value']['inputs'] = command_validation_result['value']
-              else:
-                  return command_validation_result
-              
-          #print(f"***** AgentCommandValidator command validation success\n{command_validation_result['value']}")
-          validation_result['value']['inputs'] = command_validation_result['value']
-          return validation_result
+          if command_validation_result['valid']:
+              print(f"***** AgentCommandValidator command validation success\n{command_validation_result}\n")
+              #validation_result['value']['inputs'] = command_validation_result['value']
+              return validation_result
+          else:
+            return {
+                'type': 'Validation',
+                'valid': False,
+                'feedback': 'The command '+thought['command'] +' inputs were missing or malformed. Provide them in this format:\n'
+                +command.one_shot(self._syntax)+'\n, substituting actual values for command inputs\n'
+                }
+
         except Exception as e:
             traceback.print_exc()
             return {
                 'type': 'Validation',
                 'valid': False,
                 'feedback': f'The command validation failed. try again {str(e)}'
                 }
-        #print(f"***** AgentCommandValidator generic exit fail {thought['command']['name']}")
+        print(f"***** AgentCommandValidator generic exit fail {thought['command']['name']}")
         return {
             'type': 'Validation',
             'valid': False,
-            'feedback': 'The command '+thought['command'] +' inputs were missing or malformed. Provide them in this format:\n'
-            +command.one_shot(self._syntax)+'\n, substituting actual values for command inputs\n'
-        }
-
-    async def repair_args(self, command, fail_args):
-        #print(f"***** AgentCommandValidator recovery attempt ")
-        args_validator = JSONResponseValidator(command.schema, "invalid command args syntax, use: {command.schema}")
+            'feedback': f'The command validation failed. try again {str(e)}'
+                }
 
+    async def repair_args(self, command, fail_thought):
+        #print(f"***** AgentCommandValidator recovery attempt keys {list(self._memory._memory.keys())}")
+        args_validator = JSONResponseValidator(command.schema, "invalid command inputs syntax, use: {command.one_shot()\n}")
+        fork = MemoryFork(self._memory)
         prompt_options=PromptCompletionOptions(completion_type='chat', model=self._model, temperature=0.1)
-        args_prompt=Prompt([ConversationHistory('history'),
+        args_prompt=Prompt([ConversationHistory(self._history_variable),
                             UserMessage(f'invalid command args: {fail_args}, repair using this format: {command.schema["properties"]}')])
-    
-        wave = AlphaWave(client=self._client, prompt=args_prompt, prompt_options=prompt_options, memory=self._memory)
-        #print(f"***** AgentCommandValidator recovery attempt ")
+        print(f"***** AgentCommandValidator recovery attempt wave built\ninvalid command args: {fail_args}, repair using this format: {command.schema['properties']}")
+        wave = AlphaWave(client=self._client, prompt=args_prompt, prompt_options=prompt_options, memory=fork)
+        print(f"***** AgentCommandValidator recovery attempt wave built")
+        args = None
         try:
             args = await wave.completePrompt()
+            print(f"***** AgentCommandValidator recovery wave result {args}")
         except Exception as e:
             traceback.print_exc()
-        #print(f'***** recovery result {args}')
+        print(f'***** recovery result {args}')
         if args:
             return args
-        return command_validation_result
+        print(f"***** AgentCommandValidator recovery returning fail_args {fail_args}")
+        return fail_args
 
 
 from alphawave.OSClient import OSClient
 
 if __name__ == '__main__':
     memory=VolatileMemory()
-    memory.set('history', {'role': 'assistant', 'content': {"reasoning":"use math", "command":{"name":"math", "inputs":{"abc":"xyz"}}}})
+    memory.set('history', {'role': 'assistant', 'content': {"command":{"name":"math", "inputs":{"abc":"xyz"}}}})
     acv = AgentCommandValidator(commands={"math":MathCommand()}, client=OSClient(logRequests=True), model='vicuna_v1.1', syntax='JSON', memory=memory)
     #print('acv created')
     result = asyncio.run(acv.repair_args(MathCommand(), {'abc':'xyz'}))
     #print(result)
```

### Comparing `alphawave-0.3.2/src/alphawave_agents/AskCommand.py` & `alphawave-0.3.3/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.3.3/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.3.3/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.3.3/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_agents/MathCommand.py` & `alphawave-0.3.3/src/alphawave_agents/MathCommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 @dataclass
 class MathCommandInput:
     code:str
 
 schema = CommandSchema(
     schema_type="object",
     title="math",
-    description="execute some python code to calculate a value",
+    description="evaluate a mathematical expression to calculate its value",
     properties={
         "code": {
             "type": "string",
-            "description": "python expression to evaluate"
+            "description": "expression to evaluate"
         }
     },
     required=["code"],
     returns="the calculated value"
 )
 
 class MathCommand(SchemaBasedCommand):
```

### Comparing `alphawave-0.3.2/src/alphawave_agents/PromptCommand.py` & `alphawave-0.3.3/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.3.3/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files 8% similar despite different names*

```diff
@@ -161,24 +161,26 @@
                 pass
 
         return cleaned
 
     def one_shot(self, syntax):
         content=''
         if syntax == 'JSON':
-            content += '\t\tformat: {'+f'"reasoning":"<concise reasons to use {self.title}>","command":'+f'"{self.title}", "inputs":'+'{'
+            content += '\t\tformat: {'+f'"command":'+f'"{self.title}", "inputs":'+'{'
             args = ''
             for arg in self.inputs.split(','):
-                key = (arg.split(':'))[0].strip().strip('"\'') # strip key down to bare alpha key (':' elims type info)
-                content += f'"{key}": "<value for {key}>",'
+                arg_key_dscp = arg.split(':')
+                key = arg_key_dscp[0].strip().strip('"\'') # strip key down to bare alpha key (':' elims type info)
+                content += f'"{key}": "<{arg_key_dscp[1].strip()}>",'
                 content = content[:-1]+'}}\n' # strip final comma 
             #print(f'***** AgentCommandSection one-shot prompt: {content}\n')
             return content
         else:
-            content += f'\t\tformat:\n[RESPONSE]\nreasoning="<concise reasons to use {self.title}>"\ncommand="{self.title}"\n'
+            content += f'\t\tformat:\n[RESPONSE]\ncommand="{self.title}"\n'
             args = ''
             for arg in self.inputs.split(','):
-                key = 'inputs.'+(arg.split(':'))[0].strip().strip('"\'') # strip key down to bare alpha key (':' elims type info)
-                content += f'{key}="<value for {key}>"\n'
+                arg_key_dscp = arg.split(':')
+                key = 'inputs.'+arg_key_dscp[0].strip().strip('"\'') # strip key down to bare alpha key (':' elims type info)
+                content += f'{key}="<{arg_key_dscp[1].strip()}>"\n'
                 content +='[STOP]\n'
             #print(f'***** AgentCommandSection one-shot TOML: {content}\n')
             return content
```

### Comparing `alphawave-0.3.2/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.3.3/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.3.3/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_agents/agentTypes.py` & `alphawave-0.3.3/src/alphawave_agents/agentTypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,27 +30,21 @@
 class AgentThought:
     thoughts: Dict[str, str]
     command: Dict[str, Any]
 
 AgentThoughtSchemaJSON: Dict[str,str] = {
     "type": "object",
     "properties": {
-        "reasoning": {"type": "string"},
         "command": {"type": "string"},
         "inputs": {"type": "object"},
     },
-    "required": ["reasoning", "command"]
+    "required": ["command"]
 }
 
 AgentThoughtSchemaTOML = {
-    "reasoning": {
-        "type":"string",
-        "meta":"<reasoning about user task>",
-        "required": True
-    },
     "command": {
         "type":"string",
         "meta":"<selected command>",
         "required":True
     },
     "inputs":{
         "type":"dict",
```

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/FsInference.py` & `alphawave-0.3.3/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.3.3/src/alphawave_pyexts/LLMClient.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,66 +13,14 @@
 USER_PREFIX = 'user'
 ASSISTANT_PREFIX = 'assistant'
 SYSTEM_PREFIX = 'system'
 
 host='192.168.1.195'
 port = 5004
 
-cv.register_conv_template(
-    Conversation(
-        name="falcon_instruct",
-        system="",
-        roles=("User", "Assistant"),
-        messages=(),
-        offset=0,
-        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
-        stop_str=["User:", "Assistant:"],
-        stop_token_ids=[11],
-        sep="\n",
-        sep2="<|endoftext|>",
-        first_msg_no_role=False,
-    )
-)
-cv.register_conv_template(Conversation(
-        name="guanaco",
-        system="",
-        roles=("Human", "Assistant"),
-        messages=(),
-        offset=0,
-        sep_style=SeparatorStyle.ADD_COLON_TWO,
-        sep="\n",
-        sep2="",
-    )
-)
-cv.register_conv_template(Conversation(
-        name="wizardLM",
-        system="""Below is an instruction that describes a task. Write a response that appropriately completes the request.
-### Instruction
-""",
-        roles=("### Input", "### Response"),
-        messages=(),
-        offset=0,
-        sep_style=SeparatorStyle.ADD_COLON_TWO,
-        sep="\n",
-        sep2="\n",
-    )
-)
-cv.register_conv_template(Conversation(
-        name="wizardLM2",
-        system="""Below is an instruction that describes a task. Write a response that appropriately completes the request.
-### Instruction
-""",
-        roles=("User", "Assistant"),
-        messages=(),
-        offset=0,
-        sep_style=SeparatorStyle.ADD_COLON_TWO,
-        sep="\n",
-        sep2="\n",
-    )
-)
 
 def get_available_models():
     return list(cv.conv_templates.keys())
 
 def run_query(model, messages, max_tokens, temp, top_p, host = host, port = port, tkroot = None, tkdisplay=None, format=True): 
     global USER_PREFIX, ASSISTANT_PREFIX, SYSTEM_PREFIX
```

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.3.3/src/alphawave_pyexts/SearchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/chat.py` & `alphawave-0.3.3/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.3.3/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/handler.py` & `alphawave-0.3.3/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.3.3/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.3.3/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.3.3/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.3.3/src/alphawave_pyexts/serverUtils.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.3.3/src/alphawave_pyexts/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/tests/testOSClient.py` & `alphawave-0.3.3/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.2/tests/testOpenAiClient.py` & `alphawave-0.3.3/tests/testOpenAiClient.py`

 * *Files identical despite different names*

