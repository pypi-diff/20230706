# Comparing `tmp/gpt_fn-0.0.7.tar.gz` & `tmp/gpt_fn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_fn-0.0.7.tar", max compression
+gzip compressed data, was "gpt_fn-0.0.8.tar", max compression
```

## Comparing `gpt_fn-0.0.7.tar` & `gpt_fn-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0     1066 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/LICENSE
--rw-r--r--   0        0        0     4119 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/README.md
--rw-r--r--   0        0        0      810 2023-07-04 06:43:22.850904 gpt_fn-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/__init__.py
--rw-r--r--   0        0        0      767 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/ai_function.py
--rw-r--r--   0        0        0     4278 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/completion.py
--rw-r--r--   0        0        0      537 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/conftest.py
--rw-r--r--   0        0        0      342 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/exceptions.py
--rw-r--r--   0        0        0      878 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/prompt.py
--rw-r--r--   0        0        0        0 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/py.typed
--rw-r--r--   0        0        0        0 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/__init__.py
--rw-r--r--   0        0        0      284 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
--rw-r--r--   0        0        0     9184 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/__snapshots__/test_completion.ambr
--rw-r--r--   0        0        0      330 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
--rw-r--r--   0        0        0    13049 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
--rw-r--r--   0        0        0    15305 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
--rw-r--r--   0        0        0    13478 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0    12997 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml
--rw-r--r--   0        0        0     5955 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion.yaml
--rw-r--r--   0        0        0     3138 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion_without_enough_tokens.yaml
--rw-r--r--   0        0        0     3239 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml
--rw-r--r--   0        0        0     3892 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_structural_completion.yaml
--rw-r--r--   0        0        0     3311 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_structural_completion_without_enough_tokens.yaml
--rw-r--r--   0        0        0      872 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/tests/test_ai_function.py
--rw-r--r--   0        0        0     4151 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/tests/test_completion.py
--rw-r--r--   0        0        0      522 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/__init__.py
--rw-r--r--   0        0        0     1945 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/pydantic_parser.py
--rw-r--r--   0        0        0     3560 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/signature.py
--rw-r--r--   0        0        0        0 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/__init__.py
--rw-r--r--   0        0        0      960 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
--rw-r--r--   0        0        0    14006 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
--rw-r--r--   0        0        0      892 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/test_pydantic_parser.py
--rw-r--r--   0        0        0     2647 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/test_signature.py
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 gpt_fn-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4119 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/README.md
+-rw-r--r--   0        0        0      852 2023-07-06 05:52:36.856174 gpt_fn-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/__init__.py
+-rw-r--r--   0        0        0      767 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/ai_function.py
+-rw-r--r--   0        0        0     4278 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/completion.py
+-rw-r--r--   0        0        0      537 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/conftest.py
+-rw-r--r--   0        0        0      342 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/exceptions.py
+-rw-r--r--   0        0        0      878 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/prompt.py
+-rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/py.typed
+-rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
+-rw-r--r--   0        0        0     9184 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/__snapshots__/test_completion.ambr
+-rw-r--r--   0        0        0      330 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
+-rw-r--r--   0        0        0     3457 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
+-rw-r--r--   0        0        0     4059 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
+-rw-r--r--   0        0        0    16256 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0    15664 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml
+-rw-r--r--   0        0        0     9246 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion.yaml
+-rw-r--r--   0        0        0     6251 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion_without_enough_tokens.yaml
+-rw-r--r--   0        0        0     6530 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml
+-rw-r--r--   0        0        0     7869 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_structural_completion.yaml
+-rw-r--r--   0        0        0     6611 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_structural_completion_without_enough_tokens.yaml
+-rw-r--r--   0        0        0      872 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/test_ai_function.py
+-rw-r--r--   0        0        0     4151 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/test_completion.py
+-rw-r--r--   0        0        0      522 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/__init__.py
+-rw-r--r--   0        0        0     1951 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     3560 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/signature.py
+-rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/__init__.py
+-rw-r--r--   0        0        0     4717 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
+-rw-r--r--   0        0        0    14060 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
+-rw-r--r--   0        0        0     7162 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser_with_prompt[email.txt-Email].yaml
+-rw-r--r--   0        0        0     2186 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt
+-rw-r--r--   0        0        0     1734 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_pydantic_parser.py
+-rw-r--r--   0        0        0     2647 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_signature.py
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 gpt_fn-0.0.8/PKG-INFO
```

### Comparing `gpt_fn-0.0.7/LICENSE` & `gpt_fn-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/README.md` & `gpt_fn-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/pyproject.toml` & `gpt_fn-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-fn"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gpt_fn", from = "src" }]
 include = ["fn/py.typed"]
 
 [tool.poetry.dependencies]
@@ -15,19 +15,21 @@
 docstring-parser = "^0.15"
 
 [tool.poetry.group.test.dependencies]
 syrupy = "^4.0.2"
 pytest-vcr = "^1.0.2"
 pytest-cov = "^4.1.0"
 coveralls = "^3.3.1"
+pytest-datadir = "^1.4.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
 mkdocs-material = "^9.1.15"
 mkdocstrings = { extras = ["python"], version = "^0.22.0" }
