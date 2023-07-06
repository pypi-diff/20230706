# Comparing `tmp/aicodebot-0.8.0.tar.gz` & `tmp/aicodebot-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.8.0.tar", last modified: Tue Jul  4 02:39:29 2023, max compression
+gzip compressed data, was "aicodebot-0.8.1.tar", last modified: Thu Jul  6 18:59:25 2023, max compression
```

## Comparing `aicodebot-0.8.0.tar` & `aicodebot-0.8.1.tar`

### file list

```diff
@@ -1,28 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:39:29.120513 aicodebot-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-04 02:39:00.000000 aicodebot-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-07-04 02:39:29.120513 aicodebot-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-04 02:39:00.000000 aicodebot-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:39:29.120513 aicodebot-0.8.0/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)    16438 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:39:29.120513 aicodebot-0.8.0/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/prompts/review.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 02:39:00.000000 aicodebot-0.8.0/aicodebot/prompts/sidekick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:39:29.120513 aicodebot-0.8.0/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-07-04 02:39:29.000000 aicodebot-0.8.0/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-04 02:39:29.000000 aicodebot-0.8.0/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 02:39:29.000000 aicodebot-0.8.0/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 02:39:29.000000 aicodebot-0.8.0/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 02:39:29.000000 aicodebot-0.8.0/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 02:39:29.000000 aicodebot-0.8.0/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-04 02:39:00.000000 aicodebot-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 02:39:29.120513 aicodebot-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-04 02:39:00.000000 aicodebot-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:59:25.817928 aicodebot-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-06 18:58:52.000000 aicodebot-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-06 18:59:25.817928 aicodebot-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-07-06 18:58:52.000000 aicodebot-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:59:25.817928 aicodebot-0.8.1/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:59:25.817928 aicodebot-0.8.1/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-06 18:58:52.000000 aicodebot-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:59:25.817928 aicodebot-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 18:58:52.000000 aicodebot-0.8.1/setup.py
```

### Comparing `aicodebot-0.8.0/LICENSE` & `aicodebot-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.0/PKG-INFO` & `aicodebot-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.8.0
+Version: 0.8.1
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -15,60 +15,63 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AI Code Bot 🤖
 
 ## Your AI-powered coding sidekick
 
-AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
+AICodeBot is a coding assistant designed to make your coding life easier. Think of it as your AI version of a pair programmer. Perform code reviews, create helpful commit messages, debug problems, and help you think through building new features. A team member that accelerates the pace of development and helps you write better code.
 
-We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
+We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/). In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features.
+Status: This project is in its early stages with limited features, but it already improves the software development workflow, and has a healthy roadmap of features (below).
 
-⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent. Much like Tesla's Full Self Driving, you have to keep your hands on the wheel.
+We're using AICodeBot to build AICodeBot, and it's upward spiraling all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
-We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
-
-### What it's not
+### What it's NOT
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
-It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
+⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes AICodeBot does dumb things, which is why it's mostly *reading* and *advising* and not yet *writing*. Much like Tesla's "Full Self Driving", you have to keep your hands on the wheel.
+
+It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that. It's not a no-code platform. Instead, AICodeBot is built to work with existing code bases and the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it today
 
-### AI Sidekick
+### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
  ```bash
  aicodebot sidekick file1.py file2.py
  ```
 
 In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers. For example:
 
 * How can I make this code better?
 * Tell me how to add a new feature to this code.
-* Fix an issue that I'm having when... (describe the issue)
+* Fix an issue that I'm having... (paste the error, stack trace, etc.)
 * Write unit tests for the xyz function.
 
-Please note that this feature is still in its experimental stage. While it can already provide valuable assistance, it's not perfect and we're continuously working on improving it.
+Pro-tip: add your README.md to the list of files to get context-aware answers.
+
+This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingeseting repo specific domain knowledge, writing local files, and more.
 
-### AI-Assisted Git Commit
+### AI-Assisted Git Commit 📝
 
