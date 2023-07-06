# Comparing `tmp/sweepai-0.2.4.tar.gz` & `tmp/sweepai-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.2.4.tar", max compression
+gzip compressed data, was "sweepai-0.2.5.tar", max compression
```

## Comparing `sweepai-0.2.4.tar` & `sweepai-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.4/LICENSE
--rw-r--r--   0        0        0     4221 2023-07-03 20:48:18.953249 sweepai-0.2.4/README.md
--rw-r--r--   0        0        0     1133 2023-07-03 21:08:33.771579 sweepai-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/__init__.py
--rw-r--r--   0        0        0    10664 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/api.py
--rw-r--r--   0        0        0     5893 2023-07-02 07:30:30.847953 sweepai-0.2.4/sweepai/app/api_client.py
--rw-r--r--   0        0        0     6995 2023-07-02 07:30:30.847953 sweepai-0.2.4/sweepai/app/backend.py
--rw-r--r--   0        0        0      993 2023-07-03 20:38:42.899426 sweepai-0.2.4/sweepai/app/cli.py
--rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/app/config.py
--rw-r--r--   0        0        0    10441 2023-07-03 19:27:15.637337 sweepai-0.2.4/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/core/__init__.py
--rw-r--r--   0        0        0    16077 2023-07-02 07:30:30.847953 sweepai-0.2.4/sweepai/core/chat.py
--rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     7435 2023-07-03 21:07:59.718196 sweepai-0.2.4/sweepai/core/entities.py
--rw-r--r--   0        0        0    13104 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3509 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/core/react.py
--rw-r--r--   0        0        0    16496 2023-07-03 00:51:22.966350 sweepai-0.2.4/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12030 2023-07-02 07:30:30.847953 sweepai-0.2.4/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    11178 2023-07-03 00:51:22.966350 sweepai-0.2.4/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/__init__.py
--rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/config.py
--rw-r--r--   0        0        0      670 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/utils/constants.py
--rw-r--r--   0        0        0     4072 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/utils/diff.py
--rw-r--r--   0        0        0      507 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      902 2023-07-02 07:30:30.851287 sweepai-0.2.4/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11266 2023-07-01 23:29:41.708137 sweepai-0.2.4/sweepai/utils/utils.py
--rw-r--r--   0        0        0     5286 2023-07-03 21:09:00.725748 sweepai-0.2.4/setup.py
--rw-r--r--   0        0        0     4820 2023-07-03 21:09:00.726324 sweepai-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4541 2023-07-05 21:28:16.687295 sweepai-0.2.5/README.md
+-rw-r--r--   0        0        0     1133 2023-07-06 00:20:22.834193 sweepai-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.5/sweepai/__init__.py
+-rw-r--r--   0        0        0    10754 2023-07-05 21:28:16.690628 sweepai-0.2.5/sweepai/api.py
+-rw-r--r--   0        0        0     5974 2023-07-05 23:57:08.500213 sweepai-0.2.5/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10163 2023-07-06 00:14:45.693318 sweepai-0.2.5/sweepai/app/backend.py
+-rw-r--r--   0        0        0      993 2023-07-05 21:28:16.690628 sweepai-0.2.5/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.5/sweepai/app/config.py
+-rw-r--r--   0        0        0    10897 2023-07-06 00:06:08.288163 sweepai-0.2.5/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.5/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    17168 2023-07-05 21:28:16.693961 sweepai-0.2.5/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.5/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     7435 2023-07-05 21:28:16.693961 sweepai-0.2.5/sweepai/core/entities.py
+-rw-r--r--   0        0        0    13104 2023-07-03 00:42:21.645402 sweepai-0.2.5/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3496 2023-07-05 21:28:16.693961 sweepai-0.2.5/sweepai/core/react.py
+-rw-r--r--   0        0        0    16575 2023-07-05 21:28:16.693961 sweepai-0.2.5/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12611 2023-07-05 21:28:16.693961 sweepai-0.2.5/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-07-05 21:28:16.693961 sweepai-0.2.5/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    11452 2023-07-05 21:28:16.693961 sweepai-0.2.5/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-04 07:56:27.370433 sweepai-0.2.5/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     1430 2023-07-05 21:28:16.693961 sweepai-0.2.5/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/utils/config.py
+-rw-r--r--   0        0        0      671 2023-07-06 00:14:22.909920 sweepai-0.2.5/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     4072 2023-07-03 00:42:21.645402 sweepai-0.2.5/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      719 2023-07-05 21:28:16.693961 sweepai-0.2.5/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.5/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      848 2023-07-05 21:28:16.697295 sweepai-0.2.5/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.5/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11291 2023-07-05 21:28:16.697295 sweepai-0.2.5/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     5612 2023-07-06 00:20:24.539234 sweepai-0.2.5/setup.py
+-rw-r--r--   0        0        0     5140 2023-07-06 00:20:24.539648 sweepai-0.2.5/PKG-INFO
```

### Comparing `sweepai-0.2.4/LICENSE` & `sweepai-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/README.md` & `sweepai-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 <p align="center">
     <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">
 </p>
 <p align="center">
     <i>Spend time reviewing code generated by AI, not writing it.</i>
 </p>
 
@@ -29,37 +30,40 @@
 ## 🚀 Getting Started
 
 ### 🖥️ Sweep Chat
 Sweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. 
 
 1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 
-2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or greater.
+2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.
 
 3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.
 
 4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. 
 <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">
 
 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
-2. `python sweepai/app/cli.py`. Note that you need python 3.11 or greater.
+2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.
 
 ### ✨ Sweep Github App
 Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
 
 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 2. Create new issue in repo, like "Sweep: Write tests"
 3. "👀" means it is taking a look, and it will generate the desired code
 4. "🚀" means the bot has finished its job and created a PR
 