+mypy = "^1.4.1"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 pattern = "default-unprefixed"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/ai_function.py` & `gpt_fn-0.0.8/src/gpt_fn/ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/src/gpt_fn/completion.py` & `gpt_fn-0.0.8/src/gpt_fn/completion.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/src/gpt_fn/conftest.py` & `gpt_fn-0.0.8/src/gpt_fn/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/src/gpt_fn/prompt.py` & `gpt_fn-0.0.8/src/gpt_fn/prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/__snapshots__/test_completion.ambr` & `gpt_fn-0.0.8/src/gpt_fn/tests/__snapshots__/test_completion.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml` & `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,354 +1,488 @@
 interactions:
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are now the following
-      python function:\n```\n# return fabnocci number\ndef fabnocci(n: int):\n```\nOnly
-      respond with your `return` value.\nThe output should be formatted as a JSON
-      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
-      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
-      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
-      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
-      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
-      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
-      {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```"},
-      {"role": "user", "content": "fabnocci(10)"}], "model": "gpt-3.5-turbo", "temperature":
-      0.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty": 0.0, "user":
-      "", "stop": null}'
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null, "max_tokens": 1}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '975'
+      - '283'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.7
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.7", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.8", "platform": "Linux-5.15.0-72-generic-x86_64-with-glibc2.35", "publisher":
         "openai", "uname": "Linux 5.15.0-72-generic #79-Ubuntu SMP Wed Apr 19 08:22:18
         UTC 2023 x86_64"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"id\": \"chatcmpl-7QZLqAOMdygD2B0nE7xwIlZbI5dYJ\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1686566774,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
-        \ \"usage\": {\n    \"prompt_tokens\": 199,\n    \"completion_tokens\": 6,\n
-        \   \"total_tokens\": 205\n  },\n  \"choices\": [\n    {\n      \"message\":
-        {\n        \"role\": \"assistant\",\n        \"content\": \"{\\\"ret\\\":
-        55}\"\n      },\n      \"finish_reason\": \"stop\",\n      \"index\": 0\n
-        \   }\n  ]\n}\n"
+      string: "{\n  \"id\": \"chatcmpl-7QXcyFNjAlIIPRuU5YEC6vUlqwu6R\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686560148,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
+        \ \"usage\": {\n    \"prompt_tokens\": 25,\n    \"completion_tokens\": 1,\n
+        \   \"total_tokens\": 26\n  },\n  \"choices\": [\n    {\n      \"message\":
+        {\n        \"role\": \"assistant\",\n        \"content\": \"Hello\"\n      },\n
+        \     \"finish_reason\": \"length\",\n      \"index\": 0\n    }\n  ]\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d618241afc24a1e-TPE
+      - 7d60e0820c3ba9cb-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Mon, 12 Jun 2023 10:46:14 GMT
+      - Mon, 12 Jun 2023 08:55:49 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '394'
+      - '195'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89809'
+      - '89985'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 126ms
+      - 10ms
       x-request-id:
-      - 493e1bf4e826813b9d18a2843a8f3b9b
+      - 9b24c553c430a32d49942fc89bddcd00
     status:
       code: 200
       message: OK
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are now the following
-      python function:\n```\n# return fabnocci number\ndef fabnocci(n: int):\n```\nOnly
-      respond with your `return` value.\nThe output should be formatted as a JSON
-      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
-      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
-      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
-      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
-      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
-      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
-      {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```",
-      "name": null}, {"role": "user", "content": "fabnocci(10)", "name": null}], "model":
-      "gpt-3.5-turbo", "temperature": 0.0, "top_p": 1.0, "frequency_penalty": 0.0,
-      "presence_penalty": 0.0, "user": "", "stop": null}'
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null, "max_tokens": 1}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate, br
       Connection:
       - keep-alive
       Content-Length:
-      - '1003'
+      - '283'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"error\": {\n    \"message\": \"None is not of type 'string'
-        - 'messages.0.name'\",\n    \"type\": \"invalid_request_error\",\n    \"param\":
-        null,\n    \"code\": null\n  }\n}\n"
+      string: !!binary |
+        ITQGACDWu+b7GDVv9BGubD9K5FwKtFcisx04bNeoB+qSOItGjxONOJyGAefchIi/R02PZ636ezQA
+        hw0FtIO/lZ22E7+8t3k1XmaPnXH+2MR/mj8sizu73V8NX2t6BqD+j5xdKRGUGLShzijl5PLMNRTE
+        RVVUcZ7XFfgy1cZNKGC/XflpkPur9eJf/SiNYrVbL//6joJslwDbhU7b1c9Kx262pCDJvUGuRKjx
+        pD8CIGhJCgOcsx0GOrRuScEHXZ06wMoOMxcgX+jEUcC/5XK4XP3NVjF1CWyFNwW8JYQzB+zxFn7u
+        07pTwGYQtkngc/4HBZHcnQ3wZc7GAAM=
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d793cfc7cdea39f-TPE
+      - 7d793d111f394a07-TPE
+      Cache-Control:
+      - no-cache, must-revalidate
       Connection:
       - keep-alive
-      Content-Length:
-      - '161'
+      Content-Encoding:
+      - br
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 07:53:15 GMT
+      - Thu, 15 Jun 2023 07:53:18 GMT
       Server:
       - cloudflare
+      Transfer-Encoding:
+      - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
+      openai-model:
+      - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '160'
+      - '288'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89809'
+      - '89985'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 126ms
+      - 10ms
       x-request-id:
-      - 4e91bf51eaa0875c056620b268658a0d
+      - 927252ad65ded9007382607558e3560a
     status:
-      code: 400
-      message: Bad Request
+      code: 200
+      message: OK
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are now the following
-      python function:\n```\n# return fabnocci number\ndef fabnocci(n: int):\n```\nOnly
-      respond with your `return` value.\nThe output should be formatted as a JSON
-      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
-      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
-      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
-      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
-      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
-      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
-      {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```"},
-      {"role": "user", "content": "fabnocci(10)"}], "model": "gpt-3.5-turbo", "temperature":
-      0.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty": 0.0, "user":
-      "", "stop": null}'
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null, "max_tokens": 1}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate, br
       Connection:
       - keep-alive
       Content-Length:
-      - '975'
+      - '283'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
       string: !!binary |
-        IWQGACCW6qp3U42mDuG2p6vpEX1AtuLNP1vuwKFfUQfUkkCjlw5PPfxlYcC5sT23BxTGMau/vwbg
-        9p0Cvm1e9O3oD3G7fOuayct0rtdl7sdZcXMov74v3+375aZlZAC6151900okIwZt606UfHJ5ZN8p
-        yJuu6fK67Qrw5eje7YECrr3GZVLHOg6vLs7KLK92Y3hZWwq83QL0gzt6fVK3t6dAQd73EUqyxKhN
-        0CcBEDQXWW2Af3ebjdu+2UDBHd+0OsDZjiKfgHhwB0sBX0LYBn05qVFLwmV4ZwF/7zlYvaegrv/Z
-        Fv98cOObPN2udaGAQZ1vJ3za/6Ag8+P+DfBg/o0BAw==
+        IUQGACD2Nff6M2pndQifa9mV1QcM4AVVJ5Y7cPhfTx1QSwKNfms7fNGIw9cw4JybEPH3qOnxrFV/
+        /xXA6k4Bb+VluXVDa8bft+Stvv/mT58fY/g35b77/PrQfrR+9nyloQDqa53dFiWsEoNW6Z5STi7P
+        sjsFbpREiRvGqQe+dPqetRSwGBbTt0JzWaerNh3fcdVunS9FRkG2S4DDpLthOS26yfqZAi80BrkS
+        obqT/giAoMmLFLBlO5S6umUzBTu6OnWAlR1mLkA+6TajgJd5rubl0i8xdQlshbcK+J61rSaMjQf2
+        eQunO7XuFLAhhG0U+KT/QYEjd5sCDmpTAw==
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d7941900af44a69-TPE
+      - 7d7941cc1b334a0d-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - br
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 07:56:23 GMT
+      - Thu, 15 Jun 2023 07:56:32 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '690'
+      - '403'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89809'
+      - '89985'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 126ms
+      - 10ms
       x-request-id:
-      - b91691dfeffcbd33853fea11f00149f5
+      - 4898ff5af52aaf251b73e7acf7d688f6
     status:
       code: 200
       message: OK
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are now the following
-      python function:\n```\n# return fabnocci number\ndef fabnocci(n: int):\n```\nOnly
-      respond with your `return` value.\nThe output should be formatted as a JSON
-      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
-      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
-      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
-      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
-      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
-      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
-      {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```"},
-      {"role": "user", "content": "fabnocci(10)"}], "model": "gpt-3.5-turbo", "temperature":
-      0.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty": 0.0, "user":
-      "", "stop": null}'
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null, "max_tokens": 1}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate, br
       Connection:
       - keep-alive
       Content-Length:
-      - '975'
+      - '283'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
       string: !!binary |
-        IWQGACCGuv3vLNPlZky7fZfNMS2hZXrBbAcO2xX1QF0SaDTpcYCZh7soDTg3ttfugMA4ZvX3ZADs
-        Kwqw7HJdzutkJe/l2RKrLr++0ed3z35+s3/OYSljv3dXmgZAWQx1qSthtxjUXi6UdHJ5VFcU8OI0
-        Tr0oCzPwZZZVPVGA7aqtwI4svW+FtNzA9arNrvK2pkC2O4DrJudV/2k51ouigJdpLQBtiVHiRZ8E
-        QNDou5EBHOk2nezLWlHgi69eDWBvR7YXIN7kVFOAuVK90vmig+rmOAzvLMDTN7daf1Mgig7K4uCD
-        E9/c3+1aJwpQabnKOT7tv1PAzWMOA/gxDsMAAw==
+        IUQGACBWzenfqJ3VSQnOtYrAEQXwUiLLHTj8r6cOqCWBRr+1Hb5oxOFrGHDOTYj4e9T0eNaqv18D
+        MDhRwKO/vx2TLLbrs2PrMTp3+yd9LxrT9jBwH3447Wq/P5nTMgD1EDrHmxK5EoMWaEopJ5dnzomC
+        Yq1RaxSrzWodfEn05MQU0MtudjlXtW/3y0HtQrlQVLv7de85FGS7BJhdNMlu25tGTnqloFS1BrkS
+        oRYn/REAQVOpZoB/toOvwdG5UrCkq1MHWNlh5gLkF40dCri/XoPrbZ/eYuoS2ApvFbDjxLESxp8H
+        9nkL2zu17hSwIYRtFPik/0FBQe7+BlibvzEAAw==
+    headers:
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 7d7945d46f9ea3a5-TPE
+      Cache-Control:
+      - no-cache, must-revalidate
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - br
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 15 Jun 2023 07:59:18 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
+      access-control-allow-origin:
+      - '*'
+      alt-svc:
+      - h3=":443"; ma=86400
+      openai-model:
+      - gpt-3.5-turbo-0301
+      openai-processing-ms:
+      - '632'
+      openai-version:
+      - '2020-10-01'
+      strict-transport-security:
+      - max-age=15724800; includeSubDomains
+      x-ratelimit-limit-requests:
+      - '3500'
+      x-ratelimit-limit-tokens:
+      - '90000'
+      x-ratelimit-remaining-requests:
+      - '3499'
+      x-ratelimit-remaining-tokens:
+      - '89985'
+      x-ratelimit-reset-requests:
+      - 17ms
+      x-ratelimit-reset-tokens:
+      - 10ms
+      x-request-id:
+      - 4ab3e114161a7bde8a42aebc164fbbb8
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null, "max_tokens": 1}'
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate, br
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '283'
+      Content-Type:
+      - application/json
+      User-Agent:
+      - OpenAI/v1 PythonBindings/0.27.8
+      X-OpenAI-Client-User-Agent:
+      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
+        "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
+        PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
+    method: POST
+    uri: https://api.openai.com/v1/chat/completions
+  response:
+    body:
+      string: "{\n  \"id\": \"chatcmpl-7Rcn3zfB0twBaf4WY4IedyqgsaPAU\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686818321,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
+        \ \"usage\": {\n    \"prompt_tokens\": 25,\n    \"completion_tokens\": 1,\n
+        \   \"total_tokens\": 26\n  },\n  \"choices\": [\n    {\n      \"message\":
+        {\n        \"role\": \"assistant\",\n        \"content\": \"Hello\"\n      },\n
+        \     \"finish_reason\": \"length\",\n      \"index\": 0\n    }\n  ]\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d79459ffd02075c-TPE
+      - 7d797f8a7fb56b60-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - br
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 07:59:09 GMT
+      - Thu, 15 Jun 2023 08:38:41 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '748'
+      - '428'
+      openai-version:
+      - '2020-10-01'
+      strict-transport-security:
+      - max-age=15724800; includeSubDomains
+      x-ratelimit-limit-requests:
+      - '3500'
+      x-ratelimit-limit-tokens:
+      - '90000'
+      x-ratelimit-remaining-requests:
+      - '3499'
+      x-ratelimit-remaining-tokens:
+      - '89985'
+      x-ratelimit-reset-requests:
+      - 17ms
+      x-ratelimit-reset-tokens:
+      - 10ms
+      x-request-id:
+      - 82dae754f71f98a4eca40e5321af5877
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null, "max_tokens": 1}'
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '283'
+      Content-Type:
+      - application/json
+      User-Agent:
+      - OpenAI/v1 PythonBindings/0.27.8
+      X-OpenAI-Client-User-Agent:
+      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
+        "3.11.3", "platform": "macOS-13.4.1-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
+        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 x86_64 i386"}'
+    method: POST
+    uri: https://api.openai.com/v1/chat/completions
+  response:
+    body:
+      string: "{\n  \"id\": \"chatcmpl-7ZBYIqk5BBgm3pkzl0MaodYTvEyBZ\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1688620242,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
+        \"assistant\",\n        \"content\": \"Hello\"\n      },\n      \"finish_reason\":
+        \"length\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\": 23,\n    \"completion_tokens\":
+        1,\n    \"total_tokens\": 24\n  }\n}\n"
+    headers:
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 7e2557bd58e856f5-TPE
+      Cache-Control:
+      - no-cache, must-revalidate
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 06 Jul 2023 05:10:42 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
+      access-control-allow-origin:
+      - '*'
+      alt-svc:
+      - h3=":443"; ma=86400
+      openai-model:
+      - gpt-3.5-turbo-0613
+      openai-processing-ms:
+      - '453'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89809'
+      - '89985'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 126ms
+      - 10ms
       x-request-id:
-      - 84c0975b1d8f1b49f1d1e2fcddf3e349
+      - 52555e6df4c96c6b2d4dfdc2d96761a1
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml` & `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_chat_completion.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,378 +1,497 @@
 interactions:
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are now the following
-      python function:\n```\n# generate fake hero.\ndef fake_hero(n: int):\n```\nOnly
-      respond with your `return` value.\nThe output should be formatted as a JSON
-      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
-      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
-      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
-      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
-      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
-      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
-      {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
-      \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
-      \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
-      \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
-      \"required\": [\"name\", \"age\"]}}}\n```"}, {"role": "user", "content": "fake_hero(5)"}],
-      "model": "gpt-3.5-turbo", "temperature": 0.0, "top_p": 1.0, "frequency_penalty":
-      0.0, "presence_penalty": 0.0, "user": "", "stop": null}'
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '1288'
+      - '266'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.7
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.7", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.8", "platform": "Linux-5.15.0-72-generic-x86_64-with-glibc2.35", "publisher":
         "openai", "uname": "Linux 5.15.0-72-generic #79-Ubuntu SMP Wed Apr 19 08:22:18
         UTC 2023 x86_64"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"id\": \"chatcmpl-7QZLqztg5MYsSMGntIfhFHyEduL4n\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1686566774,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
-        \ \"usage\": {\n    \"prompt_tokens\": 278,\n    \"completion_tokens\": 107,\n
-        \   \"total_tokens\": 385\n  },\n  \"choices\": [\n    {\n      \"message\":
-        {\n        \"role\": \"assistant\",\n        \"content\": \"```json\\n{\\n
-        \   \\\"ret\\\": [\\n        {\\n            \\\"name\\\": \\\"Superman\\\",\\n
-        \           \\\"age\\\": 35\\n        },\\n        {\\n            \\\"name\\\":
-        \\\"Batman\\\",\\n            \\\"age\\\": 40\\n        },\\n        {\\n
-        \           \\\"name\\\": \\\"Spiderman\\\",\\n            \\\"age\\\": 25\\n
-        \       },\\n        {\\n            \\\"name\\\": \\\"Wonder Woman\\\",\\n
-        \           \\\"age\\\": 30\\n        },\\n        {\\n            \\\"name\\\":
-        \\\"Iron Man\\\",\\n            \\\"age\\\": 45\\n        }\\n    ]\\n}\\n```\"\n
-        \     },\n      \"finish_reason\": \"stop\",\n      \"index\": 0\n    }\n
-        \ ]\n}\n"
+      string: "{\n  \"id\": \"chatcmpl-7QXcwk4gV0eJB61lUnKrwmR3qVE1R\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686560146,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
+        \ \"usage\": {\n    \"prompt_tokens\": 25,\n    \"completion_tokens\": 31,\n
+        \   \"total_tokens\": 56\n  },\n  \"choices\": [\n    {\n      \"message\":
+        {\n        \"role\": \"assistant\",\n        \"content\": \"Hello! I am a
+        language model AI created by OpenAI, designed to assist and communicate with
+        users in natural language. How may I assist you today?\"\n      },\n      \"finish_reason\":
+        \"stop\",\n      \"index\": 0\n    }\n  ]\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d618245ab316b6e-TPE
+      - 7d60e075f9684aa2-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Mon, 12 Jun 2023 10:46:19 GMT
+      - Mon, 12 Jun 2023 08:55:48 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '4195'
+      - '1580'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89743'
+      - '89970'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 170ms
+      - 20ms
       x-request-id:
-      - 017d559b51c138572998a217aeff9fb4
+      - cfe04522ace27d03b1d2175b2155e38f
     status:
       code: 200
       message: OK
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are now the following
-      python function:\n```\n# generate fake hero.\ndef fake_hero(n: int):\n```\nOnly
-      respond with your `return` value.\nThe output should be formatted as a JSON
-      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
-      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
-      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
-      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
-      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
-      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
-      {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
-      \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
-      \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
-      \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
-      \"required\": [\"name\", \"age\"]}}}\n```", "name": null}, {"role": "user",
-      "content": "fake_hero(5)", "name": null}], "model": "gpt-3.5-turbo", "temperature":
-      0.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty": 0.0, "user":
-      "", "stop": null}'
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate, br
       Connection:
       - keep-alive
       Content-Length:
-      - '1316'
+      - '266'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"error\": {\n    \"message\": \"None is not of type 'string'
-        - 'messages.0.name'\",\n    \"type\": \"invalid_request_error\",\n    \"param\":
-        null,\n    \"code\": null\n  }\n}\n"
+      string: !!binary |
+        IcAHACB+5fb2NNWbrTG9iGgVx+wv4Y7ELXdAgdL/CtoeqCVp2IKkw1dvLUjDgANP57YZkuVHTjAi
+        wttfDaC2IAHKm1Tl4zQY0W0ehNNqv+8v5O3Sebscnd+rw+JstTc8kK4BxFlX5spSzBSD0PKKYl8u
+        35UFCThhHMZOECQheDNyUQ4kQPWkDM8MDLXMGRu2ZzvWzSLTuiQBbYcATTOPk3pV3JcrSQJuoC/w
+        igTjwpAAACv8SAP+xQ0abvNSksAjnV1FgFI7nHcC9jMPJQlQKmUrVbpSOnlTVAtvLUAnSEekK+yc
+        3HuPaAXpL7mAYpyErSjaem6E/HzzMuN9Kee27Piwwph+48Ri9s0LFBfp9xbJlX8dQoXk1OunXTsS
+        IKl4kqloYgCJBOw4m38NeNb+NQMD
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d793d0099f1a9bf-TPE
+      - 7d793d052fb56a93-TPE
+      Cache-Control:
+      - no-cache, must-revalidate
       Connection:
       - keep-alive
-      Content-Length:
-      - '161'
+      Content-Encoding:
+      - br
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 07:53:16 GMT
+      - Thu, 15 Jun 2023 07:53:18 GMT
       Server:
       - cloudflare
+      Transfer-Encoding:
+      - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
+      openai-model:
+      - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '247'
+      - '1543'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89743'
+      - '89970'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 170ms
+      - 20ms
       x-request-id:
-      - ec47ea1cf3bfe9040b13fca6fcc74584
+      - dab611cf3a88eb776152739b8ed4a147
     status:
-      code: 400
-      message: Bad Request
+      code: 200
+      message: OK
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are now the following
-      python function:\n```\n# generate fake hero.\ndef fake_hero(n: int):\n```\nOnly
-      respond with your `return` value.\nThe output should be formatted as a JSON
-      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
-      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
-      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
-      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
-      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
-      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
-      {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
-      \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
-      \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
-      \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
-      \"required\": [\"name\", \"age\"]}}}\n```"}, {"role": "user", "content": "fake_hero(5)"}],
-      "model": "gpt-3.5-turbo", "temperature": 0.0, "top_p": 1.0, "frequency_penalty":
-      0.0, "presence_penalty": 0.0, "user": "", "stop": null}'
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate, br
       Connection:
       - keep-alive
       Content-Length:
-      - '1288'
+      - '266'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
       string: !!binary |
