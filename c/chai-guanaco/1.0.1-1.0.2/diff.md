# Comparing `tmp/chai-guanaco-1.0.1.tar.gz` & `tmp/chai-guanaco-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chai-guanaco-1.0.1.tar", last modified: Tue Jul  4 20:10:36 2023, max compression
+gzip compressed data, was "dist/chai-guanaco-1.0.2.tar", last modified: Thu Jul  6 19:39:29 2023, max compression
```

## Comparing `chai-guanaco-1.0.1.tar` & `chai-guanaco-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,42 @@
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/
--rw-rw-r--   0 tom       (1002) tom       (1002)     9561 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     8091 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/README.md
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/
--rw-rw-r--   0 tom       (1002) tom       (1002)     9561 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)      644 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/not-zip-safe
--rw-rw-r--   0 tom       (1002) tom       (1002)       22 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/requires.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       22 2023-07-04 18:16:45.000000 chai-guanaco-1.0.1/requirements.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/setup.cfg
--rw-rw-r--   0 tom       (1002) tom       (1002)      925 2023-07-04 20:10:31.000000 chai-guanaco-1.0.1/setup.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/src/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/src/chai_guanaco/
--rw-rw-r--   0 tom       (1002) tom       (1002)      188 2023-07-04 18:51:04.000000 chai-guanaco-1.0.1/src/chai_guanaco/__init__.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3220 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/src/chai_guanaco/feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-04 18:51:57.000000 chai-guanaco-1.0.1/src/chai_guanaco/login_cli.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     6659 2023-07-04 20:06:57.000000 chai-guanaco-1.0.1/src/chai_guanaco/submit.py
--rw-rw-r--   0 tom       (1002) tom       (1002)      496 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/src/chai_guanaco/utils.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/tests/
--rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.1/tests/test_feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/tests/test_login.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     6235 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/tests/test_submit.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/
+-rw-rw-r--   0 tom       (1002) tom       (1002)    10663 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     8969 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/README.md
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/
+-rw-rw-r--   0 tom       (1002) tom       (1002)    10663 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1221 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/not-zip-safe
+-rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/requirements.txt
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/resources/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/resources/bot_config/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/blade.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/captain_wyatt.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/coffee_shop_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/filbert.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/leo.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/levi.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/mr_wilson.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/nerd_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/scaramouche.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/story_teller.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/vampire_queen.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/wednesday_addams.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/setup.cfg
+-rw-rw-r--   0 tom       (1002) tom       (1002)      925 2023-07-06 19:39:17.000000 chai-guanaco-1.0.2/setup.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/src/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/src/chai_guanaco/
+-rw-rw-r--   0 tom       (1002) tom       (1002)      224 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/src/chai_guanaco/__init__.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     4853 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/src/chai_guanaco/chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3220 2023-07-04 17:14:25.000000 chai-guanaco-1.0.2/src/chai_guanaco/feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/src/chai_guanaco/formatters.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-06 19:37:53.000000 chai-guanaco-1.0.2/src/chai_guanaco/login_cli.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6659 2023-07-06 19:37:53.000000 chai-guanaco-1.0.2/src/chai_guanaco/submit.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)      496 2023-07-04 17:14:25.000000 chai-guanaco-1.0.2/src/chai_guanaco/utils.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/tests/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/tests/test_chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.2/tests/test_feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-04 17:14:25.000000 chai-guanaco-1.0.2/tests/test_login.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6235 2023-07-04 17:14:25.000000 chai-guanaco-1.0.2/tests/test_submit.py
```

### Comparing `chai-guanaco-1.0.1/PKG-INFO` & `chai-guanaco-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.1
+Version: 1.0.2
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
         [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
         [![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
         
         [Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
         
-        It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](https://apps.apple.com/us/app/chai-chat-with-ai-bots/id1544750895) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+        It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](http://tosto.re/chaiapp) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+        
+        ## Quick Start
+        
+        [Chai Guanaco Jupyter Notebook Quickstart](https://datalore.jetbrains.com/notebook/ABxxIKqVGejPnF8zH6zFpx/WQd6vDlfCDux5wzuoAeF8m)
         
         
         ## The Guanaco Guide
         
         🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
         
         🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
@@ -79,14 +83,38 @@
         submitter = chai.ModelSubmitter()
         submission_id = submitter.submit(submission_parameters)
         ````
         
         This will display an animation while your model is being deployed, a typical
         deployment takes approximately 10 minutes.
         
+        
+        **Chat With Your Model Submission**
+        
+        Once your model is deployed, you can verify its behaviour and raw input by running:
+        
+        ```python
+        chatbot = chai.ChatWithSubmission(submission_id)
+        chatbot.chat('nerd_girl', show_model_input=False)
+        ```
+        
+        Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
+        
+        You can get a list of avaliable bots by running:
+        
+        ```python
+        chatbot.show_avaliable_bots()
+        ```
+        
+        Finally, to enter a chat session that prints out the raw input that was fed into your model at each turn of the conversation, you can run:
+        
+        ```python
+        chatbot.chat('nerd_girl', show_model_input=True)
+        ```
+        
         **Getting User Feedback**
         
         Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
         
         ```python
         model_feedback = chai.get_feedback(submission_id)
         model_feedback.sample()
```

### Comparing `chai-guanaco-1.0.1/README.md` & `chai-guanaco-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
 
 [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 [![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
 
 [Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
 
-It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](https://apps.apple.com/us/app/chai-chat-with-ai-bots/id1544750895) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](http://tosto.re/chaiapp) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+
+## Quick Start
+
+[Chai Guanaco Jupyter Notebook Quickstart](https://datalore.jetbrains.com/notebook/ABxxIKqVGejPnF8zH6zFpx/WQd6vDlfCDux5wzuoAeF8m)
 
 
 ## The Guanaco Guide
 
 🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
 
 🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
@@ -71,14 +75,38 @@
 submitter = chai.ModelSubmitter()
 submission_id = submitter.submit(submission_parameters)
 ````
 
 This will display an animation while your model is being deployed, a typical
 deployment takes approximately 10 minutes.
 
+
+**Chat With Your Model Submission**
+
+Once your model is deployed, you can verify its behaviour and raw input by running:
+
+```python
+chatbot = chai.ChatWithSubmission(submission_id)
+chatbot.chat('nerd_girl', show_model_input=False)
+```
+
+Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
+
+You can get a list of avaliable bots by running:
+
+```python
+chatbot.show_avaliable_bots()
+```
+
+Finally, to enter a chat session that prints out the raw input that was fed into your model at each turn of the conversation, you can run:
+
+```python
+chatbot.chat('nerd_girl', show_model_input=True)
+```
+
 **Getting User Feedback**
 
 Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
 
 ```python
 model_feedback = chai.get_feedback(submission_id)
 model_feedback.sample()
```

### Comparing `chai-guanaco-1.0.1/chai_guanaco.egg-info/PKG-INFO` & `chai-guanaco-1.0.2/chai_guanaco.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.1
+Version: 1.0.2
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
         [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
         [![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
         
         [Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
         
-        It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](https://apps.apple.com/us/app/chai-chat-with-ai-bots/id1544750895) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+        It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](http://tosto.re/chaiapp) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+        
+        ## Quick Start
+        
+        [Chai Guanaco Jupyter Notebook Quickstart](https://datalore.jetbrains.com/notebook/ABxxIKqVGejPnF8zH6zFpx/WQd6vDlfCDux5wzuoAeF8m)
         
         
         ## The Guanaco Guide
         
         🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
         
         🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
@@ -79,14 +83,38 @@
         submitter = chai.ModelSubmitter()
         submission_id = submitter.submit(submission_parameters)
         ````
         
         This will display an animation while your model is being deployed, a typical
         deployment takes approximately 10 minutes.
         
+        
+        **Chat With Your Model Submission**
+        
+        Once your model is deployed, you can verify its behaviour and raw input by running:
+        
+        ```python
+        chatbot = chai.ChatWithSubmission(submission_id)
+        chatbot.chat('nerd_girl', show_model_input=False)
+        ```
+        
+        Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
+        
+        You can get a list of avaliable bots by running:
+        
+        ```python
+        chatbot.show_avaliable_bots()
+        ```
+        
+        Finally, to enter a chat session that prints out the raw input that was fed into your model at each turn of the conversation, you can run:
+        
+        ```python
+        chatbot.chat('nerd_girl', show_model_input=True)
+        ```
+        
         **Getting User Feedback**
         
         Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
         
         ```python
         model_feedback = chai.get_feedback(submission_id)
         model_feedback.sample()
```

### Comparing `chai-guanaco-1.0.1/setup.py` & `chai-guanaco-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 if os.environ.get('CI_COMMIT_TAG', None):
     version = os.environ['CI_COMMIT_TAG']
 else:
-    version = "1.0.1"
+    version = "1.0.2"
 
 setup(
     name='chai-guanaco',
     version=version,
     description='Chai Guanaco',
     author='Chai Research Corp.',
     author_email='hello@chai-research.com',
```

### Comparing `chai-guanaco-1.0.1/src/chai_guanaco/feedback.py` & `chai-guanaco-1.0.2/src/chai_guanaco/feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.1/src/chai_guanaco/login_cli.py` & `chai-guanaco-1.0.2/src/chai_guanaco/login_cli.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.1/src/chai_guanaco/submit.py` & `chai-guanaco-1.0.2/src/chai_guanaco/submit.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.1/tests/test_feedback.py` & `chai-guanaco-1.0.2/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.1/tests/test_login.py` & `chai-guanaco-1.0.2/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.1/tests/test_submit.py` & `chai-guanaco-1.0.2/tests/test_submit.py`

 * *Files identical despite different names*