-`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
+`aicodebot commit` improves the git commit process. It will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
 
-### AI-Assisted Code Review
+### AI-Assisted Code Review 👀
 
-`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code and makes us better programmers. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
+`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review.
+It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code and makes us better programmers. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
 
-### AI-Assisted Debugging
+### AI-Assisted Debugging 🐞
 
-`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, command output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
+`aicodebot debug $command` will run the command and capture the log output. It will pass the error message, stack trace, command output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to Stack Overflow in a separate window, allowing you to stay in terminal with all the context.
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg?0.6.2)](https://badge.fury.io/py/aicodebot)
 
 ## Installation and Usage
 
 To install AICodeBot, run:
 
@@ -85,59 +88,60 @@
 
 Commands:
   alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
   commit     Generate a commit message based on your changes.
   debug      Run a command and debug the output.
   fun-fact   Get a fun fact about programming and artificial intelligence.
   review     Do a code review, with [un]staged changes, or a specified...
+  sidekick   EXPERIMENTAL: Coding help from your AI sidekick
   ```
 
 ### Open AI key setup
 
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
 #### Which Language Model? GPT-3.5 vs GPT-4
 
 When using AICodeBot, you have the option to use either GPT-3.5 or GPT-4. While GPT-4 can often provide more accurate and detailed responses, GPT-3.5 is faster and might be sufficient for simpler tasks. We highly recommend GPT-4.
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
 Note: We'll be adding more options for AI models in the future, including those that can be run locally, such as [GPT4all](https://gpt4all.io/) and HuggingFace's [Transformers](https://huggingface.co/transformers/).
 
-## Roadmap of Upcoming Features
+## Roadmap of Upcoming Features ️
 
 ### Code Workflow Improvements
 
 * [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
 * [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
 * [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
 * [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
 * [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 * [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
 * [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
 * [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
-* [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
+* [X] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
 * [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
 * [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
 * [ ] **Automatically Generate ChangeLogs and Release Notes**: Generates release notes and changelogs based on commit messages and code changes.
 
 ### User Interfaces
 
 * [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
 * [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
-* [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
+* [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories. [WIP](https://github.com/gorillamania/AICodeBot-action)
 * [ ] **Jupyter Notebook Extension**: Provides a Jupyter Notebook extension that can be used to debug code in the notebook.
 * [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
 * [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
 * [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository / Project Management
 
 * [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
-* [ ] **Manage Github Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary, and provide nudges for tasks that need more input.
+* [ ] **Manage GitHub Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary, and provide nudges for tasks that need more input.
 * [ ] **Welcome new contributors**: Automatically welcome new contributors to the project, find out what they're interested in, and suggest issues for them to work on.
 
 ### Fun
 
 * [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
 * [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
 * [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
```

### Comparing `aicodebot-0.8.0/README.md` & `aicodebot-0.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 # AI Code Bot 🤖
 
 ## Your AI-powered coding sidekick
 
-AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
+AICodeBot is a coding assistant designed to make your coding life easier. Think of it as your AI version of a pair programmer. Perform code reviews, create helpful commit messages, debug problems, and help you think through building new features. A team member that accelerates the pace of development and helps you write better code.
 
-We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
+We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/). In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features.
+Status: This project is in its early stages with limited features, but it already improves the software development workflow, and has a healthy roadmap of features (below).
 
-⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent. Much like Tesla's Full Self Driving, you have to keep your hands on the wheel.
+We're using AICodeBot to build AICodeBot, and it's upward spiraling all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
-We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
-
-### What it's not
+### What it's NOT
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
-It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
+⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes AICodeBot does dumb things, which is why it's mostly *reading* and *advising* and not yet *writing*. Much like Tesla's "Full Self Driving", you have to keep your hands on the wheel.
+
+It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that. It's not a no-code platform. Instead, AICodeBot is built to work with existing code bases and the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it today
 
-### AI Sidekick
+### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
  ```bash
  aicodebot sidekick file1.py file2.py
  ```
 
 In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers. For example:
 
 * How can I make this code better?
 * Tell me how to add a new feature to this code.