-        IYgNACDG6+bvLNO9m6FQsWxfxFM8rSfBvjN1k+hRH0P5ZU0dCzSaA7elgaVRF72GD5xB6iY+opcg
-        dIfqu/DbPwfgKqcAs2VSZzu79cb32WQymH9/Xd3pbK/7dNaog+RkMHl82r1/0nUAmnStstpS7mwx
-        MFdGq9CTy3kqp0B3NBlNusPxZCAU2ZlcbSnAha29fmfo1U2ZGi/oB13rSFMlC0UBbG8B2tLsbB3V
-        ZqN0RYHeeOJKC2ELGqAbjAvfBFAQhvuToQO0+G6WZpWpigIf+jiaDXB3BwOABPzSbBUFmFTVqqoT
-        XUPFw4DX4YkJMI7jdWW01H9SA4BkqWpJgQ8eilYgsdo/dbJTkgKSD41V5S7Rkm4zkkUZ9YfOtreu
-        4/37SV2lHQRHHuwqBwu5d8WL0bkq8WKy0DHk089Ko3HVS6nF5MNM6lbqOI65OuR22mVe3TeInkmb
-        owCr2thVMeAfDQQUCJiR1gFmTusYAw==
+        IUgIACB+r1v1NNV/UwMrnhPR6hwJYpMjya5b3koSYmIE8yGZooomKC5+7YagikIWO9smgcPU4ncK
+        jWb6duMAlMckQFEWmKhWlTd5jaYXyeX7TE6fH8LyeVy8XV9dLyeXjx92SK4DEIeFjIwm+SUGPudG
+        RL9cvpMxCfTG0/G0N5rMusybmmNZkQClyngDf+QZ24bsdQfdnnZldZBKEsB2CJBquVbm13ApG00C
+        /ZFL4BUExKALSwIAXjYaOcAOXCfjPJKaBD7FlasAUGmH8S4Z+5YrSQIUaJ1rEzQGpzoY9cJbC9AN
+        ghpBg5Obe28RrUMypghXeFKyOblxURGTYhiGcZxO8Y9MVgortljkJsM8aHO2GibQpQa3+LeyzeVM
+        iAWioMGNgdGKLQzHweqIAqIdUqJWc+z3W68NCZA2rAJhtFOASALdTFQ7B/h2do4BAw==
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d794196ff924aa0-TPE
+      - 7d7941bbec006b6c-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - br
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 07:56:29 GMT
+      - Thu, 15 Jun 2023 07:56:31 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '5294'
+      - '2216'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89743'
+      - '89970'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 170ms
+      - 20ms
       x-request-id:
-      - 7ae7cabe038370621ee6396830c74a22
+      - 9634705fc80c09a1849faac89be3f2ed
     status:
       code: 200
       message: OK
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are now the following
-      python function:\n```\n# generate fake hero.\ndef fake_hero(n: int):\n```\nOnly
-      respond with your `return` value.\nThe output should be formatted as a JSON
-      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
-      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
-      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
-      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
-      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
-      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
-      {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
-      \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
-      \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
-      \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
-      \"required\": [\"name\", \"age\"]}}}\n```"}, {"role": "user", "content": "fake_hero(5)"}],
-      "model": "gpt-3.5-turbo", "temperature": 0.0, "top_p": 1.0, "frequency_penalty":
-      0.0, "presence_penalty": 0.0, "user": "", "stop": null}'
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate, br
       Connection:
       - keep-alive
       Content-Length:
-      - '1288'
+      - '266'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
       string: !!binary |
-        IYgNACBW6qx3U+1cbYdAXb5iUsxK+E4DfvbUTaJHfQzllzV1LNBoDtyWBpZGXfQaFmgG2TZpiZqC
-        wCc9zLWHvv2LANrWpEDVpgjV0R6S6X21kMvb096dvM5eH77vb2Z8d5xyeLxp+hRHAEm5M1WYKXa2
-        GOhbYRV6cjnP1KTQn8wms/54Pu4JXxylNgdSoLUNybAzTkLjSkl6w57xQOOLtSEFbHcBsk6ONmRB
-        9oY9KQyms1iacZvRAP3eNPNNABmhfzgbR0CL72Qj28p4UvjQx95MgHZ3MABIwHdyMKRAhfdbHwoO
-        UPHQoevwnilQnuc7L6z5TzMAaHImaFL44CFvGRKr/ZOLo9GkoOmhscYdC9YUN61Yl95wbGx5Gxte
-        f1KEKuyot+XBbmuwkAdHvAjXxuFFotAw5N3PnDCuei60mLxYam4153lO2SG2yy7S1X2d7Jm0KVIg
-        H8RmRYf+aMAjhR4z0EbAMmojAwM=
+        IewHACBW6rJXU+1c/YQKAFSAIpv/FEtOeN0BBUr/CtoO1JK2pLAFSccDlnEYtizg9NTjXbIU6tiJ
+        8fdXAJRbkiCTqWhqX3Xnt2Yn8uzga3Jkr65P7y/Ox4fLyfvO7c/dVUYdARDrwpmoSb0UA5fzSkRX
+        Lt85SxLD2WK2GE6X0yn4UrN1FUlQ6mN33Jt2Y9to7g7Gg6F20waVOpLgdgSQb7j28TVy6VaBJEam
+        BoC8cgE1YUsCYFgxWQrgn9wi49y4QBKP4ujKA5TaYbwDsG+4ciRBKoQ8RLWKPPEQ1Auvl6ATqBrq
+        zVtEGrFzguyXbBEZhvgkirqdGyD1N7cNGlepPQVwg9uU82r8w1sYtcIJMld5fHOLyFZ9bxFz+qdE
+        1FNOvP7ftSMJCpE9Y0HLAwgkMQi5+RfAs/gXAw==
+    headers:
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 7d7945c779ab5701-TPE
+      Cache-Control:
+      - no-cache, must-revalidate
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - br
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 15 Jun 2023 07:59:17 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
+      access-control-allow-origin:
+      - '*'
+      alt-svc:
+      - h3=":443"; ma=86400
+      openai-model:
+      - gpt-3.5-turbo-0301
+      openai-processing-ms:
+      - '1615'
+      openai-version:
+      - '2020-10-01'
+      strict-transport-security:
+      - max-age=15724800; includeSubDomains
+      x-ratelimit-limit-requests:
+      - '3500'
+      x-ratelimit-limit-tokens:
+      - '90000'
+      x-ratelimit-remaining-requests:
+      - '3499'
+      x-ratelimit-remaining-tokens:
+      - '89970'
+      x-ratelimit-reset-requests:
+      - 17ms
+      x-ratelimit-reset-tokens:
+      - 20ms
+      x-request-id:
+      - 3711cb7edf9fb45b9db1ff54c05cf148
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null}'
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate, br
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '266'
+      Content-Type:
+      - application/json
+      User-Agent:
+      - OpenAI/v1 PythonBindings/0.27.8
+      X-OpenAI-Client-User-Agent:
+      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
+        "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
+        PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
+    method: POST
+    uri: https://api.openai.com/v1/chat/completions
+  response:
+    body:
+      string: "{\n  \"id\": \"chatcmpl-7Rcn1AdfM7tJDzJUDgjic5Mmv0oa6\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686818319,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
+        \ \"usage\": {\n    \"prompt_tokens\": 25,\n    \"completion_tokens\": 25,\n
+        \   \"total_tokens\": 50\n  },\n  \"choices\": [\n    {\n      \"message\":
+        {\n        \"role\": \"assistant\",\n        \"content\": \"Hello! I am an
+        AI language model designed to assist and communicate with users like you.
+        How can I help you today?\"\n      },\n      \"finish_reason\": \"stop\",\n
+        \     \"index\": 0\n    }\n  ]\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d7945a7cbb2a9cb-TPE
+      - 7d797f7f6c554a0f-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - br
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 07:59:15 GMT
+      - Thu, 15 Jun 2023 08:38:40 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '4767'
+      - '1477'
+      openai-version:
+      - '2020-10-01'
+      strict-transport-security:
+      - max-age=15724800; includeSubDomains
+      x-ratelimit-limit-requests:
+      - '3500'
+      x-ratelimit-limit-tokens:
+      - '90000'
+      x-ratelimit-remaining-requests:
+      - '3499'
+      x-ratelimit-remaining-tokens:
+      - '89970'
+      x-ratelimit-reset-requests:
+      - 17ms
+      x-ratelimit-reset-tokens:
+      - 20ms
+      x-request-id:
+      - 563b2ecdb62ece2b0117d9c16ce95036
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "stop": null}'
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '266'
+      Content-Type:
+      - application/json
+      User-Agent:
+      - OpenAI/v1 PythonBindings/0.27.8
+      X-OpenAI-Client-User-Agent:
+      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
+        "3.11.3", "platform": "macOS-13.4.1-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
+        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 x86_64 i386"}'
+    method: POST
+    uri: https://api.openai.com/v1/chat/completions
+  response:
+    body:
+      string: "{\n  \"id\": \"chatcmpl-7ZBYGVJUJpf4SL6k2sLj89LzqdI5p\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1688620240,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
+        \"assistant\",\n        \"content\": \"Hello! I am a helpful assistant here
+        to assist you with any questions or tasks you may have. How can I help you
+        today?\"\n      },\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\":
+        {\n    \"prompt_tokens\": 23,\n    \"completion_tokens\": 27,\n    \"total_tokens\":
+        50\n  }\n}\n"
+    headers:
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 7e2557b609fd4a86-TPE
+      Cache-Control:
+      - no-cache, must-revalidate
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 06 Jul 2023 05:10:41 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
+      access-control-allow-origin:
+      - '*'
+      alt-svc:
+      - h3=":443"; ma=86400
+      openai-model:
+      - gpt-3.5-turbo-0613
+      openai-processing-ms:
+      - '894'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89743'
+      - '89970'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 170ms
+      - 20ms
       x-request-id:
-      - 855b39fe1a43a7061adb5479dd5f5356
+      - 449bb787d1a2f835fb07673e5778f4ee
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml` & `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,407 +1,256 @@
 interactions:
 - request:
     body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
-      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
-      0.0, "user": "", "stop": null, "max_tokens": 1}'
+      {"role": "user", "content": "I want to book a flight to London."}], "model":
+      "gpt-3.5-turbo", "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0,
+      "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name": "book_a_flight",
+      "description": "", "parameters": {"type": "object", "required": ["date", "destination"],
+      "properties": {"date": {"title": "Date", "type": "string"}, "destination": {"title":
+      "Destination", "type": "string"}, "origin": {"title": "Origin", "default": "London",
+      "type": "string"}}, "definitions": {}}}], "function_call": "auto"}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
-      - gzip, deflate
+      - gzip, deflate, br
       Connection:
       - keep-alive
       Content-Length:
-      - '283'
+      - '647'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.7
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.7", "httplib": "requests", "lang": "python", "lang_version":
-        "3.10.8", "platform": "Linux-5.15.0-72-generic-x86_64-with-glibc2.35", "publisher":
-        "openai", "uname": "Linux 5.15.0-72-generic #79-Ubuntu SMP Wed Apr 19 08:22:18
-        UTC 2023 x86_64"}'
-    method: POST
-    uri: https://api.openai.com/v1/chat/completions
-  response:
-    body:
-      string: "{\n  \"id\": \"chatcmpl-7QXcyFNjAlIIPRuU5YEC6vUlqwu6R\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1686560148,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
-        \ \"usage\": {\n    \"prompt_tokens\": 25,\n    \"completion_tokens\": 1,\n
-        \   \"total_tokens\": 26\n  },\n  \"choices\": [\n    {\n      \"message\":
-        {\n        \"role\": \"assistant\",\n        \"content\": \"Hello\"\n      },\n
-        \     \"finish_reason\": \"length\",\n      \"index\": 0\n    }\n  ]\n}\n"
-    headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 7d60e0820c3ba9cb-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
-      Content-Type:
-      - application/json
-      Date:
-      - Mon, 12 Jun 2023 08:55:49 GMT
-      Server:
-      - cloudflare
-      Transfer-Encoding:
-      - chunked
-      access-control-allow-origin:
-      - '*'
-      alt-svc:
-      - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0301
-      openai-processing-ms:
-      - '195'
-      openai-version:
-      - '2020-10-01'
-      strict-transport-security:
-      - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '3500'
-      x-ratelimit-limit-tokens:
-      - '90000'
-      x-ratelimit-remaining-requests:
-      - '3499'
-      x-ratelimit-remaining-tokens:
-      - '89985'
-      x-ratelimit-reset-requests:
-      - 17ms
-      x-ratelimit-reset-tokens:
-      - 10ms
-      x-request-id:
-      - 9b24c553c430a32d49942fc89bddcd00
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
-      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
-      0.0, "user": "", "stop": null, "max_tokens": 1}'
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate, br
-      Connection:
-      - keep-alive
-      Content-Length:
-      - '283'
-      Content-Type:
-      - application/json
-      User-Agent:
-      - OpenAI/v1 PythonBindings/0.27.8
-      X-OpenAI-Client-User-Agent:
-      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: !!binary |
-        ITQGACDWu+b7GDVv9BGubD9K5FwKtFcisx04bNeoB+qSOItGjxONOJyGAefchIi/R02PZ636ezQA
-        hw0FtIO/lZ22E7+8t3k1XmaPnXH+2MR/mj8sizu73V8NX2t6BqD+j5xdKRGUGLShzijl5PLMNRTE
-        RVVUcZ7XFfgy1cZNKGC/XflpkPur9eJf/SiNYrVbL//6joJslwDbhU7b1c9Kx262pCDJvUGuRKjx
-        pD8CIGhJCgOcsx0GOrRuScEHXZ06wMoOMxcgX+jEUcC/5XK4XP3NVjF1CWyFNwW8JYQzB+zxFn7u
-        07pTwGYQtkngc/4HBZHcnQ3wZc7GAAM=
+      string: "{\n  \"error\": {\n    \"message\": \"Unrecognized request arguments
+        supplied: function_call, functions\",\n    \"type\": \"invalid_request_error\",\n
+        \   \"param\": null,\n    \"code\": null\n  }\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d793d111f394a07-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - br
-      Content-Type:
-      - application/json
-      Date:
-      - Thu, 15 Jun 2023 07:53:18 GMT
-      Server:
-      - cloudflare
-      Transfer-Encoding:
-      - chunked
-      access-control-allow-origin:
-      - '*'
-      alt-svc:
-      - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0301
-      openai-processing-ms:
-      - '288'
-      openai-version:
-      - '2020-10-01'
-      strict-transport-security:
-      - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '3500'
-      x-ratelimit-limit-tokens:
-      - '90000'
-      x-ratelimit-remaining-requests:
-      - '3499'
-      x-ratelimit-remaining-tokens:
-      - '89985'
-      x-ratelimit-reset-requests:
-      - 17ms
-      x-ratelimit-reset-tokens:
-      - 10ms
-      x-request-id:
-      - 927252ad65ded9007382607558e3560a
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
-      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
-      0.0, "user": "", "stop": null, "max_tokens": 1}'
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate, br
+      - 7d797a9cbbfda3a6-TPE
       Connection:
       - keep-alive
       Content-Length:
-      - '283'
-      Content-Type:
-      - application/json
-      User-Agent:
-      - OpenAI/v1 PythonBindings/0.27.8
-      X-OpenAI-Client-User-Agent:
-      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
-        "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
-        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
-        PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
-    method: POST
-    uri: https://api.openai.com/v1/chat/completions
-  response:
-    body:
-      string: !!binary |
-        IUQGACD2Nff6M2pndQifa9mV1QcM4AVVJ5Y7cPhfTx1QSwKNfms7fNGIw9cw4JybEPH3qOnxrFV/
-        /xXA6k4Bb+VluXVDa8bft+Stvv/mT58fY/g35b77/PrQfrR+9nyloQDqa53dFiWsEoNW6Z5STi7P
-        sjsFbpREiRvGqQe+dPqetRSwGBbTt0JzWaerNh3fcdVunS9FRkG2S4DDpLthOS26yfqZAi80BrkS
-        obqT/giAoMmLFLBlO5S6umUzBTu6OnWAlR1mLkA+6TajgJd5rubl0i8xdQlshbcK+J61rSaMjQf2
-        eQunO7XuFLAhhG0U+KT/QYEjd5sCDmpTAw==
-    headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 7d7941cc1b334a0d-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - br
+      - '178'
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 07:56:32 GMT
+      - Thu, 15 Jun 2023 08:35:19 GMT
       Server:
       - cloudflare
-      Transfer-Encoding:
-      - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '403'
+      - '277'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89985'
+      - '89965'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 10ms
+      - 22ms
       x-request-id:
-      - 4898ff5af52aaf251b73e7acf7d688f6
+      - 43f58092d90c67d254b56d02e9a79f28
     status:
-      code: 200
-      message: OK
+      code: 400
+      message: Bad Request
 - request:
     body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
-      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
-      0.0, "user": "", "stop": null, "max_tokens": 1}'
+      {"role": "user", "content": "I want to book a flight to London."}], "model":
+      "gpt-3.5-turbo-0613", "temperature": 1.0, "top_p": 1.0, "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name":
+      "book_a_flight", "description": "", "parameters": {"type": "object", "required":
+      ["date", "destination"], "properties": {"date": {"title": "Date", "type": "string"},
+      "destination": {"title": "Destination", "type": "string"}, "origin": {"title":
+      "Origin", "default": "London", "type": "string"}}, "definitions": {}}}], "function_call":
+      "auto"}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate, br
       Connection:
       - keep-alive
       Content-Length:
-      - '283'
+      - '652'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
         "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: !!binary |