+## 🤝 Contributing
+
+Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you'll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.
 For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).
 
 ---
 
 ## 📘 Story
 
 We were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.
@@ -93,7 +97,8 @@
     <a href="https://github.com/sweepai/sweep/graphs/contributors">
       <img src="https://contrib.rocks/image?repo=sweepai/sweep" />
     </a>
 </p>
 <p align="center">
     and, of course, Sweep!
 </p>
+
```

#### html2text {}

```diff
@@ -9,43 +9,47 @@
 4 supports --- ## â¨ Demo For the best experience, [install Sweep](https://
 github.com/apps/sweep-ai) to one of your repos and see the magic happen. [Demo]
 (https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
 0af02f2b0e47) ## ð Getting Started ### ð¥ï¸ Sweep Chat Sweep Chat allows
 you to interact with Sweep locally and will sync with GitHub. You can plan out
 your changes with Sweep, and then Sweep can create a pull request for you. 1.
 Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
-2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or
+2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or
 greater. 3. This should spin up a GitHub auth flow in your browser. Copy-paste
 the ðµ blue 8-digit code from your terminal into the page. Then wait a few
 seconds and it should spin up Sweep Chat. You should only need to do the auth
 once. 4. Pick a repo from the dropdown at the top (the Github app must be
 installed on this repo). Then start chatting with Sweep Chat. Relevant searched
 files will show up on the right. Sweep Chat can make PRs if you ask it to
 create a PR. [https://github.com/sweepai/sweep/blob/
 856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png] ð¡
 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark. ####
 From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