-* Fix an issue that I'm having when... (describe the issue)
+* Fix an issue that I'm having... (paste the error, stack trace, etc.)
 * Write unit tests for the xyz function.
 
-Please note that this feature is still in its experimental stage. While it can already provide valuable assistance, it's not perfect and we're continuously working on improving it.
+Pro-tip: add your README.md to the list of files to get context-aware answers.
+
+This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingeseting repo specific domain knowledge, writing local files, and more.
 
-### AI-Assisted Git Commit
+### AI-Assisted Git Commit 📝
 
-`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
+`aicodebot commit` improves the git commit process. It will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
 
-### AI-Assisted Code Review
+### AI-Assisted Code Review 👀
 
-`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code and makes us better programmers. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
+`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review.
+It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code and makes us better programmers. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
 
-### AI-Assisted Debugging
+### AI-Assisted Debugging 🐞
 
-`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, command output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
+`aicodebot debug $command` will run the command and capture the log output. It will pass the error message, stack trace, command output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to Stack Overflow in a separate window, allowing you to stay in terminal with all the context.
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg?0.6.2)](https://badge.fury.io/py/aicodebot)
 
 ## Installation and Usage
 
 To install AICodeBot, run:
 
@@ -68,59 +71,60 @@
 
 Commands:
   alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
   commit     Generate a commit message based on your changes.
   debug      Run a command and debug the output.
   fun-fact   Get a fun fact about programming and artificial intelligence.
   review     Do a code review, with [un]staged changes, or a specified...
+  sidekick   EXPERIMENTAL: Coding help from your AI sidekick
   ```
 
 ### Open AI key setup
 
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
 #### Which Language Model? GPT-3.5 vs GPT-4
 
 When using AICodeBot, you have the option to use either GPT-3.5 or GPT-4. While GPT-4 can often provide more accurate and detailed responses, GPT-3.5 is faster and might be sufficient for simpler tasks. We highly recommend GPT-4.
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
 Note: We'll be adding more options for AI models in the future, including those that can be run locally, such as [GPT4all](https://gpt4all.io/) and HuggingFace's [Transformers](https://huggingface.co/transformers/).
 
-## Roadmap of Upcoming Features
+## Roadmap of Upcoming Features ️
 
 ### Code Workflow Improvements
 
 * [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
 * [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
 * [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
 * [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
 * [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 * [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
 * [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
 * [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
-* [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
+* [X] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
 * [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
 * [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
 * [ ] **Automatically Generate ChangeLogs and Release Notes**: Generates release notes and changelogs based on commit messages and code changes.
 
 ### User Interfaces
 
 * [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
 * [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
-* [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
+* [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories. [WIP](https://github.com/gorillamania/AICodeBot-action)
 * [ ] **Jupyter Notebook Extension**: Provides a Jupyter Notebook extension that can be used to debug code in the notebook.
 * [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
 * [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
 * [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository / Project Management
 
 * [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
-* [ ] **Manage Github Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary, and provide nudges for tasks that need more input.
+* [ ] **Manage GitHub Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary, and provide nudges for tasks that need more input.
 * [ ] **Welcome new contributors**: Automatically welcome new contributors to the project, find out what they're interested in, and suggest issues for them to work on.
 
 ### Fun
 
 * [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
 * [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
 * [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
```

### Comparing `aicodebot-0.8.0/aicodebot/agents.py` & `aicodebot-0.8.1/aicodebot/agents.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.0/aicodebot/cli.py` & `aicodebot-0.8.1/aicodebot/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from aicodebot import version as aicodebot_version
-from aicodebot.helpers import exec_and_get_output, get_token_length, git_diff_context
-from aicodebot.prompts import generate_files_context, generate_sidekick_prompt
+from aicodebot.helpers import exec_and_get_output, get_llm_model, get_token_length, git_diff_context, logger
+from aicodebot.prompts import generate_files_context, get_prompt
 from dotenv import load_dotenv
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
 from langchain.memory import ConversationTokenBufferMemory
-from langchain.prompts import load_prompt
 from openai.api_resources import engine
 from pathlib import Path
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.style import Style
 import click, datetime, openai, os, random, subprocess, sys, tempfile, webbrowser
@@ -25,14 +24,15 @@
 # ----------------------- Setup for rich console output ---------------------- #
 
 console = Console()
 bot_style = Style(color="#30D5C8")
 error_style = Style(color="#FF0000")
 warning_style = Style(color="#FFA500")
 
+
 # -------------------------- Top level command group ------------------------- #
 
 
 @click.group()
 @click.version_option(aicodebot_version, "--version", "-V")
 @click.help_option("--help", "-h")
 def cli():
@@ -46,29 +46,31 @@
 # Commands are defined as functions with the @click decorator.
 # The function name is the command name, and the docstring is the help text.
 # Keep the commands in alphabetical order.
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
-def alignment(verbose):
+@click.option("-t", "--response-token-size", type=int, default=350)
+def alignment(response_token_size, verbose):
     """Get a message about Heart-Centered AI Alignment ❤ + 🤖."""
     setup_environment()
 
     # Load the prompt
-    prompt = load_prompt(Path(__file__).parent / "prompts" / "alignment.yaml")
+    prompt = get_prompt("alignment")
+    logger.trace(f"Prompt: {prompt}")
 
     # Set up the language model
     model = get_llm_model(get_token_length(prompt.template))
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=CREATIVE_TEMPERATURE,
-            max_tokens=DEFAULT_MAX_TOKENS,
+            max_tokens=response_token_size,
             verbose=verbose,
             streaming=True,
             callbacks=[RichLiveCallbackHandler(live)],
         )
 
         # Set up the chain
         chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