-        IUQGACBWzenfqJ3VSQnOtYrAEQXwUiLLHTj8r6cOqCWBRr+1Hb5oxOFrGHDOTYj4e9T0eNaqv18D
-        MDhRwKO/vx2TLLbrs2PrMTp3+yd9LxrT9jBwH3447Wq/P5nTMgD1EDrHmxK5EoMWaEopJ5dnzomC
-        Yq1RaxSrzWodfEn05MQU0MtudjlXtW/3y0HtQrlQVLv7de85FGS7BJhdNMlu25tGTnqloFS1BrkS
-        oRYn/REAQVOpZoB/toOvwdG5UrCkq1MHWNlh5gLkF40dCri/XoPrbZ/eYuoS2ApvFbDjxLESxp8H
-        9nkL2zu17hSwIYRtFPik/0FBQe7+BlibvzEAAw==
+      string: "{\n  \"id\": \"chatcmpl-7Rcn0p2QWV0fnKNBaYh9kxjxiOr2c\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686818318,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
+        \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n
+        \         \"name\": \"book_a_flight\",\n          \"arguments\": \"{\\n  \\\"date\\\":
+        \\\"2022-10-15\\\",\\n  \\\"destination\\\": \\\"London\\\"\\n}\"\n        }\n
+        \     },\n      \"finish_reason\": \"function_call\"\n    }\n  ],\n  \"usage\":
+        {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 28,\n    \"total_tokens\":
+        95\n  }\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d7945d46f9ea3a5-TPE
+      - 7d797f72bafa49f7-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - br
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 07:59:18 GMT
+      - Thu, 15 Jun 2023 08:38:39 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
-      - gpt-3.5-turbo-0301
+      - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '632'
+      - '1203'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
-      - '3500'
+      - '3000'
       x-ratelimit-limit-tokens:
-      - '90000'
+      - '250000'
       x-ratelimit-remaining-requests:
-      - '3499'
+      - '2999'
       x-ratelimit-remaining-tokens:
-      - '89985'
+      - '249966'
       x-ratelimit-reset-requests:
-      - 17ms
+      - 20ms
       x-ratelimit-reset-tokens:
-      - 10ms
+      - 8ms
       x-request-id:
-      - 4ab3e114161a7bde8a42aebc164fbbb8
+      - 6944c8adb679697ffefbf82d397bfa3b
     status:
       code: 200
       message: OK
 - request:
     body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
-      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
-      0.0, "user": "", "stop": null, "max_tokens": 1}'
+      {"role": "user", "content": "I want to book a flight to London."}], "model":
+      "gpt-3.5-turbo-0613", "temperature": 1.0, "top_p": 1.0, "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name":
+      "book_a_flight", "description": "", "parameters": {"type": "object", "required":
+      ["date", "destination"], "properties": {"date": {"title": "Date", "type": "string"},
+      "destination": {"title": "Destination", "type": "string"}, "origin": {"title":
+      "Origin", "default": "London", "type": "string"}}, "definitions": {}}}], "function_call":
+      "auto"}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
-      - gzip, deflate, br
+      - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '283'
+      - '652'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
-        "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
-        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
-        PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
+        "3.11.3", "platform": "macOS-13.4.1-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
+        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"id\": \"chatcmpl-7Rcn3zfB0twBaf4WY4IedyqgsaPAU\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1686818321,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
-        \ \"usage\": {\n    \"prompt_tokens\": 25,\n    \"completion_tokens\": 1,\n
-        \   \"total_tokens\": 26\n  },\n  \"choices\": [\n    {\n      \"message\":
-        {\n        \"role\": \"assistant\",\n        \"content\": \"Hello\"\n      },\n
-        \     \"finish_reason\": \"length\",\n      \"index\": 0\n    }\n  ]\n}\n"
+      string: "{\n  \"id\": \"chatcmpl-7ZBY7p5W84q561lbKQPy5WXZleRnB\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1688620231,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
+        \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n
+        \         \"name\": \"book_a_flight\",\n          \"arguments\": \"{\\n  \\\"date\\\":
+        \\\"2022-10-10\\\",\\n  \\\"destination\\\": \\\"London\\\"\\n}\"\n        }\n
+        \     },\n      \"finish_reason\": \"function_call\"\n    }\n  ],\n  \"usage\":
+        {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 28,\n    \"total_tokens\":
+        95\n  }\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d797f8a7fb56b60-TPE
+      - 7e25577928e46b62-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
-      - br
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 08:38:41 GMT
+      - Thu, 06 Jul 2023 05:10:31 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
-      - gpt-3.5-turbo-0301
+      - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '428'
+      - '984'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89985'
+      - '89965'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 10ms
+      - 22ms
       x-request-id:
-      - 82dae754f71f98a4eca40e5321af5877
+      - 2b30f764185282aeefd5dffc471df95c
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion.yaml` & `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion_without_enough_tokens.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,167 +1,175 @@
 interactions:
 - request:
     body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "I want to book a flight to London."}], "model":
-      "gpt-3.5-turbo", "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0,
-      "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name": "book_a_flight",
-      "description": "", "parameters": {"type": "object", "required": ["date", "destination"],
-      "properties": {"date": {"title": "Date", "type": "string"}, "destination": {"title":
-      "Destination", "type": "string"}, "origin": {"title": "Origin", "default": "London",
-      "type": "string"}}, "definitions": {}}}], "function_call": "auto"}'
+      {"role": "user", "content": "I want to book a restaurant in London."}], "model":
+      "gpt-3.5-turbo-0613", "temperature": 1.0, "top_p": 1.0, "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name":
+      "book_a_flight", "description": "", "parameters": {"type": "object", "required":
+      ["date", "destination"], "properties": {"date": {"title": "Date", "type": "string"},
+      "destination": {"title": "Destination", "type": "string"}, "origin": {"title":
+      "Origin", "default": "London", "type": "string"}}, "definitions": {}}}], "function_call":
+      "auto", "max_tokens": 10}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
-      - gzip, deflate, br
+      - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '647'
+      - '674'
       Content-Type:
       - application/json
       User-Agent:
-      - OpenAI/v1 PythonBindings/0.27.7
+      - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
-      - '{"bindings_version": "0.27.7", "httplib": "requests", "lang": "python", "lang_version":
-        "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
-        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
-        PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
+      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
+        "3.10.8", "platform": "macOS-12.4-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 21.5.0 Darwin Kernel Version 21.5.0: Tue Apr 26 21:08:22
+        PDT 2022; root:xnu-8020.121.3~4/RELEASE_X86_64 x86_64"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"error\": {\n    \"message\": \"Unrecognized request arguments
-        supplied: function_call, functions\",\n    \"type\": \"invalid_request_error\",\n
-        \   \"param\": null,\n    \"code\": null\n  }\n}\n"
+      string: "{\n  \"id\": \"chatcmpl-7Vj1f3ooUNnNia71ycQeNKu3ak80v\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1687795603,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
+        \"assistant\",\n        \"content\": \"Sure, I can help you with that.\"\n
+        \     },\n      \"finish_reason\": \"length\"\n    }\n  ],\n  \"usage\": {\n
+        \   \"prompt_tokens\": 67,\n    \"completion_tokens\": 10,\n    \"total_tokens\":
+        77\n  }\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d797a9cbbfda3a6-TPE
+      - 7dd6b2f68c7c4a67-TPE
+      Cache-Control:
+      - no-cache, must-revalidate
       Connection:
       - keep-alive
-      Content-Length:
-      - '178'
+      Content-Encoding:
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 08:35:19 GMT
+      - Mon, 26 Jun 2023 16:06:43 GMT
       Server:
       - cloudflare
+      Transfer-Encoding:
+      - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
+      openai-model:
+      - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '277'
+      - '386'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89965'
+      - '89970'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 22ms
+      - 19ms
       x-request-id:
-      - 43f58092d90c67d254b56d02e9a79f28
+      - cf4890712fd4a77a56bf5a9d8079339b
     status:
-      code: 400
-      message: Bad Request
+      code: 200
+      message: OK
 - request:
     body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "I want to book a flight to London."}], "model":
+      {"role": "user", "content": "I want to book a restaurant in London."}], "model":
       "gpt-3.5-turbo-0613", "temperature": 1.0, "top_p": 1.0, "frequency_penalty":
       0.0, "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name":
       "book_a_flight", "description": "", "parameters": {"type": "object", "required":
       ["date", "destination"], "properties": {"date": {"title": "Date", "type": "string"},
       "destination": {"title": "Destination", "type": "string"}, "origin": {"title":
       "Origin", "default": "London", "type": "string"}}, "definitions": {}}}], "function_call":
-      "auto"}'
+      "auto", "max_tokens": 10}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
-      - gzip, deflate, br
+      - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '652'
+      - '674'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
-        "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
-        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
-        PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
+        "3.11.3", "platform": "macOS-13.4.1-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
+        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"id\": \"chatcmpl-7Rcn0p2QWV0fnKNBaYh9kxjxiOr2c\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1686818318,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+      string: "{\n  \"id\": \"chatcmpl-7ZBY8uZFGFehUaSyw7QwJA7vP4rNF\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1688620232,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
         \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-        \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n
-        \         \"name\": \"book_a_flight\",\n          \"arguments\": \"{\\n  \\\"date\\\":
-        \\\"2022-10-15\\\",\\n  \\\"destination\\\": \\\"London\\\"\\n}\"\n        }\n
-        \     },\n      \"finish_reason\": \"function_call\"\n    }\n  ],\n  \"usage\":
-        {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 28,\n    \"total_tokens\":
-        95\n  }\n}\n"
+        \"assistant\",\n        \"content\": \"I'm sorry, but I am not able\"\n      },\n
+        \     \"finish_reason\": \"length\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
+        67,\n    \"completion_tokens\": 10,\n    \"total_tokens\": 77\n  }\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d797f72bafa49f7-TPE
+      - 7e255781ad2a4a82-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
-      - br
+      - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 15 Jun 2023 08:38:39 GMT
+      - Thu, 06 Jul 2023 05:10:33 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '1203'
+      - '997'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
-      - '3000'
+      - '3500'
       x-ratelimit-limit-tokens:
-      - '250000'
+      - '90000'
       x-ratelimit-remaining-requests:
-      - '2999'
+      - '3499'
       x-ratelimit-remaining-tokens:
-      - '249966'
+      - '89971'
       x-ratelimit-reset-requests:
-      - 20ms
+      - 17ms
       x-ratelimit-reset-tokens:
-      - 8ms
+      - 19ms
       x-request-id:
-      - 6944c8adb679697ffefbf82d397bfa3b
+      - 64db3ab8104473b641b94f6d95198342
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion_without_enough_tokens.yaml` & `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,92 @@
 interactions:
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "I want to book a restaurant in London."}], "model":
-      "gpt-3.5-turbo-0613", "temperature": 1.0, "top_p": 1.0, "frequency_penalty":
-      0.0, "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name":
-      "book_a_flight", "description": "", "parameters": {"type": "object", "required":
-      ["date", "destination"], "properties": {"date": {"title": "Date", "type": "string"},
-      "destination": {"title": "Destination", "type": "string"}, "origin": {"title":
-      "Origin", "default": "London", "type": "string"}}, "definitions": {}}}], "function_call":
-      "auto", "max_tokens": 10}'
+    body: '{"messages": [{"role": "system", "content": "You are now the following
+      python function:\n```\n# return fabnocci number\ndef fabnocci(n: int):\n```\nOnly
+      respond with your `return` value.\n- The output should be formatted as a JSON
+      instance that conforms to the JSON schema below.\n\n- As an example, for the
+      schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a
+      list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
+      \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
+      instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
+      is not well-formatted.\n\n- Here is the output schema:\n```\n{\"properties\":
+      {\"ret\": {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```"},
+      {"role": "user", "content": "fabnocci(10)"}], "model": "gpt-3.5-turbo", "temperature":
+      0.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty": 0.0, "user":
+      "", "stop": null}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '674'
+      - '981'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
-        "3.10.8", "platform": "macOS-12.4-x86_64-i386-64bit", "publisher": "openai",
-        "uname": "Darwin 21.5.0 Darwin Kernel Version 21.5.0: Tue Apr 26 21:08:22
-        PDT 2022; root:xnu-8020.121.3~4/RELEASE_X86_64 x86_64"}'
+        "3.11.3", "platform": "macOS-13.4.1-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
+        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"id\": \"chatcmpl-7Vj1f3ooUNnNia71ycQeNKu3ak80v\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1687795603,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+      string: "{\n  \"id\": \"chatcmpl-7ZBZ0cgg7n3wzAIXM8IvVuiQYstjW\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1688620286,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
         \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-        \"assistant\",\n        \"content\": \"Sure, I can help you with that.\"\n
-        \     },\n      \"finish_reason\": \"length\"\n    }\n  ],\n  \"usage\": {\n
-        \   \"prompt_tokens\": 67,\n    \"completion_tokens\": 10,\n    \"total_tokens\":
-        77\n  }\n}\n"
+        \"assistant\",\n        \"content\": \"{\\\"ret\\\": 55}\"\n      },\n      \"finish_reason\":
+        \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\": 200,\n    \"completion_tokens\":
+        6,\n    \"total_tokens\": 206\n  }\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7dd6b2f68c7c4a67-TPE
+      - 7e2558d5297c56e9-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Mon, 26 Jun 2023 16:06:43 GMT
+      - Thu, 06 Jul 2023 05:11:26 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '386'
+      - '225'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89970'
+      - '89809'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
-      - 19ms
+      - 127ms
       x-request-id:
-      - cf4890712fd4a77a56bf5a9d8079339b
+      - 7933103f0717a888f4d13ee5558f77ed
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml` & `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -83,8 +83,97 @@
       x-ratelimit-reset-tokens:
       - 8ms
       x-request-id:
       - 03348d5940aa708d149dff8ce7452a28
     status:
       code: 200
       message: OK
+- request:
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "I want to book a restaurant in London."}], "model":
+      "gpt-3.5-turbo-0613", "temperature": 1.0, "top_p": 1.0, "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name":
+      "book_a_flight", "description": "", "parameters": {"type": "object", "required":
+      ["date", "destination"], "properties": {"date": {"title": "Date", "type": "string"},
+      "destination": {"title": "Destination", "type": "string"}, "origin": {"title":
+      "Origin", "default": "London", "type": "string"}}, "definitions": {}}}], "function_call":
+      "auto"}'
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '656'
+      Content-Type:
+      - application/json
+      User-Agent:
+      - OpenAI/v1 PythonBindings/0.27.8
+      X-OpenAI-Client-User-Agent:
+      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
+        "3.11.3", "platform": "macOS-13.4.1-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
+        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 x86_64 i386"}'
+    method: POST
+    uri: https://api.openai.com/v1/chat/completions
+  response:
+    body:
+      string: "{\n  \"id\": \"chatcmpl-7ZBY9DUqTANRGNO21QkSxA3KiTa8X\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1688620233,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
+        \"assistant\",\n        \"content\": \"Sure, I can help you with that. Can
+        you please provide me with the date and time you would like to book the restaurant
+        for, as well as any specific cuisine preferences or dietary restrictions you
+        have?\"\n      },\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\":
+        {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 42,\n    \"total_tokens\":
+        109\n  }\n}\n"
+    headers:
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 7e25578bca516b6c-TPE
+      Cache-Control:
+      - no-cache, must-revalidate
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 06 Jul 2023 05:10:34 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
+      access-control-allow-origin:
+      - '*'
+      alt-svc:
+      - h3=":443"; ma=86400
+      openai-model:
+      - gpt-3.5-turbo-0613
+      openai-processing-ms:
+      - '1075'
+      openai-version:
+      - '2020-10-01'
+      strict-transport-security:
+      - max-age=15724800; includeSubDomains
+      x-ratelimit-limit-requests:
+      - '3500'
+      x-ratelimit-limit-tokens:
+      - '90000'
+      x-ratelimit-remaining-requests:
+      - '3499'
+      x-ratelimit-remaining-tokens:
+      - '89965'
+      x-ratelimit-reset-requests:
+      - 17ms
+      x-ratelimit-reset-tokens:
+      - 23ms
+      x-request-id:
+      - 6b3910bcda87e232dadf25653dff1ca1
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_structural_completion_without_enough_tokens.yaml` & `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_structural_completion_without_enough_tokens.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -83,8 +83,96 @@
       x-ratelimit-reset-tokens:
       - 16ms
       x-request-id:
       - 1fd9cc433da2bddde7ab0814cecc6c6c
     status:
       code: 200
       message: OK
+- request:
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "Give me a sample email."}], "model": "gpt-3.5-turbo-0613",
+      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
+      0.0, "user": "", "functions": [{"name": "structural_response", "description":
+      "Response to user in a structural way.", "parameters": {"title": "Email", "type":
+      "object", "properties": {"subject": {"title": "Subject", "description": "the
+      subject of email", "type": "string"}, "body": {"title": "Body", "description":
+      "the body of email", "type": "string"}}, "required": ["subject", "body"]}}],
+      "function_call": {"name": "structural_response"}, "max_tokens": 10}'
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '705'
+      Content-Type:
+      - application/json
+      User-Agent:
+      - OpenAI/v1 PythonBindings/0.27.8
+      X-OpenAI-Client-User-Agent:
+      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
+        "3.11.3", "platform": "macOS-13.4.1-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
+        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 x86_64 i386"}'
+    method: POST
+    uri: https://api.openai.com/v1/chat/completions
+  response:
+    body:
+      string: "{\n  \"id\": \"chatcmpl-7ZBYFA7wkLrUwlnbBYkmbgjM49eqX\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1688620239,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
+        \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n
+        \         \"name\": \"structural_response\",\n          \"arguments\": \"{\\n
+        \ \\\"subject\\\": \\\"Sample Email\\\",\\n \"\n        }\n      },\n      \"finish_reason\":
+        \"length\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\": 82,\n    \"completion_tokens\":
+        10,\n    \"total_tokens\": 92\n  }\n}\n"
+    headers:
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 7e2557af9c8aa9d1-TPE
+      Cache-Control:
+      - no-cache, must-revalidate
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 06 Jul 2023 05:10:40 GMT
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
+      access-control-allow-origin:
+      - '*'
+      alt-svc:
+      - h3=":443"; ma=86400
+      openai-model:
+      - gpt-3.5-turbo-0613
+      openai-processing-ms:
+      - '692'
+      openai-version:
+      - '2020-10-01'
+      strict-transport-security:
+      - max-age=15724800; includeSubDomains
+      x-ratelimit-limit-requests:
+      - '3500'
+      x-ratelimit-limit-tokens:
+      - '90000'
+      x-ratelimit-remaining-requests:
+      - '3499'
+      x-ratelimit-remaining-tokens:
+      - '89974'
+      x-ratelimit-reset-requests:
+      - 17ms
+      x-ratelimit-reset-tokens:
+      - 16ms
+      x-request-id:
+      - 695bce85483c6d0cf8682bbf97c08f79
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/test_ai_function.py` & `gpt_fn-0.0.8/src/gpt_fn/tests/test_ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/test_completion.py` & `gpt_fn-0.0.8/src/gpt_fn/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/src/gpt_fn/tests/test_prompt.py` & `gpt_fn-0.0.8/src/gpt_fn/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/src/gpt_fn/utils/pydantic_parser.py` & `gpt_fn-0.0.8/src/gpt_fn/utils/pydantic_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 T = TypeVar("T", bound=BaseModel)
 
 
 class ParserError(Exception):
     pass
 
 