-`python sweepai/app/cli.py`. Note that you need python 3.11 or greater. ### â¨
+`python sweepai/app/cli.py`. Note that you need python 3.10 or greater. ### â¨
 Sweep Github App Setting up Sweep is as simple as adding the GitHub bot to a
 repo, then creating an issue for the bot to address. 1. Add the [Sweep GitHub
 app](https://github.com/apps/sweep-ai) to desired repos 2. Create new issue in
 repo, like "Sweep: Write tests" 3. "ð" means it is taking a look, and it
 will generate the desired code 4. "ð" means the bot has finished its job and
-created a PR For more detailed docs, see [ð Quickstart](https://
-docs.sweep.dev/start). --- ## ð Story We were frustrated by small tickets,
-like simple bug fixes, annoying refactors, and small features, each task
-requiring us to open our IDE to fix simple bugs. So, we decided to leverage the
-capabilities of ChatGPT to address this directly in GitHub. Unlike existing AI
-solutions, this can solve entire tickets and can be parallelized: developers
-can spin up 10 tickets and Sweep will address them all at once. ## ð The
-Stack - GPT-4 32k 0613 (default) / Claude v1.3 100k - ActiveLoop DeepLake for
-Vector DB with MiniLM L12 as our embeddings model - Modal Labs for infra +
-deployment ## ð  Features * Automatic feature development * PR auto self-
-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/
+created a PR ## ð¤ Contributing Contributions are welcome and greatly
+appreciated! For detailed guidelines on how to contribute, please see the
+[CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you'll need to fork the
+repository, create a new branch for your feature or bug fix, commit your
+changes, and open a pull request. For more detailed docs, see [ð Quickstart]
+(https://docs.sweep.dev/start). --- ## ð Story We were frustrated by small
+tickets, like simple bug fixes, annoying refactors, and small features, each
+task requiring us to open our IDE to fix simple bugs. So, we decided to
+leverage the capabilities of ChatGPT to address this directly in GitHub. Unlike
+existing AI solutions, this can solve entire tickets and can be parallelized:
+developers can spin up 10 tickets and Sweep will address them all at once. ##
+ð The Stack - GPT-4 32k 0613 (default) / Claude v1.3 100k - ActiveLoop
+DeepLake for Vector DB with MiniLM L12 as our embeddings model - Modal Labs for
+infra + deployment ## ð  Features * Automatic feature development * PR auto
+self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/
 2303.11366)) * Address developer comments after PR is created * Code snippets
 embedding-based search * Chain-of-Thought retrieval using GPT Functions ##
 ðºï¸ Roadmap We're currently working on responding to linters and external
 search. For more, see [ðºï¸ Roadmap](https://docs.sweep.dev/roadmap). ---
                            ***** Contributors *****
                        Thank you for your contribution!
                [https://contrib.rocks/image?repo=sweepai/sweep]
```

### Comparing `sweepai-0.2.4/pyproject.toml` & `sweepai-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.2.4"
+version = "0.2.5"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `sweepai-0.2.4/sweepai/api.py` & `sweepai-0.2.5/sweepai/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     PRRequest,
     ReposAddedRequest,
 )
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client, index_full_repository
 from fastapi import HTTPException, Request
 
+from pymongo import MongoClient
+
 stub = modal.Stub(API_NAME)
 image = (
     modal.Image.debian_slim()
     .apt_install("git")
     .pip_install(
         "openai",
         "anthropic",
@@ -31,38 +33,39 @@
         "docarray",
         "backoff",
         "tiktoken",
         "highlight-io",
         "GitPython",
         "posthog",
         "tqdm",
-        "pyyaml"
+        "pyyaml",
+        "pymongo"
     )
 )
 secrets = [
     modal.Secret.from_name(BOT_TOKEN_NAME),
     modal.Secret.from_name("openai-secret"),
     modal.Secret.from_name("anthropic"),
     modal.Secret.from_name("posthog"),
     modal.Secret.from_name("highlight"),
+    modal.Secret.from_name("mongodb"),
 ]
 
 FUNCTION_SETTINGS = {
     "image": image,
     "secrets": secrets,
     "timeout": 30 * 60,
 }
 
 
 handle_ticket = stub.function(**FUNCTION_SETTINGS)(on_ticket)
 handle_comment = stub.function(**FUNCTION_SETTINGS)(on_comment)
 handle_pr = stub.function(**FUNCTION_SETTINGS)(create_pr)
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
-
 @stub.function(**FUNCTION_SETTINGS)
 @modal.web_endpoint(method="POST")
 async def webhook(raw_request: Request):
     """Handle a webhook request from GitHub."""
     try:
         request_dict = await raw_request.json()
         logger.info(f"Received request: {request_dict.keys()}")
```

### Comparing `sweepai-0.2.4/sweepai/app/api_client.py` & `sweepai-0.2.5/sweepai/app/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,16 @@
             self.api_endpoint + "/search",
             json={
                 "query": query,
                 "n_results": n_results,
                 "config": self.config.dict(),
             }
         )
+        if results.status_code != 200:
+            raise Exception(results.text)
         snippets = [Snippet(**item) for item in results.json()]
         return snippets
     
     def create_pr(
         self,
         file_change_requests: list[tuple[str, str]],
         pull_request: PullRequest,
```

### Comparing `sweepai-0.2.4/sweepai/app/cli.py` & `sweepai-0.2.5/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/app/config.py` & `sweepai-0.2.5/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/app/ui.py` & `sweepai-0.2.5/sweepai/app/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
+import os
+from git import Repo
 from github import Github
 import gradio as gr
 from loguru import logger
-import webbrowser
+
 from sweepai.app.api_client import APIClient, create_pr_function, create_pr_function_call
 from sweepai.app.config import SweepChatConfig
 from sweepai.core.entities import Snippet
 
 config = SweepChatConfig.load()
 
 api_client = APIClient(config=config)
@@ -34,57 +36,70 @@
 }
 #snippets {
     height: 750px;
     overflow-y: scroll;
 }
 '''
 
-def get_files_recursively(repo, path=''):
+def get_files_recursively(root_path, path=''):
+    files = []
     path_to_contents = {}
-    try:
-        contents = repo.get_contents(path)
-        files = []
-        while contents:
-            file_content = contents.pop(0)
-            if file_content.type == 'dir':
-                contents.extend(repo.get_contents(file_content.path))
-            else:
-                try:
-                    decoded_contents = file_content.decoded_content.decode("utf-8")
-                except:
-                    continue
-                if decoded_contents:
-                    path_to_contents[file_content.path] = file_content.decoded_content.decode("utf-8")
-                    files.append(file_content.path)
-        return sorted(files), path_to_contents
-    except Exception as e:
-        logger.error(e)
-        return [], path_to_contents
+
+    if path == '.git':
+        return files, path_to_contents
+
+    current_dir = os.path.join(root_path, path)
+    entries = os.listdir(current_dir)
+
+    for entry in entries:
+        entry_path = os.path.join(current_dir, entry)
+
+        if os.path.isfile(entry_path):
+            try:
+                with open(entry_path, 'r') as file:
+                    contents = file.read()
+                path_to_contents[entry_path[len(root_path) + 1:]] = contents
+                files.append(entry_path[len(root_path) + 1:])
+            except UnicodeDecodeError as e:
+                logger.warning(f"Received warning {e}, skipping...")
+                continue
+        elif os.path.isdir(entry_path):
+            subfiles, subpath_to_contents = get_files_recursively(root_path, os.path.join(path, entry))
+            files.extend(subfiles)
+            path_to_contents.update(subpath_to_contents)
+
+    return files, path_to_contents
 
 def get_installation_id(repo_full_name):
     config.repo_full_name = repo_full_name
     api_client.config = config
     installation_id = api_client.get_installation_id()
     return installation_id
 
 path_to_contents = {}
-def get_files(name):
+def get_files(repo_full_name):
     global path_to_contents
     global repo
-    if name is None:
+    if repo_full_name is None:
         all_files = []
     else:
         # Make sure repo is added to Sweep before checking all recursive files
         try:
-            installation_id = get_installation_id(name)
+            installation_id = get_installation_id(repo_full_name)
             assert installation_id
         except:
             return []
-        repo = github_client.get_repo(name)
-        all_files, path_to_contents = get_files_recursively(repo)
+        repo = github_client.get_repo(repo_full_name)
+        repo_url = f"https://x-access-token:{config.github_pat}@github.com/{repo_full_name}.git"
+        if os.path.exists("/tmp/" + repo_full_name):
+            git_repo = Repo("/tmp/" + repo_full_name)
+            git_repo.remotes.origin.pull()
+        else:
+            Repo.clone_from(repo_url, "/tmp/" + repo_full_name)
+        all_files, path_to_contents = get_files_recursively("/tmp/" + repo_full_name)
     return all_files
 
 def get_files_update(*args):
     global repo
     if len(args) > 0:
         repo = args[0]
     else:
@@ -101,16 +116,15 @@
         repo_full_name.change(get_files_update, repo_full_name, file_names)
 
     with gr.Row():
         with gr.Column(scale=2):
             chatbot = gr.Chatbot(height=750)
         with gr.Column():
             snippets_text = gr.Markdown(value="### Relevant snippets", elem_id="snippets")
-    msg = gr.Textbox(label="Message to Sweep", placeholder="Write unit tests for OpenAI calls")
-    # clear = gr.ClearButton([msg, chatbot, snippets_text])
+    msg = gr.Textbox(label="Message to Sweep", placeholder="Send a message to Sweep")
 
     proposed_pr: str | None = None
     searched = False
     selected_snippets = []
     file_to_str = {}
 
     def repo_name_change(repo_full_name):
@@ -119,15 +133,14 @@
             installation_id = get_installation_id(repo_full_name)
             assert installation_id
             config.installation_id = installation_id
             api_client.config = config
             config.save()
             return ""
         except Exception as e:
-            webbrowser.open_new_tab("https://github.com/apps/sweep-ai")
             config.repo_full_name = None
             config.installation_id = None
             config.save()
             api_client.config = config
             raise e
 
     repo_full_name.change(repo_name_change, [repo_full_name], [msg])
```

### Comparing `sweepai-0.2.4/sweepai/core/chat.py` & `sweepai-0.2.5/sweepai/core/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import deepcopy
 import json
 import os
-from typing import Generator, Iterator, Literal, Self
+from typing import Iterator, Literal, Self
 
 import modal
 import openai
 import anthropic
 from loguru import logger
 from pydantic import BaseModel
 import backoff
@@ -17,14 +17,15 @@
 from sweepai.core.prompts import (
     system_message_prompt,
     system_message_issue_comment_prompt,
 )
 from sweepai.utils.constants import UTILS_NAME
 from sweepai.utils.prompt_constructor import HumanMessagePrompt
 from sweepai.core.entities import Message, Function
+from sweepai.utils.chat_logger import ChatLogger
 
 # TODO: combine anthropic and openai
 
 AnthropicModel = (
     Literal["claude-v1"]
     | Literal["claude-v1.3-100k"]
     | Literal["claude-instant-v1.1-100k"]
@@ -65,14 +66,15 @@
             content=system_message_prompt,
         )
     ]
     prev_message_states: list[list[Message]] = []
     model: ChatModel = "gpt-4-32k-0613"
     human_message: HumanMessagePrompt | None = None
     file_change_paths = []
+    chat_logger: ChatLogger | None = None
 
     @classmethod
     def from_system_message_content(
         cls, human_message: HumanMessagePrompt, is_reply: bool = False, **kwargs
     ) -> Self:
         if is_reply:
             system_message_content = system_message_issue_comment_prompt
@@ -140,16 +142,16 @@
         else:
             name = self.messages[-1].function_call["name"]
             self.messages.append(Message(role="function", content=content, key=message_key, name=name))
         model = model or self.model
         is_function_call = False
         if model in [args.__args__[0] for args in OpenAIModel.__args__]:
             # might be a bug here in all of this
-            response = self.call_openai(model=model, functions=functions, function_name=function_name)
             if functions:
+                response = self.call_openai(model=model, functions=functions, function_name=function_name)
                 response, is_function_call = response
                 if is_function_call:
                     self.messages.append(
                         Message(role="assistant", content=None, function_call=response, key=message_key)
                     )
                     self.prev_message_states.append(self.messages)
                     return self.messages[-1].function_call
@@ -213,37 +215,48 @@
 
             )
             def fetch():
                 global retry_counter
                 retry_counter += 1
                 token_sub = retry_counter * 200
                 try:
+                    output = None
                     if function_name:
-                        return (
+                        output = (
                             openai.ChatCompletion.create(
                                 model=model,
                                 messages=self.messages_dicts,
                                 max_tokens=max_tokens - token_sub,
                                 temperature=temperature,
                                 functions=[json.loads(function.json()) for function in functions],
                                 function_call=function_name,
                             )
                             .choices[0].message
                         )
                     else:
-                        return (
-                        openai.ChatCompletion.create(
-                            model=model,
-                            messages=self.messages_dicts,
-                            max_tokens=max_tokens - token_sub,
-                            temperature=temperature,
-                            functions=[json.loads(function.json()) for function in functions],
+                        output = (
+                            openai.ChatCompletion.create(
+                                model=model,
+                                messages=self.messages_dicts,
+                                max_tokens=max_tokens - token_sub,
+                                temperature=temperature,
+                                functions=[json.loads(function.json()) for function in functions],
+                            )
+                            .choices[0].message
                         )
-                        .choices[0].message
-                    )
+                    if self.chat_logger is not None: self.chat_logger.add_chat({
+                        'model': model,
+                        'messages': self.messages_dicts,
+                        'max_tokens': max_tokens - token_sub,
+                        'temperature': temperature,
+                        'functions': [json.loads(function.json()) for function in functions],
+                        'function_call': function_name,
+                        'output': output,
+                    })
+                    return output
                 except Exception as e:
                     logger.warning(e)
                     raise e
             result = fetch()
             if "function_call" in result:
                 result = dict(result["function_call"]), True
             else:
@@ -259,22 +272,30 @@
                 jitter=backoff.random_jitter,
             )
             def fetch():
                 global retry_counter
                 retry_counter += 1
                 token_sub = retry_counter * 200
                 try:
-                    return openai.ChatCompletion.create(
+                    output = openai.ChatCompletion.create(
                             model=model,
                             messages=self.messages_dicts,
                             max_tokens=max_tokens - token_sub,
                             temperature=temperature,
                         ) \
                         .choices[0] \
                         .message["content"]
+                    if self.chat_logger is not None: self.chat_logger.add_chat({
+                        'model': model,
+                        'messages': self.messages_dicts,
+                        'max_tokens': max_tokens - token_sub,
+                        'temperature': temperature,
+                        'output': output
+                    })
+                    return output
                 except Exception as e:
                     logger.warning(e)
                     raise e
             result = fetch()
             logger.info(f"Output to call openai:\n{result}")
             return result
```

### Comparing `sweepai-0.2.4/sweepai/core/code_repair.py` & `sweepai-0.2.5/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/core/entities.py` & `sweepai-0.2.5/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/core/prompts.py` & `sweepai-0.2.5/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/core/react.py` & `sweepai-0.2.5/sweepai/core/react.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Utils for react agent
 """
 
 import re
 from textwrap import dedent
-from typing import Callable, Concatenate
+from typing import Callable
 
 from pydantic import BaseModel
 
 REACT_INITIAL_PROMPT = """
 Gather information to solve the above problem using the tools below. 
 * You should use the tools about 2-3 times
 * Only use Finish when you are CERTAIN you have enough information to solve the problem. More information is usually better.
```

### Comparing `sweepai-0.2.4/sweepai/core/sweep_bot.py` & `sweepai-0.2.5/sweepai/core/sweep_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import github
 from github.Repository import Repository
 from github.ContentFile import ContentFile
 from github.GithubException import GithubException
 import modal
 from pydantic import BaseModel
 from sweepai.core.code_repair import CodeRepairer
+from sweepai.utils.chat_logger import ChatLogger
 
 from sweepai.core.entities import (
     FileChange,
     FileChangeRequest,
     FilesToChange,
     PullRequest,
     RegexMatchError,
@@ -97,15 +98,15 @@
 
     def get_contents(self, path: str, branch: str = ""):
         if not branch:
             branch = self.repo.default_branch
         try:
             return self.repo.get_contents(path, ref=branch)
         except Exception as e:
-            logger.error(path)
+            logger.warning(path)
             raise e
 
     def get_file(self, file_path: str, branch: str = "") -> ContentFile:
         content = self.get_contents(file_path, branch)
         assert not isinstance(content, list)
         return content
 
@@ -271,15 +272,15 @@
                     modify_file_prompt,
                     message_key=f"file_change_{file_change_request.filename}",
                 )
                 try:
                     logger.info(f"modify_file_response: {modify_file_response}")
                     new_file = generate_new_file(modify_file_response, contents)
                     if not is_markdown(file_change_request.filename):
-                        code_repairer = CodeRepairer()
+                        code_repairer = CodeRepairer(chat_logger=self.chat_logger)
                         diff = generate_diff(old_code=contents, new_code=new_file)
                         new_file = code_repairer.repair_code(diff=diff, user_code=new_file, feature=file_change_request.instructions)
                     return (new_file, file_change_request.filename)
                 except Exception as e:
                     logger.warning(f"Recieved error {e}")
                     logger.warning(
                         f"Failed to parse. Retrying for the {count}th time..."
```

### Comparing `sweepai-0.2.4/sweepai/core/vector_db.py` & `sweepai-0.2.5/sweepai/core/vector_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 DEEPLAKE_DIR = "/root/cache/"
 DISKCACHE_DIR = "/root/cache/diskcache/"
 DEEPLAKE_FOLDER = "deeplake/"
 BATCH_SIZE = 256
 SENTENCE_TRANSFORMERS_MODEL = "sentence-transformers/all-MiniLM-L12-v2"
 timeout = 60 * 30 # 30 minutes
 CACHE_VERSION = "v1.0.0"
+MAX_FILES = 3000
 
 image = (
     modal.Image.debian_slim()
     .apt_install("git")
     .pip_install("deeplake==3.6.3", "sentence-transformers")
     .pip_install("openai", "PyGithub", "loguru", "docarray", "GitPython", "tqdm", "highlight-io", "anthropic", "posthog", "redis", "pyyaml")
 )
@@ -67,15 +68,15 @@
     name = re.sub(r"^(-*\w{0,61}\w)-*$", r"\1", name[:63].ljust(3, "x"))
     return name
 
 @stub.cls(
     image=image,
     secrets=secrets,
     shared_volumes={MODEL_DIR: model_volume},
-    keep_warm=2,
+    keep_warm=1 if ENV == "prod" else 0,
     gpu="T4",
     retries=modal.Retries(max_retries=5, backoff_coefficient=2, initial_delay=5),
 )
 class Embedding:
     def __enter__(self):
         from sentence_transformers import SentenceTransformer
 
@@ -181,20 +182,32 @@
                 contents = file + contents
             except UnicodeDecodeError as e:
                 logger.warning(f"Received warning {e}, skipping...")
                 continue
             file_path = file[len("repo/") :]
             file_paths.append(file_path)
             file_contents.append(contents)
+            if len(file_list) > MAX_FILES:
+                scores.append(1)
+                continue
             try:
+                cache_key = f"{repo_name}-{file_path}-{CACHE_VERSION}"
+                if cache_success:
+                    cached_value = cache.get(cache_key)
+                    if cached_value:
+                        score = json.loads(cached_value)
+                        scores.append(score)
+                        continue
                 commits = list(repo.get_commits(path=file_path, sha=branch_name))
-                score, logit = compute_score(contents, commits)
+                score = compute_score(contents, commits)
+                if cache_success:
+                    cache.set(cache_key, json.dumps(score), ex=60 * 60 * 2)
                 scores.append(score)
             except Exception as e:
-                logger.warning(f"Received warning {e}, skipping...")
+                logger.warning(f"Received warning during scoring {e}, skipping...")
                 scores.append(1)
                 continue
     scores = convert_to_percentiles(scores)
         
     chunked_results = chunker.map(file_contents, file_paths, scores, kwargs={
         "additional_metadata": {"repo_name": repo_name, "branch_name": branch_name}
     })
@@ -221,15 +234,15 @@
                         sha):
     deeplake_vs = init_deeplake_vs(collection_name)
     if len(documents) > 0:
         logger.info("Computing embeddings...")
         # Check cache here for all documents
         embeddings = [None] * len(documents)
         if cache_success:
-            cache_keys = [hash_sha256(doc) + SENTENCE_TRANSFORMERS_MODEL + sha + CACHE_VERSION for doc in documents]
+            cache_keys = [hash_sha256(doc) + SENTENCE_TRANSFORMERS_MODEL + CACHE_VERSION for doc in documents]
             cache_values = cache.mget(cache_keys)
             for idx, value in enumerate(cache_values):
                 if value is not None:
                     embeddings[idx] = json.loads(value)
         logger.info(f"Found {len([x for x in embeddings if x is not None])} embeddings in cache")
         indices_to_compute = [idx for idx, x in enumerate(embeddings) if x is None]
         documents_to_compute = [documents[idx] for idx in indices_to_compute]
@@ -242,15 +255,15 @@
             text = ids,
             embedding = embeddings,
             metadata = metadatas
         )
         if cache_success: cache.set(f"github-{sha}{CACHE_VERSION}", json.dumps({"metadatas": metadatas, "ids": ids, "embeddings": embeddings}))
         if cache_success and len(documents_to_compute) > 0:
             logger.info(f"Updating cache with {len(computed_embeddings)} embeddings")
-            cache_keys = [hash_sha256(doc) + SENTENCE_TRANSFORMERS_MODEL + sha + CACHE_VERSION for doc in documents_to_compute]
+            cache_keys = [hash_sha256(doc) + SENTENCE_TRANSFORMERS_MODEL + CACHE_VERSION for doc in documents_to_compute]
             cache.mset({key: json.dumps(value) for key, value in zip(cache_keys, computed_embeddings)})
         return deeplake_vs
     else:
         logger.error("No documents found in repository")
         return deeplake_vs
```

### Comparing `sweepai-0.2.4/sweepai/events.py` & `sweepai-0.2.5/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/handlers/create_pr.py` & `sweepai-0.2.5/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/handlers/on_comment.py` & `sweepai-0.2.5/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/handlers/on_review.py` & `sweepai-0.2.5/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/handlers/on_ticket.py` & `sweepai-0.2.5/sweepai/handlers/on_ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from sweepai.handlers.create_pr import create_pr
 from sweepai.handlers.on_comment import on_comment
 from sweepai.handlers.on_review import review_pr
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client, search_snippets
 from sweepai.utils.prompt_constructor import HumanMessagePrompt
 from sweepai.utils.constants import DB_NAME, PREFIX, UTILS_NAME
+from sweepai.utils.chat_logger import ChatLogger
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
 bot_suffix = "I'm a bot that handles simple bugs and feature requests \
@@ -194,16 +195,24 @@
         username=username,
         repo_description=repo_description,
         title=title,
         summary=summary + replies_text,
         snippets=snippets,
         tree=tree, # TODO: Anything in repo tree that has something going through is expanded
     )
+
+    chat_logger = ChatLogger({
+        'repo_name': repo_name,
+        'issue_url': issue_url,
+        'username': username,
+        'title': title,
+        'summary': summary + replies_text,
+    })
     sweep_bot = SweepBot.from_system_message_content(
-        human_message=human_message, repo=repo, is_reply=bool(comments)
+        human_message=human_message, repo=repo, is_reply=bool(comments), chat_logger=chat_logger
     )
     sweepbot_retries = 3
     try:
         for i in range(sweepbot_retries):
             logger.info("CoT retrieval...")
             if sweep_bot.model == "gpt-4-32k-0613":
                 sweep_bot.cot_retrieval()
```

### Comparing `sweepai-0.2.4/sweepai/slack.py` & `sweepai-0.2.5/sweepai/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/utils/constants.py` & `sweepai-0.2.5/sweepai/utils/constants.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     SWEEP_LOGIN = "sweep-canary[bot]"
 elif PREFIX == "dev":
     APP_ID = 324098
     ENV = PREFIX
     SWEEP_LOGIN = "sweep-nightly[bot]"
 LABEL_NAME = "sweep"
 LABEL_COLOR = "#9400D3"
-LABEL_DESCRIPTION = "Sweep your software chores"
+LABEL_DESCRIPTION = "Sweep your software chores"
```

### Comparing `sweepai-0.2.4/sweepai/utils/diff.py` & `sweepai-0.2.5/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/utils/file_change_functions.py` & `sweepai-0.2.5/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/utils/github_utils.py` & `sweepai-0.2.5/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/utils/huggingface.py` & `sweepai-0.2.5/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/utils/prompt_constructor.py` & `sweepai-0.2.5/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/utils/scorer.py` & `sweepai-0.2.5/sweepai/utils/scorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 def compute_score(contents, commits):
     line_count = contents.count("\n") 
     if line_count > 200:
         line_count_score = 10
     else:
         line_count_score = line_count / 20
     commit_count = len(commits) + 1
-    days_since_last_modified = ((datetime.now() - commits[0].commit.author.date).total_seconds() // 3600) + 1
-    return (line_count_score * commit_count / days_since_last_modified), (line_count_score, commit_count, days_since_last_modified)
+    days_since_last_modified = max(((datetime.now() - commits[0].commit.author.date).total_seconds() // 3600), 0) + 1
+    return (line_count_score * commit_count / days_since_last_modified)
 
 def convert_to_percentiles(values):
     sorted_values = sorted(values)  # Sort the values in ascending order
     n = len(sorted_values)
     max_percentile = .25
-    percentile_mapping = {value: (i / (n-1)) * max_percentile for i, value in enumerate(sorted_values)}
+    percentile_mapping = {value: (i / (n)) * max_percentile for i, value in enumerate(sorted_values)}
     percentiles = [percentile_mapping[value] for value in values]  # Create the percentiles list based on the mapping
 
     return percentiles
```

### Comparing `sweepai-0.2.4/sweepai/utils/snippets.py` & `sweepai-0.2.5/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.4/sweepai/utils/utils.py` & `sweepai-0.2.5/sweepai/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,26 +141,27 @@
     "md": "markdown",
     "rst": "markdown",
     "txt": "markdown",
     "erb": "embedded-template",
     "ejs": "embedded-template",
     "html": "embedded-template",
     "vue": "vue",
+    "php": "php",
 }
 
 @stub.cls(
     image=chunking_image, 
     shared_volumes={CHUNKING_CACHE_DIR: chunking_volume},
 )
 class Chunking:
 
     def __enter__(self):
         from tree_sitter import Language
 
-        LANGUAGE_NAMES = ["python", "java", "cpp", "go", "rust", "ruby"]
+        LANGUAGE_NAMES = ["python", "java", "cpp", "go", "rust", "ruby", "php"]
         for language in LANGUAGE_NAMES:
             subprocess.run(f"git clone https://github.com/tree-sitter/tree-sitter-{language} cache/tree-sitter-{language}", shell=True)
         for language in LANGUAGE_NAMES:
             Language.build_library(f'cache/build/{language}.so', [f"cache/tree-sitter-{language}"]) 
             subprocess.run(f"cp cache/build/{language}.so /tmp/{language}.so", shell=True) # copying for executability
         self.languages = {language: Language(f"/tmp/{language}.so", language) for language in LANGUAGE_NAMES}
```

### Comparing `sweepai-0.2.4/setup.py` & `sweepai-0.2.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Sweep software chores',
-    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">\n</p>\n<p align="center">\n    <i>Spend time reviewing code generated by AI, not writing it.</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev/">🌐 Website</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://docs.sweep.dev/">📚 Docs</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://discord.gg/sweep-ai">📢 Discord</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.11 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n\n## 🌠 Features\n* Automatic feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
+    'long_description': '\n<p align="center">\n    <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">\n</p>\n<p align="center">\n    <i>Spend time reviewing code generated by AI, not writing it.</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev/">🌐 Website</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://docs.sweep.dev/">📚 Docs</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://discord.gg/sweep-ai">📢 Discord</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you\'ll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n\n## 🌠 Features\n* Automatic feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['PyGithub==1.58.2', 'config-
 path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0',
 'requests>=2.28.2,<3.0.0', 'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0']
 entry_points = \ {'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai =
-sweepai.app.cli:app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.2.4',
-'description': 'Sweep software chores', 'long_description': '
+sweepai.app.cli:app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.2.5',
+'description': 'Sweep software chores', 'long_description': '\n
                   \n [https://github.com/sweepai/sweep/blob/
   856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]\n
 \n
         \n Spend time reviewing code generated by AI, not writing it.\n
 \n\n
           \nð_Website\n  â¢  \nð_Docs\n  â¢  \nð¢_Discord\n
 \n\nSweep allows you to create and review GitHub issues with ease.\nSimply
@@ -20,51 +20,56 @@
 Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic
 happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-
 7317-40a7-9b5e-0af02f2b0e47)\n\n## ð Getting Started\n\n### ð¥ï¸ Sweep
 Chat\nSweep Chat allows you to interact with Sweep locally and will sync with
 GitHub. You can plan out your changes with Sweep, and then Sweep can create a
 pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/
 apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note
-that you need python 3.11 or greater.\n\n3. This should spin up a GitHub auth
+that you need python 3.10 or greater.\n\n3. This should spin up a GitHub auth
 flow in your browser. Copy-paste the ðµ blue 8-digit code from your terminal
 into the page. Then wait a few seconds and it should spin up Sweep Chat. You
 should only need to do the auth once.\n\n4. Pick a repo from the dropdown at
 the top (the Github app must be installed on this repo). Then start chatting
 with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat
 can make PRs if you ask it to create a PR. \n[https://github.com/sweepai/sweep/
 blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
 screenshot.png]\n\nð¡ You can force dark mode by going to http://127.0.0.1:
 7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or
 if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/
 sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need
-python 3.11 or greater.\n\n### â¨ Sweep Github App\nSetting up Sweep is as
+python 3.10 or greater.\n\n### â¨ Sweep Github App\nSetting up Sweep is as
 simple as adding the GitHub bot to a repo, then creating an issue for the bot
 to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai)
 to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3.
 "ð" means it is taking a look, and it will generate the desired code\n4.
-"ð" means the bot has finished its job and created a PR\n\nFor more detailed
-docs, see [ð Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## ð
-Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying
-refactors, and small features, each task requiring us to open our IDE to fix
-simple bugs. So, we decided to leverage the capabilities of ChatGPT to address
-this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire
-tickets and can be parallelized: developers can spin up 10 tickets and Sweep
-will address them all at once.\n\n## ð The Stack\n- GPT-4 32k 0613 (default)
-/ Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our
-embeddings model\n- Modal Labs for infra + deployment\n\n## ð  Features\n*
-Automatic feature development\n* PR auto self-review + comment handling
-(effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address
-developer comments after PR is created\n* Code snippets embedding-based
-search\n* Chain-of-Thought retrieval using GPT Functions\n\n## ðºï¸
-Roadmap\nWe\'re currently working on responding to linters and external search.
-For more, see [ðºï¸ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n
+"ð" means the bot has finished its job and created a PR\n\n## ð¤
+Contributing\n\nContributions are welcome and greatly appreciated! For detailed
+guidelines on how to contribute, please see the [CONTRIBUTING.md]
+(CONTRIBUTING.md) file. In essence, you\'ll need to fork the repository, create
+a new branch for your feature or bug fix, commit your changes, and open a pull
+request.\nFor more detailed docs, see [ð Quickstart](https://docs.sweep.dev/
+start).\n\n---\n\n## ð Story\n\nWe were frustrated by small tickets, like
+simple bug fixes, annoying refactors, and small features, each task requiring
+us to open our IDE to fix simple bugs. So, we decided to leverage the
+capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing
+AI solutions, this can solve entire tickets and can be parallelized: developers
+can spin up 10 tickets and Sweep will address them all at once.\n\n## ð The
+Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for
+Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra +
+deployment\n\n## ð  Features\n* Automatic feature development\n* PR auto
+self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/
+2303.11366))\n* Address developer comments after PR is created\n* Code snippets
+embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n##
+ðºï¸ Roadmap\nWe\'re currently working on responding to linters and external
+search. For more, see [ðºï¸ Roadmap](https://docs.sweep.dev/roadmap).\n\n---
+\n\n
                          ***** \n Contributors\n *****
 \n
                      \n Thank you for your contribution!\n
 \n
           \n \n_[https://contrib.rocks/image?repo=sweepai/sweep]\n\n
 \n
                           \n and, of course, Sweep!\n
-\n', 'author': 'Kevin Lu', 'author_email': None, 'maintainer': None,
+\n\n', 'author': 'Kevin Lu', 'author_email': None, 'maintainer': None,
 'maintainer_email': None, 'url': None, 'packages': packages, 'package_data':
 package_data, 'install_requires': install_requires, 'entry_points':
 entry_points, 'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `sweepai-0.2.4/PKG-INFO` & `sweepai-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.2.4
+Version: 0.2.5
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.58.2)
@@ -12,14 +12,15 @@
 Requires-Dist: gradio (>=3.35.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
+
 <p align="center">
     <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">
 </p>
 <p align="center">
     <i>Spend time reviewing code generated by AI, not writing it.</i>
 </p>
 
@@ -47,37 +48,40 @@
 ## 🚀 Getting Started
 
 ### 🖥️ Sweep Chat
 Sweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. 
 
 1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 
-2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or greater.
+2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.
 
 3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.
 
 4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. 
 <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">
 
 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
-2. `python sweepai/app/cli.py`. Note that you need python 3.11 or greater.
+2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.
 
 ### ✨ Sweep Github App
 Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
 
 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 2. Create new issue in repo, like "Sweep: Write tests"
 3. "👀" means it is taking a look, and it will generate the desired code
 4. "🚀" means the bot has finished its job and created a PR
 
+## 🤝 Contributing
+
+Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you'll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.
 For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).
 
 ---
 
 ## 📘 Story
 
 We were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.
@@ -112,7 +116,8 @@
       <img src="https://contrib.rocks/image?repo=sweepai/sweep" />
     </a>
 </p>
 <p align="center">
     and, of course, Sweep!
 </p>
 
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.2.4 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.2.5 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: PyGithub
 (==1.58.2) Requires-Dist: config-path (>=1.0.3,<2.0.0) Requires-Dist: gradio
 (>=3.35.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
 requests (>=2.28.2,<3.0.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-
 Dist: urllib3 (>=2.0.3,<3.0.0) Description-Content-Type: text/markdown
@@ -17,43 +17,47 @@
 4 supports --- ## â¨ Demo For the best experience, [install Sweep](https://
 github.com/apps/sweep-ai) to one of your repos and see the magic happen. [Demo]
 (https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
 0af02f2b0e47) ## ð Getting Started ### ð¥ï¸ Sweep Chat Sweep Chat allows
 you to interact with Sweep locally and will sync with GitHub. You can plan out
 your changes with Sweep, and then Sweep can create a pull request for you. 1.
 Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
-2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or
+2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or
 greater. 3. This should spin up a GitHub auth flow in your browser. Copy-paste
 the ðµ blue 8-digit code from your terminal into the page. Then wait a few
 seconds and it should spin up Sweep Chat. You should only need to do the auth
 once. 4. Pick a repo from the dropdown at the top (the Github app must be
 installed on this repo). Then start chatting with Sweep Chat. Relevant searched
 files will show up on the right. Sweep Chat can make PRs if you ask it to
 create a PR. [https://github.com/sweepai/sweep/blob/
 856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png] ð¡
 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark. ####
 From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
-`python sweepai/app/cli.py`. Note that you need python 3.11 or greater. ### â¨
+`python sweepai/app/cli.py`. Note that you need python 3.10 or greater. ### â¨
 Sweep Github App Setting up Sweep is as simple as adding the GitHub bot to a
 repo, then creating an issue for the bot to address. 1. Add the [Sweep GitHub
 app](https://github.com/apps/sweep-ai) to desired repos 2. Create new issue in
 repo, like "Sweep: Write tests" 3. "ð" means it is taking a look, and it
 will generate the desired code 4. "ð" means the bot has finished its job and
-created a PR For more detailed docs, see [ð Quickstart](https://
-docs.sweep.dev/start). --- ## ð Story We were frustrated by small tickets,
-like simple bug fixes, annoying refactors, and small features, each task
-requiring us to open our IDE to fix simple bugs. So, we decided to leverage the
-capabilities of ChatGPT to address this directly in GitHub. Unlike existing AI
-solutions, this can solve entire tickets and can be parallelized: developers
-can spin up 10 tickets and Sweep will address them all at once. ## ð The
-Stack - GPT-4 32k 0613 (default) / Claude v1.3 100k - ActiveLoop DeepLake for
-Vector DB with MiniLM L12 as our embeddings model - Modal Labs for infra +
-deployment ## ð  Features * Automatic feature development * PR auto self-
-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/
+created a PR ## ð¤ Contributing Contributions are welcome and greatly
+appreciated! For detailed guidelines on how to contribute, please see the
+[CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you'll need to fork the
+repository, create a new branch for your feature or bug fix, commit your
+changes, and open a pull request. For more detailed docs, see [ð Quickstart]
+(https://docs.sweep.dev/start). --- ## ð Story We were frustrated by small
+tickets, like simple bug fixes, annoying refactors, and small features, each
+task requiring us to open our IDE to fix simple bugs. So, we decided to
+leverage the capabilities of ChatGPT to address this directly in GitHub. Unlike
+existing AI solutions, this can solve entire tickets and can be parallelized:
+developers can spin up 10 tickets and Sweep will address them all at once. ##
+ð The Stack - GPT-4 32k 0613 (default) / Claude v1.3 100k - ActiveLoop
+DeepLake for Vector DB with MiniLM L12 as our embeddings model - Modal Labs for
+infra + deployment ## ð  Features * Automatic feature development * PR auto
+self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/
 2303.11366)) * Address developer comments after PR is created * Code snippets
 embedding-based search * Chain-of-Thought retrieval using GPT Functions ##
 ðºï¸ Roadmap We're currently working on responding to linters and external
 search. For more, see [ðºï¸ Roadmap](https://docs.sweep.dev/roadmap). ---
                            ***** Contributors *****
                        Thank you for your contribution!
                [https://contrib.rocks/image?repo=sweepai/sweep]
```