@@ -90,20 +92,22 @@
         console.print("Running pre-commit checks...")
         result = subprocess.run(["pre-commit", "run", "--all-files"])
         if result.returncode != 0:
             console.print("🛑 Pre-commit checks failed. Please fix the issues and try again.")
             return
 
     # Load the prompt
-    prompt = load_prompt(Path(__file__).parent / "prompts" / "commit_message.yaml")
+    prompt = get_prompt("commit")
+    logger.trace(f"Prompt: {prompt}")
 
     # Get the changes from git
     staged_files = exec_and_get_output(["git", "diff", "--name-only", "--cached"])
     if not staged_files:
         # If no files are staged, Assume they want to commit all changed files
+        logger.info("No files staged, assuming we want to commit all changed files, running git add -A")
         exec_and_get_output(["git", "add", "-A"])
         # Get the list of files to be committed
         files = exec_and_get_output(["git", "diff", "--name-only", "--cached"])
     else:
         # The list of files to be committed is the same as the list of staged files
         files = staged_files
 
@@ -112,16 +116,18 @@
     if not diff_context:
         console.print("No changes to commit. 🤷")
         sys.exit(0)
 
     # Check the size of the diff context and adjust accordingly
     request_token_size = get_token_length(diff_context) + get_token_length(prompt.template)
     model = get_llm_model(request_token_size)