-PYDANTIC_FORMAT_INSTRUCTIONS = """The output should be formatted as a JSON instance that conforms to the JSON schema below.
+PYDANTIC_FORMAT_INSTRUCTIONS = """- The output should be formatted as a JSON instance that conforms to the JSON schema below.
 
-As an example, for the schema {{"properties": {{"foo": {{"title": "Foo", "description": "a list of strings", "type": "array", "items": {{"type": "string"}}}}}}, "required": ["foo"]}}}}
+- As an example, for the schema {{"properties": {{"foo": {{"title": "Foo", "description": "a list of strings", "type": "array", "items": {{"type": "string"}}}}}}, "required": ["foo"]}}}}
 the object {{"foo": ["bar", "baz"]}} is a well-formatted instance of the schema. The object {{"properties": {{"foo": ["bar", "baz"]}}}} is not well-formatted.
 
-Here is the output schema:
+- Here is the output schema:
 ```
 {schema}
 ```"""
 
 
 class PydanticParser(GenericModel, Generic[T]):
     pydantic_model: type[T]
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/utils/signature.py` & `gpt_fn-0.0.8/src/gpt_fn/utils/signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr` & `gpt_fn-0.0.8/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
   '''
   You are now the following python function:
   ```
   # Add two numbers.
   def add(a: int, b: int = 10):
   ```
   Only respond with your `return` value.
-  The output should be formatted as a JSON instance that conforms to the JSON schema below.
+  - The output should be formatted as a JSON instance that conforms to the JSON schema below.
   
-  As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
+  - As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
   the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.
   
-  Here is the output schema:
+  - Here is the output schema:
   ```
   {"properties": {"ret": {"title": "Ret", "type": "integer"}}, "required": ["ret"]}
   ```
   
   '''
 # ---
 # name: test_function_signature[add-args0-kwargs0].1
@@ -51,20 +51,20 @@
   '''
   You are now the following python function:
   ```
   # Complex function
   def complex(a: str, b: str, *args: str, c: str, d: str, **kwargs: str):
   ```
   Only respond with your `return` value.
-  The output should be formatted as a JSON instance that conforms to the JSON schema below.
+  - The output should be formatted as a JSON instance that conforms to the JSON schema below.
   
-  As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
+  - As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
   the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.
   
-  Here is the output schema:
+  - Here is the output schema:
   ```
   {"properties": {"ret": {"title": "Ret", "type": "string"}}, "required": ["ret"]}
   ```
   
   '''
 # ---
 # name: test_function_signature[complex-args5-kwargs5].1
@@ -112,20 +112,20 @@
   # Concat two strings
   :param a: first string
   :param b: second string
   
   def concat(a: str, b: str):
   ```
   Only respond with your `return` value.
-  The output should be formatted as a JSON instance that conforms to the JSON schema below.
+  - The output should be formatted as a JSON instance that conforms to the JSON schema below.
   
-  As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
+  - As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
   the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.
   
-  Here is the output schema:
+  - Here is the output schema:
   ```
   {"properties": {"ret": {"title": "Ret", "type": "string"}}, "required": ["ret"]}
   ```
   
   '''
 # ---
 # name: test_function_signature[concat-args2-kwargs2].1
@@ -170,20 +170,20 @@
   # Concat two strings
   :param a: first string
   :param b: second string
   
   def concat(a: str, b: str):
   ```
   Only respond with your `return` value.
-  The output should be formatted as a JSON instance that conforms to the JSON schema below.
+  - The output should be formatted as a JSON instance that conforms to the JSON schema below.
   
-  As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
+  - As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
   the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.
   
-  Here is the output schema:
+  - Here is the output schema:
   ```
   {"properties": {"ret": {"title": "Ret", "type": "string"}}, "required": ["ret"]}
   ```
   
   '''
 # ---
 # name: test_function_signature[concat-args3-kwargs3].1
@@ -225,20 +225,20 @@
   '''
   You are now the following python function:
   ```
   # Concat the given strings
   def concats(*args: str):
   ```
   Only respond with your `return` value.
-  The output should be formatted as a JSON instance that conforms to the JSON schema below.
+  - The output should be formatted as a JSON instance that conforms to the JSON schema below.
   
-  As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
+  - As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
   the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.
   
-  Here is the output schema:
+  - Here is the output schema:
   ```
   {"properties": {"ret": {"title": "Ret", "type": "string"}}, "required": ["ret"]}
   ```
   
   '''
 # ---
 # name: test_function_signature[concats-args4-kwargs4].1
@@ -263,20 +263,20 @@
   '''
   You are now the following python function:
   ```
   # generate fake person.
   def fake_person(count: int):
   ```
   Only respond with your `return` value.
-  The output should be formatted as a JSON instance that conforms to the JSON schema below.
+  - The output should be formatted as a JSON instance that conforms to the JSON schema below.
   
-  As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
+  - As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
   the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.
   
-  Here is the output schema:
+  - Here is the output schema:
   ```
   {"properties": {"ret": {"$ref": "#/definitions/Person"}}, "required": ["ret"], "definitions": {"Person": {"title": "Person", "description": "Person model.", "type": "object", "properties": {"name": {"title": "Name", "type": "string"}, "age": {"title": "Age", "type": "integer"}}, "required": ["name", "age"]}}}
   ```
   
   '''
 # ---
 # name: test_function_signature[fake_person-args1-kwargs1].1
@@ -306,20 +306,20 @@
   '''
   You are now the following python function:
   ```
   # "Get the current weather in a given location
   def get_current_weather(*locations: str, unit: Literal['celsius', 'fahrenheit']):
   ```
   Only respond with your `return` value.
-  The output should be formatted as a JSON instance that conforms to the JSON schema below.
+  - The output should be formatted as a JSON instance that conforms to the JSON schema below.
   
-  As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
+  - As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
   the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.
   
-  Here is the output schema:
+  - Here is the output schema:
   ```
   {"properties": {"ret": {"title": "Ret", "type": "array", "items": {"type": "object"}}}, "required": ["ret"]}
   ```
   
   '''
 # ---
 # name: test_function_signature[get_current_weather-args6-kwargs6].1
@@ -360,20 +360,20 @@
   '''
   You are now the following python function:
   ```
   # return the given number
   def how_many(num: typing.Annotated[int, FieldInfo(default=PydanticUndefined, description='greater than 10', gt=10, extra={})]):
   ```
   Only respond with your `return` value.
-  The output should be formatted as a JSON instance that conforms to the JSON schema below.
+  - The output should be formatted as a JSON instance that conforms to the JSON schema below.
   
-  As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
+  - As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
   the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.
   
-  Here is the output schema:
+  - Here is the output schema:
   ```
   {"properties": {"ret": {"title": "Ret", "type": "integer"}}, "required": ["ret"]}
   ```
   
   '''
 # ---
 # name: test_function_signature[how_many-args8-kwargs8].1
@@ -405,20 +405,20 @@
   '''
   You are now the following python function:
   ```
   # return the person is male
   def is_male(person: gpt_fn.utils.tests.test_signature.Person):
   ```
   Only respond with your `return` value.
-  The output should be formatted as a JSON instance that conforms to the JSON schema below.
+  - The output should be formatted as a JSON instance that conforms to the JSON schema below.
   
-  As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
+  - As an example, for the schema {"properties": {"foo": {"title": "Foo", "description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}}
   the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.
   
-  Here is the output schema:
+  - Here is the output schema:
   ```
   {"properties": {"ret": {"title": "Ret", "type": "boolean"}}, "required": ["ret"]}
   ```
   
   '''
 # ---
 # name: test_function_signature[is_male-args7-kwargs7].1
```

### Comparing `gpt_fn-0.0.7/src/gpt_fn/utils/tests/test_signature.py` & `gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.7/PKG-INFO` & `gpt_fn-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-fn
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