-    if verbose:
-        console.print(f"Diff context token size: {request_token_size}, using model: {model}")
+    if model is None:
+        raise click.ClickException(
+            f"The diff is too large to generate a commit message ({request_token_size} tokens). 😢"
+        )
 
     # Set up the language model
     llm = ChatOpenAI(model=model, temperature=PRECISE_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
@@ -171,18 +177,22 @@
 
     # If the command failed, send its output to ChatGPT for analysis
     error_output = process.stderr
 
     console.print(f"The command exited with status {process.returncode}.")
 
     # Load the prompt
-    prompt = load_prompt(Path(__file__).parent / "prompts" / "debug.yaml")
+    prompt = get_prompt("debug")
+    logger.trace(f"Prompt: {prompt}")
 
     # Set up the language model
-    model = get_llm_model(get_token_length(error_output) + get_token_length(prompt.template))
+    request_token_size = get_token_length(error_output) + get_token_length(prompt.template)
+    model = get_llm_model(request_token_size)
+    if model is None:
+        raise click.ClickException(f"The output is too large to debug ({request_token_size} tokens). 😢")
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=PRECISE_TEMPERATURE,
             max_tokens=DEFAULT_MAX_TOKENS,
             verbose=verbose,
@@ -200,15 +210,16 @@
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 def fun_fact(verbose):
     """Get a fun fact about programming and artificial intelligence."""
     setup_environment()
 
     # Load the prompt
-    prompt = load_prompt(Path(__file__).parent / "prompts" / "fun_fact.yaml")
+    prompt = get_prompt("fun_fact")
+    logger.trace(f"Prompt: {prompt}")
 
     # Set up the language model
     model = get_llm_model(get_token_length(prompt.template))
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
@@ -235,22 +246,23 @@
 
     diff_context = git_diff_context(commit)
     if not diff_context:
         console.print("No changes detected for review. 🤷")
         sys.exit(0)
 
     # Load the prompt
-    prompt = load_prompt(Path(__file__).parent / "prompts" / "review.yaml")
+    prompt = get_prompt("review")
+    logger.trace(f"Prompt: {prompt}")
 
     # Check the size of the diff context and adjust accordingly
     response_token_size = DEFAULT_MAX_TOKENS
     request_token_size = get_token_length(diff_context) + get_token_length(prompt.template)
     model = get_llm_model(request_token_size)
-    if verbose:
-        console.print(f"Diff context token size: {request_token_size}, using model: {model}")
+    if model is None:
+        raise click.ClickException(f"The diff is too large to review ({request_token_size} tokens). 😢")
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=PRECISE_TEMPERATURE,
             max_tokens=response_token_size,
             verbose=verbose,
@@ -282,46 +294,56 @@
     # Soon, we could add vector embeddings of:
     # imported code / modules / libraries
     # Style guides/reference code
     # git history
     context = generate_files_context(files)
 
     # Generate the prompt and set up the model
-    prompt = generate_sidekick_prompt(request, files)
-    model = get_llm_model(get_token_length(prompt.template) + get_token_length(context))
-    if verbose:
-        console.print(f"Context token size: {get_token_length(context)}, using model: {model}")
+    prompt = get_prompt("sidekick")
+    request_token_size = get_token_length(prompt.template) + get_token_length(context)
+    model = get_llm_model(request_token_size)
+    if model is None:
+        raise click.ClickException(
+            f"The file context you supplied is too large ({request_token_size} tokens). 😢 Try again with less files."
+        )
 
     llm = ChatOpenAI(
         model=model,
         temperature=PRECISE_TEMPERATURE,
         max_tokens=DEFAULT_MAX_TOKENS * 2,
         verbose=verbose,
         streaming=True,
     )
 
+    # Open the temporary file in the user's editor
+    editor = Path(os.getenv("EDITOR", "/usr/bin/vim")).name
+
     # Set up the chain
     memory = ConversationTokenBufferMemory(
         memory_key="chat_history", input_key="task", llm=llm, max_token_limit=DEFAULT_MAX_TOKENS
     )
     chain = LLMChain(llm=llm, prompt=prompt, memory=memory, verbose=verbose)
 
     while True:  # continuous loop for multiple questions
         if request:
             human_input = request
             request = None  # clear the command line request once we've handled it
         else:
             human_input = click.prompt(
-                "Enter a question OR (q) quit, OR (e) edit for entering a question in your editor\n>>>",
+                f"Enter a question OR (q) quit, OR (e) to edit using {editor}\n>>>",
                 prompt_suffix="",
             )
-            if human_input.lower() == "q":
-                break
-            elif human_input.lower() == "e":
-                human_input = click.edit()
+            if len(human_input) == 1:
+                if human_input.lower() == "q":
+                    break
+                elif human_input.lower() == "e":
+                    human_input = click.edit()
+            elif human_input.lower()[-2:] == r"\e":
+                # If the text ends with \e then we want to edit it
+                human_input = click.edit(human_input[:-2])
 
         with Live(Markdown(""), auto_refresh=True) as live:
             callback = RichLiveCallbackHandler(live)
             callback.buffer = []
             llm.callbacks = [callback]
             chain.run({"task": human_input, "context": context})
 
@@ -333,14 +355,15 @@
 
 def setup_environment():
     # Load environment variables from the config file
     config_file = Path(Path.home() / ".aicodebot")
     load_dotenv(config_file)
 
     if os.getenv("OPENAI_API_KEY"):
+        logger.debug("OPENAI_API_KEY environment variable is set")
         openai.api_key = os.getenv("OPENAI_API_KEY")
         return True
 
     openai_api_key_url = "https://platform.openai.com/account/api-keys"
 
     console.print(
         "[bold red]The OPENAI_API_KEY environment variable is not set.[/bold red]\n"
@@ -355,14 +378,15 @@
         api_key = click.prompt("Please enter your OpenAI API key")
 
         # Validate the API key and check if it supports GPT-4
         openai.api_key = api_key
         try:
             click.echo("Validating the API key, and checking if GPT-4 is supported...")
             engines = engine.Engine.list()
+            logger.trace(f"Engines: {engines}")
             gpt_4_supported = "true" if "gpt-4" in [engine.id for engine in engines.data] else "false"
             if gpt_4_supported == "true":
                 click.echo("✅ The API key is valid and supports GPT-4.")
             else:
                 click.echo("✅ The API key is valid, but does not support GPT-4. GPT-3.5 will be used instead.")
         except Exception as e:
             raise click.ClickException(f"Failed to validate the API key: {str(e)}") from e
@@ -385,45 +409,14 @@
         sys.exit(0)
 
     raise click.ClickException(
         "🛑 Please set an API key in the OPENAI_API_KEY environment variable or in a .aicodebot file."
     )
 
 
-def get_llm_model(token_size=0):
-    # https://platform.openai.com/docs/models/gpt-3-5
-    # We want to use GPT-4, if it is available for this OPENAI_API_KEY, otherwise GPT-3.5
-    # We also want to use the largest model that supports the token size we need
-    model_options = {
-        "gpt-4": 8192,
-        "gpt-4-32k": 32768,
-        "gpt-3.5-turbo": 4096,
-        "gpt-3.5-turbo-16k": 16384,
-    }
-    gpt_4_supported = os.getenv("GPT_4_SUPPORTED") == "true"
-
-    # For some unknown reason, tiktoken often underestimates the token size by ~10%, so let's buffer
-    token_size = int(token_size * 1.1)
-
-    if gpt_4_supported:
-        if token_size <= model_options["gpt-4"]:
-            return "gpt-4"
-        elif token_size <= model_options["gpt-4-32k"]:
-            return "gpt-4-32k"
-        else:
-            raise click.ClickException("🛑 The context is too large to for the Model. 😞")
-    else:
-        if token_size <= model_options["gpt-3.5-turbo"]:  # noqa: PLR5501
-            return "gpt-3.5-turbo"
-        elif token_size <= model_options["gpt-3.5-turbo-16k"]:
-            return "gpt-3.5-turbo-16k"
-        else:
-            raise click.ClickException("🛑 The context is too large to for the Model. 😞")
-
-
 class RichLiveCallbackHandler(BaseCallbackHandler):
     buffer = []
 
     def __init__(self, live):
         self.live = live
 
     def on_llm_new_token(self, token, **kwargs):
```

### Comparing `aicodebot-0.8.0/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.8.1/aicodebot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.8.0
+Version: 0.8.1
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -15,60 +15,63 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AI Code Bot 🤖
 
 ## Your AI-powered coding sidekick
 
-AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
+AICodeBot is a coding assistant designed to make your coding life easier. Think of it as your AI version of a pair programmer. Perform code reviews, create helpful commit messages, debug problems, and help you think through building new features. A team member that accelerates the pace of development and helps you write better code.
 
-We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
+We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/). In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features.
+Status: This project is in its early stages with limited features, but it already improves the software development workflow, and has a healthy roadmap of features (below).
 
-⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent. Much like Tesla's Full Self Driving, you have to keep your hands on the wheel.
+We're using AICodeBot to build AICodeBot, and it's upward spiraling all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
-We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
-
-### What it's not
+### What it's NOT
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
-It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
+⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes AICodeBot does dumb things, which is why it's mostly *reading* and *advising* and not yet *writing*. Much like Tesla's "Full Self Driving", you have to keep your hands on the wheel.
+
+It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that. It's not a no-code platform. Instead, AICodeBot is built to work with existing code bases and the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it today
 
-### AI Sidekick
+### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
  ```bash
  aicodebot sidekick file1.py file2.py
  ```
 
 In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers. For example:
 
 * How can I make this code better?
 * Tell me how to add a new feature to this code.
-* Fix an issue that I'm having when... (describe the issue)
+* Fix an issue that I'm having... (paste the error, stack trace, etc.)
 * Write unit tests for the xyz function.
 
-Please note that this feature is still in its experimental stage. While it can already provide valuable assistance, it's not perfect and we're continuously working on improving it.
+Pro-tip: add your README.md to the list of files to get context-aware answers.
+
+This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingeseting repo specific domain knowledge, writing local files, and more.
 
-### AI-Assisted Git Commit
+### AI-Assisted Git Commit 📝
 
-`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
+`aicodebot commit` improves the git commit process. It will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
 
-### AI-Assisted Code Review
+### AI-Assisted Code Review 👀
 
-`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code and makes us better programmers. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
+`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review.
+It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code and makes us better programmers. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
 
-### AI-Assisted Debugging
+### AI-Assisted Debugging 🐞
 
-`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, command output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
+`aicodebot debug $command` will run the command and capture the log output. It will pass the error message, stack trace, command output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to Stack Overflow in a separate window, allowing you to stay in terminal with all the context.
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg?0.6.2)](https://badge.fury.io/py/aicodebot)
 
 ## Installation and Usage
 
 To install AICodeBot, run:
 
@@ -85,59 +88,60 @@
 
 Commands:
   alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
   commit     Generate a commit message based on your changes.
   debug      Run a command and debug the output.
   fun-fact   Get a fun fact about programming and artificial intelligence.
   review     Do a code review, with [un]staged changes, or a specified...
+  sidekick   EXPERIMENTAL: Coding help from your AI sidekick
   ```
 
 ### Open AI key setup
 
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
 #### Which Language Model? GPT-3.5 vs GPT-4
 
 When using AICodeBot, you have the option to use either GPT-3.5 or GPT-4. While GPT-4 can often provide more accurate and detailed responses, GPT-3.5 is faster and might be sufficient for simpler tasks. We highly recommend GPT-4.
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
 Note: We'll be adding more options for AI models in the future, including those that can be run locally, such as [GPT4all](https://gpt4all.io/) and HuggingFace's [Transformers](https://huggingface.co/transformers/).
 
-## Roadmap of Upcoming Features
+## Roadmap of Upcoming Features ️
 
 ### Code Workflow Improvements
 
 * [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
 * [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
 * [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
 * [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
 * [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 * [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
 * [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
 * [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
-* [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
+* [X] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
 * [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
 * [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
 * [ ] **Automatically Generate ChangeLogs and Release Notes**: Generates release notes and changelogs based on commit messages and code changes.
 
 ### User Interfaces
 
 * [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
 * [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
-* [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
+* [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories. [WIP](https://github.com/gorillamania/AICodeBot-action)
 * [ ] **Jupyter Notebook Extension**: Provides a Jupyter Notebook extension that can be used to debug code in the notebook.
 * [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
 * [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
 * [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository / Project Management
 
 * [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
-* [ ] **Manage Github Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary, and provide nudges for tasks that need more input.
+* [ ] **Manage GitHub Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary, and provide nudges for tasks that need more input.
 * [ ] **Welcome new contributors**: Automatically welcome new contributors to the project, find out what they're interested in, and suggest issues for them to work on.
 
 ### Fun
 
 * [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
 * [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
 * [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
```

### Comparing `aicodebot-0.8.0/pyproject.toml` & `aicodebot-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.0/setup.py` & `aicodebot-0.8.1/setup.py`

 * *Files identical despite different names*

