# Comparing `tmp/botcity-framework-core-1.1.1.tar.gz` & `tmp/botcity-framework-core-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/botcity-framework-core-python/botcity-framework-core-python/dist/.tmp-eiumycgb/botcity-framework-core-1.1.1.t", last modified: Tue May  9 21:27:55 2023, max compression
+gzip compressed data, was "/home/runner/work/botcity-framework-core-python/botcity-framework-core-python/dist/.tmp-d8_m854x/botcity-framework-core-1.1.2.t", last modified: Thu Jul  6 18:53:32 2023, max compression
```

## Comparing `botcity-framework-core-1.1.1.tar` & `botcity-framework-core-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/core/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/core/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/core/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/application/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/application/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    54451 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/cv2find.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/os_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity/core/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity/core/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/application/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/application/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54605 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/cv2find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/os_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/botcity/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity_framework_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity_framework_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity_framework_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity_framework_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity_framework_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/botcity_framework_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-06 18:53:32.000000 botcity-framework-core-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-07-06 18:53:20.000000 botcity-framework-core-1.1.2/versioneer.py
```

### Comparing `botcity-framework-core-1.1.1/LICENSE` & `botcity-framework-core-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.1/PKG-INFO` & `botcity-framework-core-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: botcity-framework-core
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://www.github.com/botcity-dev/botcity-framework-core-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <h1 align="center">BotCity Framework Core - Python</h1>
 
   <p align="center">
-    <strong>« Explore Framework <a href="https://botcity-dev.github.io/botcity-framework-core-python/">docs</a> »</strong>
+    <strong>« Explore Framework <a href="https://documentation.botcity.dev/frameworks/desktop/">docs</a> »</strong>
   </p>
 </p>
 
 <br>
 
 ## Summary  <!-- omit in toc -->
 
@@ -29,16 +29,15 @@
 - [💬 Forum](#-forum)
 - [🌎 BotCity Automation Platform](#-botcity-automation-platform)
   - [1️⃣  All in One Platform](#1️⃣--all-in-one-platform)
   - [2️⃣  Deploy with a Single Line](#2️⃣--deploy-with-a-single-line)
   - [3️⃣  Manage your Task Queue](#3️⃣--manage-your-task-queue)
   - [4️⃣  Manage your Runtime Environments](#4️⃣--manage-your-runtime-environments)
   - [5️⃣  Create Alerts and Reports from the Automation Execution](#5️⃣--create-alerts-and-reports-from-the-automation-execution)
-  - [6️⃣  Create Google Data Studio Dashboards](#6️⃣--create-google-data-studio-dashboards)
-  - [7️⃣  Create your Community Account](#7️⃣--create-your-community-account)
+  - [6️⃣  Create your Community Account](#6️⃣--create-your-community-account)
 - [🤝 Contributing to BotCity Framework](#-contributing-to-botcity-framework)
 - [⛑ Support](#-support)
   - [🐛 Bug reports and 💎 Feature requests](#-bug-reports-and--feature-requests)
   - [📢 Contact us](#-contact-us)
 - [💡 Related Projects](#-related-projects)
 
 
@@ -48,15 +47,15 @@
 
 Operate any UI interface independent of the technology or platform (desktop, web, terminal).
 
 ## 🐍 Generate Python Code while Interacting with your UI
 
 Use our Development Tool alongside your favorite IDE to select UI components and generate python code.
 
-[![BotCity Studio](https://botcity.dev/github/readme/studio/studio.gif)](https://botcity.atlassian.net/l/c/eBJ6bLLV)
+[![BotCity Studio](https://botcity.dev/github/readme/studio/studio.gif)](https://documentation.botcity.dev/studio/)
 
 [SIGN UP](https://developers.botcity.dev/signup) and download our tools.
 
 
 ## 🚀 Getting Started
 
 ### 📦 Prerequisites
@@ -70,69 +69,68 @@
 
 ```bash
 pip install botcity-framework-core
 ```
 
 ### ⭐ Developing Your First Automation
 
-[![First Automation](https://botcity.dev/github/readme/python-core/firstbot.png)](https://botcity-dev.github.io/botcity-framework-core-python/intro/)
+[![First Automation](https://botcity.dev/github/readme/python-core/firstbot.png)](https://documentation.botcity.dev/tutorials/python-automations/desktop/)
 
 ## 📚 Documentation
 
-Documentation is available at https://botcity-dev.github.io/botcity-framework-core-python.
+Documentation is available at https://documentation.botcity.dev/frameworks/desktop/.
 
 ## 💻 Developers Portal
 
-[![Developers Portal](https://botcity.dev/github/readme/portal.png)](https://documentation.botcity.dev)
+[![Developers Portal](https://botcity.dev/github/readme/portal.png?)](https://documentation.botcity.dev)
 
 ## 💬 Forum
 
 [![Forum](https://botcity.dev/github/readme/forum.png)](https://community.botcity.dev/)
 
 ## 🌎 BotCity Automation Platform
 BotCity is a platform to develop, deploy, manage and maintain automations. Automations can be developed in Python or Java using open-source libraries that are market standard.
 
 ### 1️⃣  All in One Platform
 Develop, deploy, manage and scale your Automation Ops using All in One platform that provides task queue, runtime environment management, reports, alerts, logs and much more.
 
-[![BotCity Maestro](https://botcity.dev/github/readme/maestro/maestro.png)](https://botcity.atlassian.net/l/c/WWGswYRX)
+[![BotCity Maestro](https://botcity.dev/github/readme/maestro/maestro.png?)](https://documentation.botcity.dev/maestro/)
 
 ### 2️⃣  Deploy with a Single Line
 
 Use BotCity command-line interface (CLI) to deploy your bot into a runtime environment with a single line:
 
-[![BotCity CLI](https://botcity.dev/github/readme/cli/botcli.gif)](https://botcity.atlassian.net/l/c/hJHE1ZFv)
+[![BotCity CLI](https://botcity.dev/github/readme/cli/botcli.gif)](https://documentation.botcity.dev/cli/)
 
 ### 3️⃣  Manage your Task Queue
 
-[![BotCity Maestro Task Queue](https://botcity.dev/github/readme/maestro/tasks.png)](https://botcity.atlassian.net/l/c/gR3AAd2a)
+[![BotCity Maestro Task Queue](https://botcity.dev/github/readme/maestro/tasks.png?)](https://documentation.botcity.dev/maestro/features/task-queue/)
 
 ### 4️⃣  Manage your Runtime Environments
 
-[![BotCity Maestro Machines](https://botcity.dev/github/readme/maestro/machines.png)](https://botcity.atlassian.net/l/c/uDB087nK)
+[![BotCity Maestro Machines](https://botcity.dev/github/readme/maestro/machines.png?)](https://documentation.botcity.dev/maestro/features/runners/)
 
 ### 5️⃣  Create Alerts and Reports from the Automation Execution
 
-[![BotCity Maestro Alerts](https://botcity.dev/github/readme/maestro/alerts.png)](https://botcity.atlassian.net/l/c/McH09qYw)
+#### Alerts
+[![BotCity Maestro Alerts](https://botcity.dev/github/readme/maestro/alerts.png?)](https://documentation.botcity.dev/maestro/features/alerts/)
 
-### 6️⃣  Create Google Data Studio Dashboards
+#### Execution Logs
+[![BotCity Maestro Alerts](https://botcity.dev/github/readme/maestro/logs.png?)](https://documentation.botcity.dev/maestro/features/logs/)
 
-[![BotCity Maestro Dashboards](https://botcity.dev/github/readme/maestro/dashboard.png)](https://botcity.atlassian.net/l/c/Z1uMY1vX)
-
-### 7️⃣  Create your Community Account
+### 6️⃣  Create your Community Account
 
 We have a community account for hobbyists and students. Just signup and start automating.
 
-[![Sign Up](https://botcity.dev/github/readme/signup.png)](https://developers.botcity.dev/signup)
-
+[![Sign Up](https://botcity.dev/github/readme/signup.png?)](https://developers.botcity.dev/signup)
 
 ## 🤝 Contributing to BotCity Framework
 
 - [Guidelines](https://github.com/botcity-dev/botcity-framework-core-python/blob/main/.github/CONTRIBUTING.md)
-- [Documentation](https://botcity-dev.github.io/botcity-framework-core-python/)
+- [Documentation](https://documentation.botcity.dev/frameworks/desktop/)
 
 ## ⛑ Support
 
 ### 🐛 Bug reports and 💎 Feature requests
 
 If you spot a problem, please let us know by following the template in
 here: [Report a bug](https://github.com/botcity-dev/botcity-framework-core-python/issues/new?template=bug-report.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botcity-framework-core Version: 1.1.1 Home-page:
+Metadata-Version: 2.1 Name: botcity-framework-core Version: 1.1.2 Home-page:
 https://www.github.com/botcity-dev/botcity-framework-core-python Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
                  ****** BotCity Framework Core - Python ******
                          Â« Explore Framework docs Â»
 
 ## Summary  - [ð¤ Computer-vision based UI Automation](#-computer-vision-
 based-ui-automation) - [ð Generate Python Code while Interacting with your
@@ -13,72 +13,72 @@
 [ð» Developers Portal](#-developers-portal) - [ð¬ Forum](#-forum) - [ð
 BotCity Automation Platform](#-botcity-automation-platform) - [1ï¸â£ All in
 One Platform](#1ï¸â£--all-in-one-platform) - [2ï¸â£ Deploy with a Single
 Line](#2ï¸â£--deploy-with-a-single-line) - [3ï¸â£ Manage your Task Queue]
 (#3ï¸â£--manage-your-task-queue) - [4ï¸â£ Manage your Runtime Environments]
 (#4ï¸â£--manage-your-runtime-environments) - [5ï¸â£ Create Alerts and
 Reports from the Automation Execution](#5ï¸â£--create-alerts-and-reports-
-from-the-automation-execution) - [6ï¸â£ Create Google Data Studio Dashboards]
-(#6ï¸â£--create-google-data-studio-dashboards) - [7ï¸â£ Create your
-Community Account](#7ï¸â£--create-your-community-account) - [ð¤
-Contributing to BotCity Framework](#-contributing-to-botcity-framework) - [â
-Support](#-support) - [ð Bug reports and ð Feature requests](#-bug-
-reports-and--feature-requests) - [ð¢ Contact us](#-contact-us) - [ð¡
-Related Projects](#-related-projects) ## ð¤ Computer-vision based UI
-Automation Recognize and interact with UI elements using state-of-art computer
-vision module. Operate any UI interface independent of the technology or
-platform (desktop, web, terminal). ## ð Generate Python Code while
-Interacting with your UI Use our Development Tool alongside your favorite IDE
-to select UI components and generate python code. [![BotCity Studio](https://
-botcity.dev/github/readme/studio/studio.gif)](https://botcity.atlassian.net/l/
-c/eBJ6bLLV) [SIGN UP](https://developers.botcity.dev/signup) and download our
-tools. ## ð Getting Started ### ð¦ Prerequisites * Python 3.7+ * python3-
-tk **(Linux Only)** * scrot **(Linux Only)** * xsel **(Linux Only)** * xclip **
-(Linux Only)** ### ð« Installing ```bash pip install botcity-framework-core
-``` ### â­ Developing Your First Automation [![First Automation](https://
-botcity.dev/github/readme/python-core/firstbot.png)](https://botcity-
-dev.github.io/botcity-framework-core-python/intro/) ## ð Documentation
-Documentation is available at https://botcity-dev.github.io/botcity-framework-
-core-python. ## ð» Developers Portal [![Developers Portal](https://
-botcity.dev/github/readme/portal.png)](https://documentation.botcity.dev) ##
-ð¬ Forum [![Forum](https://botcity.dev/github/readme/forum.png)](https://
-community.botcity.dev/) ## ð BotCity Automation Platform BotCity is a
-platform to develop, deploy, manage and maintain automations. Automations can
-be developed in Python or Java using open-source libraries that are market
-standard. ### 1ï¸â£ All in One Platform Develop, deploy, manage and scale
-your Automation Ops using All in One platform that provides task queue, runtime
-environment management, reports, alerts, logs and much more. [![BotCity
-Maestro](https://botcity.dev/github/readme/maestro/maestro.png)](https://
-botcity.atlassian.net/l/c/WWGswYRX) ### 2ï¸â£ Deploy with a Single Line Use
-BotCity command-line interface (CLI) to deploy your bot into a runtime
-environment with a single line: [![BotCity CLI](https://botcity.dev/github/
-readme/cli/botcli.gif)](https://botcity.atlassian.net/l/c/hJHE1ZFv) ### 3ï¸â£
-Manage your Task Queue [![BotCity Maestro Task Queue](https://botcity.dev/
-github/readme/maestro/tasks.png)](https://botcity.atlassian.net/l/c/gR3AAd2a)
-### 4ï¸â£ Manage your Runtime Environments [![BotCity Maestro Machines]
-(https://botcity.dev/github/readme/maestro/machines.png)](https://
-botcity.atlassian.net/l/c/uDB087nK) ### 5ï¸â£ Create Alerts and Reports from
-the Automation Execution [![BotCity Maestro Alerts](https://botcity.dev/github/
-readme/maestro/alerts.png)](https://botcity.atlassian.net/l/c/McH09qYw) ###
-6ï¸â£ Create Google Data Studio Dashboards [![BotCity Maestro Dashboards]
-(https://botcity.dev/github/readme/maestro/dashboard.png)](https://
-botcity.atlassian.net/l/c/Z1uMY1vX) ### 7ï¸â£ Create your Community Account
-We have a community account for hobbyists and students. Just signup and start
-automating. [![Sign Up](https://botcity.dev/github/readme/signup.png)](https://
-developers.botcity.dev/signup) ## ð¤ Contributing to BotCity Framework -
-[Guidelines](https://github.com/botcity-dev/botcity-framework-core-python/blob/
-main/.github/CONTRIBUTING.md) - [Documentation](https://botcity-dev.github.io/
-botcity-framework-core-python/) ## â Support ### ð Bug reports and ð
-Feature requests If you spot a problem, please let us know by following the
-template in here: [Report a bug](https://github.com/botcity-dev/botcity-
-framework-core-python/issues/new?template=bug-report.md). Ideas or suggestions
-for enhancements are more than welcome. Please use the following template in
-here: [Request feature](https://github.com/botcity-dev/botcity-framework-core-
-python/issues/new?template=feature-request.md). ### ð¢ Contact us If you have
-questions or comments in general about the framework, we want to know. You can
-choose between the channels the one that best fit you: - [BotCity Community](
+from-the-automation-execution) - [6ï¸â£ Create your Community Account]
+(#6ï¸â£--create-your-community-account) - [ð¤ Contributing to BotCity
+Framework](#-contributing-to-botcity-framework) - [â Support](#-support) -
+[ð Bug reports and ð Feature requests](#-bug-reports-and--feature-
+requests) - [ð¢ Contact us](#-contact-us) - [ð¡ Related Projects](#-
+related-projects) ## ð¤ Computer-vision based UI Automation Recognize and
+interact with UI elements using state-of-art computer vision module. Operate
+any UI interface independent of the technology or platform (desktop, web,
+terminal). ## ð Generate Python Code while Interacting with your UI Use our
+Development Tool alongside your favorite IDE to select UI components and
+generate python code. [![BotCity Studio](https://botcity.dev/github/readme/
+studio/studio.gif)](https://documentation.botcity.dev/studio/) [SIGN UP](https:
+//developers.botcity.dev/signup) and download our tools. ## ð Getting
+Started ### ð¦ Prerequisites * Python 3.7+ * python3-tk **(Linux Only)** *
+scrot **(Linux Only)** * xsel **(Linux Only)** * xclip **(Linux Only)** ###
+ð« Installing ```bash pip install botcity-framework-core ``` ### â­
+Developing Your First Automation [![First Automation](https://botcity.dev/
+github/readme/python-core/firstbot.png)](https://documentation.botcity.dev/
+tutorials/python-automations/desktop/) ## ð Documentation Documentation is
+available at https://documentation.botcity.dev/frameworks/desktop/. ## ð»
+Developers Portal [![Developers Portal](https://botcity.dev/github/readme/
+portal.png?)](https://documentation.botcity.dev) ## ð¬ Forum [![Forum](https:
+//botcity.dev/github/readme/forum.png)](https://community.botcity.dev/) ## ð
+BotCity Automation Platform BotCity is a platform to develop, deploy, manage
+and maintain automations. Automations can be developed in Python or Java using
+open-source libraries that are market standard. ### 1ï¸â£ All in One Platform
+Develop, deploy, manage and scale your Automation Ops using All in One platform
+that provides task queue, runtime environment management, reports, alerts, logs
+and much more. [![BotCity Maestro](https://botcity.dev/github/readme/maestro/
+maestro.png?)](https://documentation.botcity.dev/maestro/) ### 2ï¸â£ Deploy
+with a Single Line Use BotCity command-line interface (CLI) to deploy your bot
+into a runtime environment with a single line: [![BotCity CLI](https://
+botcity.dev/github/readme/cli/botcli.gif)](https://documentation.botcity.dev/
+cli/) ### 3ï¸â£ Manage your Task Queue [![BotCity Maestro Task Queue](https:/
+/botcity.dev/github/readme/maestro/tasks.png?)](https://
+documentation.botcity.dev/maestro/features/task-queue/) ### 4ï¸â£ Manage your
+Runtime Environments [![BotCity Maestro Machines](https://botcity.dev/github/
+readme/maestro/machines.png?)](https://documentation.botcity.dev/maestro/
+features/runners/) ### 5ï¸â£ Create Alerts and Reports from the Automation
+Execution #### Alerts [![BotCity Maestro Alerts](https://botcity.dev/github/
+readme/maestro/alerts.png?)](https://documentation.botcity.dev/maestro/
+features/alerts/) #### Execution Logs [![BotCity Maestro Alerts](https://
+botcity.dev/github/readme/maestro/logs.png?)](https://
+documentation.botcity.dev/maestro/features/logs/) ### 6ï¸â£ Create your
+Community Account We have a community account for hobbyists and students. Just
+signup and start automating. [![Sign Up](https://botcity.dev/github/readme/
+signup.png?)](https://developers.botcity.dev/signup) ## ð¤ Contributing to
+BotCity Framework - [Guidelines](https://github.com/botcity-dev/botcity-
+framework-core-python/blob/main/.github/CONTRIBUTING.md) - [Documentation]
+(https://documentation.botcity.dev/frameworks/desktop/) ## â Support ### ð
+Bug reports and ð Feature requests If you spot a problem, please let us know
+by following the template in here: [Report a bug](https://github.com/botcity-
+dev/botcity-framework-core-python/issues/new?template=bug-report.md). Ideas or
+suggestions for enhancements are more than welcome. Please use the following
+template in here: [Request feature](https://github.com/botcity-dev/botcity-
+framework-core-python/issues/new?template=feature-request.md). ### ð¢ Contact
+us If you have questions or comments in general about the framework, we want to
+know. You can choose between the channels the one that best fit you: - [BotCity
+Community](
 community.botcity.dev>) (Public) or you can [file a bug](https://github.com/
 botcity-dev/botcity-framework-core-python/issues/new?template=bug-report.md)
 and let us know where our documentation could be improved. ## ð¡ Related
 Projects [https://github-readme-stats.vercel.app/api/pin/?username=botcity-
 dev&repo=botcity-framework-web-python] [https://github-readme-stats.vercel.app/
 api/pin/?username=botcity-dev&repo=botcity-maestro-sdk-python]
```

### Comparing `botcity-framework-core-1.1.1/README.md` & `botcity-framework-core-1.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <p align="center">
   <h1 align="center">BotCity Framework Core - Python</h1>
 
   <p align="center">
-    <strong>« Explore Framework <a href="https://botcity-dev.github.io/botcity-framework-core-python/">docs</a> »</strong>
+    <strong>« Explore Framework <a href="https://documentation.botcity.dev/frameworks/desktop/">docs</a> »</strong>
   </p>
 </p>
 
 <br>
 
 ## Summary  <!-- omit in toc -->
 
@@ -21,16 +21,15 @@
 - [💬 Forum](#-forum)
 - [🌎 BotCity Automation Platform](#-botcity-automation-platform)
   - [1️⃣  All in One Platform](#1️⃣--all-in-one-platform)
   - [2️⃣  Deploy with a Single Line](#2️⃣--deploy-with-a-single-line)
   - [3️⃣  Manage your Task Queue](#3️⃣--manage-your-task-queue)
   - [4️⃣  Manage your Runtime Environments](#4️⃣--manage-your-runtime-environments)
   - [5️⃣  Create Alerts and Reports from the Automation Execution](#5️⃣--create-alerts-and-reports-from-the-automation-execution)
-  - [6️⃣  Create Google Data Studio Dashboards](#6️⃣--create-google-data-studio-dashboards)
-  - [7️⃣  Create your Community Account](#7️⃣--create-your-community-account)
+  - [6️⃣  Create your Community Account](#6️⃣--create-your-community-account)
 - [🤝 Contributing to BotCity Framework](#-contributing-to-botcity-framework)
 - [⛑ Support](#-support)
   - [🐛 Bug reports and 💎 Feature requests](#-bug-reports-and--feature-requests)
   - [📢 Contact us](#-contact-us)
 - [💡 Related Projects](#-related-projects)
 
 
@@ -40,15 +39,15 @@
 
 Operate any UI interface independent of the technology or platform (desktop, web, terminal).
 
 ## 🐍 Generate Python Code while Interacting with your UI
 
 Use our Development Tool alongside your favorite IDE to select UI components and generate python code.
 
-[![BotCity Studio](https://botcity.dev/github/readme/studio/studio.gif)](https://botcity.atlassian.net/l/c/eBJ6bLLV)
+[![BotCity Studio](https://botcity.dev/github/readme/studio/studio.gif)](https://documentation.botcity.dev/studio/)
 
 [SIGN UP](https://developers.botcity.dev/signup) and download our tools.
 
 
 ## 🚀 Getting Started
 
 ### 📦 Prerequisites
@@ -62,69 +61,68 @@
 
 ```bash
 pip install botcity-framework-core
 ```
 
 ### ⭐ Developing Your First Automation
 
-[![First Automation](https://botcity.dev/github/readme/python-core/firstbot.png)](https://botcity-dev.github.io/botcity-framework-core-python/intro/)
+[![First Automation](https://botcity.dev/github/readme/python-core/firstbot.png)](https://documentation.botcity.dev/tutorials/python-automations/desktop/)
 
 ## 📚 Documentation
 
-Documentation is available at https://botcity-dev.github.io/botcity-framework-core-python.
+Documentation is available at https://documentation.botcity.dev/frameworks/desktop/.
 
 ## 💻 Developers Portal
 
-[![Developers Portal](https://botcity.dev/github/readme/portal.png)](https://documentation.botcity.dev)
+[![Developers Portal](https://botcity.dev/github/readme/portal.png?)](https://documentation.botcity.dev)
 
 ## 💬 Forum
 
 [![Forum](https://botcity.dev/github/readme/forum.png)](https://community.botcity.dev/)
 
 ## 🌎 BotCity Automation Platform
 BotCity is a platform to develop, deploy, manage and maintain automations. Automations can be developed in Python or Java using open-source libraries that are market standard.
 
 ### 1️⃣  All in One Platform
 Develop, deploy, manage and scale your Automation Ops using All in One platform that provides task queue, runtime environment management, reports, alerts, logs and much more.
 
-[![BotCity Maestro](https://botcity.dev/github/readme/maestro/maestro.png)](https://botcity.atlassian.net/l/c/WWGswYRX)
+[![BotCity Maestro](https://botcity.dev/github/readme/maestro/maestro.png?)](https://documentation.botcity.dev/maestro/)
 
 ### 2️⃣  Deploy with a Single Line
 
 Use BotCity command-line interface (CLI) to deploy your bot into a runtime environment with a single line:
 
-[![BotCity CLI](https://botcity.dev/github/readme/cli/botcli.gif)](https://botcity.atlassian.net/l/c/hJHE1ZFv)
+[![BotCity CLI](https://botcity.dev/github/readme/cli/botcli.gif)](https://documentation.botcity.dev/cli/)
 
 ### 3️⃣  Manage your Task Queue
 
-[![BotCity Maestro Task Queue](https://botcity.dev/github/readme/maestro/tasks.png)](https://botcity.atlassian.net/l/c/gR3AAd2a)
+[![BotCity Maestro Task Queue](https://botcity.dev/github/readme/maestro/tasks.png?)](https://documentation.botcity.dev/maestro/features/task-queue/)
 
 ### 4️⃣  Manage your Runtime Environments
 
-[![BotCity Maestro Machines](https://botcity.dev/github/readme/maestro/machines.png)](https://botcity.atlassian.net/l/c/uDB087nK)
+[![BotCity Maestro Machines](https://botcity.dev/github/readme/maestro/machines.png?)](https://documentation.botcity.dev/maestro/features/runners/)
 
 ### 5️⃣  Create Alerts and Reports from the Automation Execution
 
-[![BotCity Maestro Alerts](https://botcity.dev/github/readme/maestro/alerts.png)](https://botcity.atlassian.net/l/c/McH09qYw)
+#### Alerts
+[![BotCity Maestro Alerts](https://botcity.dev/github/readme/maestro/alerts.png?)](https://documentation.botcity.dev/maestro/features/alerts/)
 
-### 6️⃣  Create Google Data Studio Dashboards
+#### Execution Logs
+[![BotCity Maestro Alerts](https://botcity.dev/github/readme/maestro/logs.png?)](https://documentation.botcity.dev/maestro/features/logs/)
 
-[![BotCity Maestro Dashboards](https://botcity.dev/github/readme/maestro/dashboard.png)](https://botcity.atlassian.net/l/c/Z1uMY1vX)
-
-### 7️⃣  Create your Community Account
+### 6️⃣  Create your Community Account
 
 We have a community account for hobbyists and students. Just signup and start automating.
 
-[![Sign Up](https://botcity.dev/github/readme/signup.png)](https://developers.botcity.dev/signup)
-
+[![Sign Up](https://botcity.dev/github/readme/signup.png?)](https://developers.botcity.dev/signup)
 
 ## 🤝 Contributing to BotCity Framework
 
 - [Guidelines](https://github.com/botcity-dev/botcity-framework-core-python/blob/main/.github/CONTRIBUTING.md)
-- [Documentation](https://botcity-dev.github.io/botcity-framework-core-python/)
+- [Documentation](https://documentation.botcity.dev/frameworks/desktop/)
 
 ## ⛑ Support
 
 ### 🐛 Bug reports and 💎 Feature requests
 
 If you spot a problem, please let us know by following the template in
 here: [Report a bug](https://github.com/botcity-dev/botcity-framework-core-python/issues/new?template=bug-report.md).
```

#### html2text {}

```diff
@@ -10,72 +10,72 @@
 [ð» Developers Portal](#-developers-portal) - [ð¬ Forum](#-forum) - [ð
 BotCity Automation Platform](#-botcity-automation-platform) - [1ï¸â£ All in
 One Platform](#1ï¸â£--all-in-one-platform) - [2ï¸â£ Deploy with a Single
 Line](#2ï¸â£--deploy-with-a-single-line) - [3ï¸â£ Manage your Task Queue]
 (#3ï¸â£--manage-your-task-queue) - [4ï¸â£ Manage your Runtime Environments]
 (#4ï¸â£--manage-your-runtime-environments) - [5ï¸â£ Create Alerts and
 Reports from the Automation Execution](#5ï¸â£--create-alerts-and-reports-
-from-the-automation-execution) - [6ï¸â£ Create Google Data Studio Dashboards]
-(#6ï¸â£--create-google-data-studio-dashboards) - [7ï¸â£ Create your
-Community Account](#7ï¸â£--create-your-community-account) - [ð¤
-Contributing to BotCity Framework](#-contributing-to-botcity-framework) - [â
-Support](#-support) - [ð Bug reports and ð Feature requests](#-bug-
-reports-and--feature-requests) - [ð¢ Contact us](#-contact-us) - [ð¡
-Related Projects](#-related-projects) ## ð¤ Computer-vision based UI
-Automation Recognize and interact with UI elements using state-of-art computer
-vision module. Operate any UI interface independent of the technology or
-platform (desktop, web, terminal). ## ð Generate Python Code while
-Interacting with your UI Use our Development Tool alongside your favorite IDE
-to select UI components and generate python code. [![BotCity Studio](https://
-botcity.dev/github/readme/studio/studio.gif)](https://botcity.atlassian.net/l/
-c/eBJ6bLLV) [SIGN UP](https://developers.botcity.dev/signup) and download our
-tools. ## ð Getting Started ### ð¦ Prerequisites * Python 3.7+ * python3-
-tk **(Linux Only)** * scrot **(Linux Only)** * xsel **(Linux Only)** * xclip **
-(Linux Only)** ### ð« Installing ```bash pip install botcity-framework-core
-``` ### â­ Developing Your First Automation [![First Automation](https://
-botcity.dev/github/readme/python-core/firstbot.png)](https://botcity-
-dev.github.io/botcity-framework-core-python/intro/) ## ð Documentation
-Documentation is available at https://botcity-dev.github.io/botcity-framework-
-core-python. ## ð» Developers Portal [![Developers Portal](https://
-botcity.dev/github/readme/portal.png)](https://documentation.botcity.dev) ##
-ð¬ Forum [![Forum](https://botcity.dev/github/readme/forum.png)](https://
-community.botcity.dev/) ## ð BotCity Automation Platform BotCity is a
-platform to develop, deploy, manage and maintain automations. Automations can
-be developed in Python or Java using open-source libraries that are market
-standard. ### 1ï¸â£ All in One Platform Develop, deploy, manage and scale
-your Automation Ops using All in One platform that provides task queue, runtime
-environment management, reports, alerts, logs and much more. [![BotCity
-Maestro](https://botcity.dev/github/readme/maestro/maestro.png)](https://
-botcity.atlassian.net/l/c/WWGswYRX) ### 2ï¸â£ Deploy with a Single Line Use
-BotCity command-line interface (CLI) to deploy your bot into a runtime
-environment with a single line: [![BotCity CLI](https://botcity.dev/github/
-readme/cli/botcli.gif)](https://botcity.atlassian.net/l/c/hJHE1ZFv) ### 3ï¸â£
-Manage your Task Queue [![BotCity Maestro Task Queue](https://botcity.dev/
-github/readme/maestro/tasks.png)](https://botcity.atlassian.net/l/c/gR3AAd2a)
-### 4ï¸â£ Manage your Runtime Environments [![BotCity Maestro Machines]
-(https://botcity.dev/github/readme/maestro/machines.png)](https://
-botcity.atlassian.net/l/c/uDB087nK) ### 5ï¸â£ Create Alerts and Reports from
-the Automation Execution [![BotCity Maestro Alerts](https://botcity.dev/github/
-readme/maestro/alerts.png)](https://botcity.atlassian.net/l/c/McH09qYw) ###
-6ï¸â£ Create Google Data Studio Dashboards [![BotCity Maestro Dashboards]
-(https://botcity.dev/github/readme/maestro/dashboard.png)](https://
-botcity.atlassian.net/l/c/Z1uMY1vX) ### 7ï¸â£ Create your Community Account
-We have a community account for hobbyists and students. Just signup and start
-automating. [![Sign Up](https://botcity.dev/github/readme/signup.png)](https://
-developers.botcity.dev/signup) ## ð¤ Contributing to BotCity Framework -
-[Guidelines](https://github.com/botcity-dev/botcity-framework-core-python/blob/
-main/.github/CONTRIBUTING.md) - [Documentation](https://botcity-dev.github.io/
-botcity-framework-core-python/) ## â Support ### ð Bug reports and ð
-Feature requests If you spot a problem, please let us know by following the
-template in here: [Report a bug](https://github.com/botcity-dev/botcity-
-framework-core-python/issues/new?template=bug-report.md). Ideas or suggestions
-for enhancements are more than welcome. Please use the following template in
-here: [Request feature](https://github.com/botcity-dev/botcity-framework-core-
-python/issues/new?template=feature-request.md). ### ð¢ Contact us If you have
-questions or comments in general about the framework, we want to know. You can
-choose between the channels the one that best fit you: - [BotCity Community](
+from-the-automation-execution) - [6ï¸â£ Create your Community Account]
+(#6ï¸â£--create-your-community-account) - [ð¤ Contributing to BotCity
+Framework](#-contributing-to-botcity-framework) - [â Support](#-support) -
+[ð Bug reports and ð Feature requests](#-bug-reports-and--feature-
+requests) - [ð¢ Contact us](#-contact-us) - [ð¡ Related Projects](#-
+related-projects) ## ð¤ Computer-vision based UI Automation Recognize and
+interact with UI elements using state-of-art computer vision module. Operate
+any UI interface independent of the technology or platform (desktop, web,
+terminal). ## ð Generate Python Code while Interacting with your UI Use our
+Development Tool alongside your favorite IDE to select UI components and
+generate python code. [![BotCity Studio](https://botcity.dev/github/readme/
+studio/studio.gif)](https://documentation.botcity.dev/studio/) [SIGN UP](https:
+//developers.botcity.dev/signup) and download our tools. ## ð Getting
+Started ### ð¦ Prerequisites * Python 3.7+ * python3-tk **(Linux Only)** *
+scrot **(Linux Only)** * xsel **(Linux Only)** * xclip **(Linux Only)** ###
+ð« Installing ```bash pip install botcity-framework-core ``` ### â­
+Developing Your First Automation [![First Automation](https://botcity.dev/
+github/readme/python-core/firstbot.png)](https://documentation.botcity.dev/
+tutorials/python-automations/desktop/) ## ð Documentation Documentation is
+available at https://documentation.botcity.dev/frameworks/desktop/. ## ð»
+Developers Portal [![Developers Portal](https://botcity.dev/github/readme/
+portal.png?)](https://documentation.botcity.dev) ## ð¬ Forum [![Forum](https:
+//botcity.dev/github/readme/forum.png)](https://community.botcity.dev/) ## ð
+BotCity Automation Platform BotCity is a platform to develop, deploy, manage
+and maintain automations. Automations can be developed in Python or Java using
+open-source libraries that are market standard. ### 1ï¸â£ All in One Platform
+Develop, deploy, manage and scale your Automation Ops using All in One platform
+that provides task queue, runtime environment management, reports, alerts, logs
+and much more. [![BotCity Maestro](https://botcity.dev/github/readme/maestro/
+maestro.png?)](https://documentation.botcity.dev/maestro/) ### 2ï¸â£ Deploy
+with a Single Line Use BotCity command-line interface (CLI) to deploy your bot
+into a runtime environment with a single line: [![BotCity CLI](https://
+botcity.dev/github/readme/cli/botcli.gif)](https://documentation.botcity.dev/
+cli/) ### 3ï¸â£ Manage your Task Queue [![BotCity Maestro Task Queue](https:/
+/botcity.dev/github/readme/maestro/tasks.png?)](https://
+documentation.botcity.dev/maestro/features/task-queue/) ### 4ï¸â£ Manage your
+Runtime Environments [![BotCity Maestro Machines](https://botcity.dev/github/
+readme/maestro/machines.png?)](https://documentation.botcity.dev/maestro/
+features/runners/) ### 5ï¸â£ Create Alerts and Reports from the Automation
+Execution #### Alerts [![BotCity Maestro Alerts](https://botcity.dev/github/
+readme/maestro/alerts.png?)](https://documentation.botcity.dev/maestro/
+features/alerts/) #### Execution Logs [![BotCity Maestro Alerts](https://
+botcity.dev/github/readme/maestro/logs.png?)](https://
+documentation.botcity.dev/maestro/features/logs/) ### 6ï¸â£ Create your
+Community Account We have a community account for hobbyists and students. Just
+signup and start automating. [![Sign Up](https://botcity.dev/github/readme/
+signup.png?)](https://developers.botcity.dev/signup) ## ð¤ Contributing to
+BotCity Framework - [Guidelines](https://github.com/botcity-dev/botcity-
+framework-core-python/blob/main/.github/CONTRIBUTING.md) - [Documentation]
+(https://documentation.botcity.dev/frameworks/desktop/) ## â Support ### ð
+Bug reports and ð Feature requests If you spot a problem, please let us know
+by following the template in here: [Report a bug](https://github.com/botcity-
+dev/botcity-framework-core-python/issues/new?template=bug-report.md). Ideas or
+suggestions for enhancements are more than welcome. Please use the following
+template in here: [Request feature](https://github.com/botcity-dev/botcity-
+framework-core-python/issues/new?template=feature-request.md). ### ð¢ Contact
+us If you have questions or comments in general about the framework, we want to
+know. You can choose between the channels the one that best fit you: - [BotCity
+Community](
 community.botcity.dev>) (Public) or you can [file a bug](https://github.com/
 botcity-dev/botcity-framework-core-python/issues/new?template=bug-report.md)
 and let us know where our documentation could be improved. ## ð¡ Related
 Projects [https://github-readme-stats.vercel.app/api/pin/?username=botcity-
 dev&repo=botcity-framework-web-python] [https://github-readme-stats.vercel.app/
 api/pin/?username=botcity-dev&repo=botcity-maestro-sdk-python]
```

### Comparing `botcity-framework-core-1.1.1/botcity/core/application/functions.py` & `botcity-framework-core-1.1.2/botcity/core/application/functions.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.1/botcity/core/application/utils.py` & `botcity-framework-core-1.1.2/botcity/core/application/utils.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.1/botcity/core/bot.py` & `botcity-framework-core-1.1.2/botcity/core/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import platform
 import psutil
 import random
 import subprocess
 import time
 import webbrowser
-from typing import Union, List
+from typing import Union
 
 
 import pyperclip
 from botcity.base import BaseBot, State
 from botcity.base.utils import is_retina, only_if_element
 from PIL import Image, ImageGrab
 from psutil import Process
@@ -442,15 +442,15 @@
 
         Returns:
             element (NamedTuple): The element coordinates. None if not found.
         """
         return self.find_until(label, x, y, width, height, threshold=threshold, matching=matching,
                                waiting_time=waiting_time, best=best, grayscale=True)
 
-    def find_process(self, name: str = None, pid: str = None) -> List[Process]:
+    def find_process(self, name: str = None, pid: str = None) -> Process:
         """
         Find a process by name or PID
 
         Args:
             name (str): The process name.
             pid (str) or (int): The PID (Process Identifier).
 
@@ -504,14 +504,20 @@
         Args:
             filepath (str, optional): The filepath in which to save the screenshot. Defaults to None.
             region (tuple, optional): Bounding box containing left, top, width and height to crop screenshot.
 
         Returns:
             Image: The screenshot Image object
         """
+        if region:
+            x, y, width, height = region
+            width = x + width
+            height = y + height
+            region = (x, y, width, height)
+
         img = ImageGrab.grab(bbox=region)
         if filepath:
             img.save(filepath)
         return img
 
     def get_screenshot(self, filepath=None, region=None):
         """
```

### Comparing `botcity-framework-core-1.1.1/botcity/core/cv2find.py` & `botcity-framework-core-1.1.2/botcity/core/cv2find.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.1/botcity/core/input_utils.py` & `botcity-framework-core-1.1.2/botcity/core/input_utils.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.1/botcity/core/os_compat.py` & `botcity-framework-core-1.1.2/botcity/core/os_compat.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.1/botcity_framework_core.egg-info/PKG-INFO` & `botcity-framework-core-1.1.2/botcity_framework_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: botcity-framework-core
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://www.github.com/botcity-dev/botcity-framework-core-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <h1 align="center">BotCity Framework Core - Python</h1>
 
   <p align="center">
-    <strong>« Explore Framework <a href="https://botcity-dev.github.io/botcity-framework-core-python/">docs</a> »</strong>
+    <strong>« Explore Framework <a href="https://documentation.botcity.dev/frameworks/desktop/">docs</a> »</strong>
   </p>
 </p>
 
 <br>
 
 ## Summary  <!-- omit in toc -->
 
@@ -29,16 +29,15 @@
 - [💬 Forum](#-forum)
 - [🌎 BotCity Automation Platform](#-botcity-automation-platform)
   - [1️⃣  All in One Platform](#1️⃣--all-in-one-platform)
   - [2️⃣  Deploy with a Single Line](#2️⃣--deploy-with-a-single-line)
   - [3️⃣  Manage your Task Queue](#3️⃣--manage-your-task-queue)
   - [4️⃣  Manage your Runtime Environments](#4️⃣--manage-your-runtime-environments)
   - [5️⃣  Create Alerts and Reports from the Automation Execution](#5️⃣--create-alerts-and-reports-from-the-automation-execution)
-  - [6️⃣  Create Google Data Studio Dashboards](#6️⃣--create-google-data-studio-dashboards)
-  - [7️⃣  Create your Community Account](#7️⃣--create-your-community-account)
+  - [6️⃣  Create your Community Account](#6️⃣--create-your-community-account)
 - [🤝 Contributing to BotCity Framework](#-contributing-to-botcity-framework)
 - [⛑ Support](#-support)
   - [🐛 Bug reports and 💎 Feature requests](#-bug-reports-and--feature-requests)
   - [📢 Contact us](#-contact-us)
 - [💡 Related Projects](#-related-projects)
 
 
@@ -48,15 +47,15 @@
 
 Operate any UI interface independent of the technology or platform (desktop, web, terminal).
 
 ## 🐍 Generate Python Code while Interacting with your UI
 
 Use our Development Tool alongside your favorite IDE to select UI components and generate python code.
 
-[![BotCity Studio](https://botcity.dev/github/readme/studio/studio.gif)](https://botcity.atlassian.net/l/c/eBJ6bLLV)
+[![BotCity Studio](https://botcity.dev/github/readme/studio/studio.gif)](https://documentation.botcity.dev/studio/)
 
 [SIGN UP](https://developers.botcity.dev/signup) and download our tools.
 
 
 ## 🚀 Getting Started
 
 ### 📦 Prerequisites
@@ -70,69 +69,68 @@
 
 ```bash
 pip install botcity-framework-core
 ```
 
 ### ⭐ Developing Your First Automation
 
-[![First Automation](https://botcity.dev/github/readme/python-core/firstbot.png)](https://botcity-dev.github.io/botcity-framework-core-python/intro/)
+[![First Automation](https://botcity.dev/github/readme/python-core/firstbot.png)](https://documentation.botcity.dev/tutorials/python-automations/desktop/)
 
 ## 📚 Documentation
 
-Documentation is available at https://botcity-dev.github.io/botcity-framework-core-python.
+Documentation is available at https://documentation.botcity.dev/frameworks/desktop/.
 
 ## 💻 Developers Portal
 
-[![Developers Portal](https://botcity.dev/github/readme/portal.png)](https://documentation.botcity.dev)
+[![Developers Portal](https://botcity.dev/github/readme/portal.png?)](https://documentation.botcity.dev)
 
 ## 💬 Forum
 
 [![Forum](https://botcity.dev/github/readme/forum.png)](https://community.botcity.dev/)
 
 ## 🌎 BotCity Automation Platform
 BotCity is a platform to develop, deploy, manage and maintain automations. Automations can be developed in Python or Java using open-source libraries that are market standard.
 
 ### 1️⃣  All in One Platform
 Develop, deploy, manage and scale your Automation Ops using All in One platform that provides task queue, runtime environment management, reports, alerts, logs and much more.
 
-[![BotCity Maestro](https://botcity.dev/github/readme/maestro/maestro.png)](https://botcity.atlassian.net/l/c/WWGswYRX)
+[![BotCity Maestro](https://botcity.dev/github/readme/maestro/maestro.png?)](https://documentation.botcity.dev/maestro/)
 
 ### 2️⃣  Deploy with a Single Line
 
 Use BotCity command-line interface (CLI) to deploy your bot into a runtime environment with a single line:
 
-[![BotCity CLI](https://botcity.dev/github/readme/cli/botcli.gif)](https://botcity.atlassian.net/l/c/hJHE1ZFv)
+[![BotCity CLI](https://botcity.dev/github/readme/cli/botcli.gif)](https://documentation.botcity.dev/cli/)
 
 ### 3️⃣  Manage your Task Queue
 
-[![BotCity Maestro Task Queue](https://botcity.dev/github/readme/maestro/tasks.png)](https://botcity.atlassian.net/l/c/gR3AAd2a)
+[![BotCity Maestro Task Queue](https://botcity.dev/github/readme/maestro/tasks.png?)](https://documentation.botcity.dev/maestro/features/task-queue/)
 
 ### 4️⃣  Manage your Runtime Environments
 
-[![BotCity Maestro Machines](https://botcity.dev/github/readme/maestro/machines.png)](https://botcity.atlassian.net/l/c/uDB087nK)
+[![BotCity Maestro Machines](https://botcity.dev/github/readme/maestro/machines.png?)](https://documentation.botcity.dev/maestro/features/runners/)
 
 ### 5️⃣  Create Alerts and Reports from the Automation Execution
 
-[![BotCity Maestro Alerts](https://botcity.dev/github/readme/maestro/alerts.png)](https://botcity.atlassian.net/l/c/McH09qYw)
+#### Alerts
+[![BotCity Maestro Alerts](https://botcity.dev/github/readme/maestro/alerts.png?)](https://documentation.botcity.dev/maestro/features/alerts/)
 
-### 6️⃣  Create Google Data Studio Dashboards
+#### Execution Logs
+[![BotCity Maestro Alerts](https://botcity.dev/github/readme/maestro/logs.png?)](https://documentation.botcity.dev/maestro/features/logs/)
 
-[![BotCity Maestro Dashboards](https://botcity.dev/github/readme/maestro/dashboard.png)](https://botcity.atlassian.net/l/c/Z1uMY1vX)
-
-### 7️⃣  Create your Community Account
+### 6️⃣  Create your Community Account
 
 We have a community account for hobbyists and students. Just signup and start automating.
 
-[![Sign Up](https://botcity.dev/github/readme/signup.png)](https://developers.botcity.dev/signup)
-
+[![Sign Up](https://botcity.dev/github/readme/signup.png?)](https://developers.botcity.dev/signup)
 
 ## 🤝 Contributing to BotCity Framework
 
 - [Guidelines](https://github.com/botcity-dev/botcity-framework-core-python/blob/main/.github/CONTRIBUTING.md)
-- [Documentation](https://botcity-dev.github.io/botcity-framework-core-python/)
+- [Documentation](https://documentation.botcity.dev/frameworks/desktop/)
 
 ## ⛑ Support
 
 ### 🐛 Bug reports and 💎 Feature requests
 
 If you spot a problem, please let us know by following the template in
 here: [Report a bug](https://github.com/botcity-dev/botcity-framework-core-python/issues/new?template=bug-report.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botcity-framework-core Version: 1.1.1 Home-page:
+Metadata-Version: 2.1 Name: botcity-framework-core Version: 1.1.2 Home-page:
 https://www.github.com/botcity-dev/botcity-framework-core-python Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
                  ****** BotCity Framework Core - Python ******
                          Â« Explore Framework docs Â»
 
 ## Summary  - [ð¤ Computer-vision based UI Automation](#-computer-vision-
 based-ui-automation) - [ð Generate Python Code while Interacting with your
@@ -13,72 +13,72 @@
 [ð» Developers Portal](#-developers-portal) - [ð¬ Forum](#-forum) - [ð
 BotCity Automation Platform](#-botcity-automation-platform) - [1ï¸â£ All in
 One Platform](#1ï¸â£--all-in-one-platform) - [2ï¸â£ Deploy with a Single
 Line](#2ï¸â£--deploy-with-a-single-line) - [3ï¸â£ Manage your Task Queue]
 (#3ï¸â£--manage-your-task-queue) - [4ï¸â£ Manage your Runtime Environments]
 (#4ï¸â£--manage-your-runtime-environments) - [5ï¸â£ Create Alerts and
 Reports from the Automation Execution](#5ï¸â£--create-alerts-and-reports-
-from-the-automation-execution) - [6ï¸â£ Create Google Data Studio Dashboards]
-(#6ï¸â£--create-google-data-studio-dashboards) - [7ï¸â£ Create your
-Community Account](#7ï¸â£--create-your-community-account) - [ð¤
-Contributing to BotCity Framework](#-contributing-to-botcity-framework) - [â
-Support](#-support) - [ð Bug reports and ð Feature requests](#-bug-
-reports-and--feature-requests) - [ð¢ Contact us](#-contact-us) - [ð¡
-Related Projects](#-related-projects) ## ð¤ Computer-vision based UI
-Automation Recognize and interact with UI elements using state-of-art computer
-vision module. Operate any UI interface independent of the technology or
-platform (desktop, web, terminal). ## ð Generate Python Code while
-Interacting with your UI Use our Development Tool alongside your favorite IDE
-to select UI components and generate python code. [![BotCity Studio](https://
-botcity.dev/github/readme/studio/studio.gif)](https://botcity.atlassian.net/l/
-c/eBJ6bLLV) [SIGN UP](https://developers.botcity.dev/signup) and download our
-tools. ## ð Getting Started ### ð¦ Prerequisites * Python 3.7+ * python3-
-tk **(Linux Only)** * scrot **(Linux Only)** * xsel **(Linux Only)** * xclip **
-(Linux Only)** ### ð« Installing ```bash pip install botcity-framework-core
-``` ### â­ Developing Your First Automation [![First Automation](https://
-botcity.dev/github/readme/python-core/firstbot.png)](https://botcity-
-dev.github.io/botcity-framework-core-python/intro/) ## ð Documentation
-Documentation is available at https://botcity-dev.github.io/botcity-framework-
-core-python. ## ð» Developers Portal [![Developers Portal](https://
-botcity.dev/github/readme/portal.png)](https://documentation.botcity.dev) ##
-ð¬ Forum [![Forum](https://botcity.dev/github/readme/forum.png)](https://
-community.botcity.dev/) ## ð BotCity Automation Platform BotCity is a
-platform to develop, deploy, manage and maintain automations. Automations can
-be developed in Python or Java using open-source libraries that are market
-standard. ### 1ï¸â£ All in One Platform Develop, deploy, manage and scale
-your Automation Ops using All in One platform that provides task queue, runtime
-environment management, reports, alerts, logs and much more. [![BotCity
-Maestro](https://botcity.dev/github/readme/maestro/maestro.png)](https://
-botcity.atlassian.net/l/c/WWGswYRX) ### 2ï¸â£ Deploy with a Single Line Use
-BotCity command-line interface (CLI) to deploy your bot into a runtime
-environment with a single line: [![BotCity CLI](https://botcity.dev/github/
-readme/cli/botcli.gif)](https://botcity.atlassian.net/l/c/hJHE1ZFv) ### 3ï¸â£
-Manage your Task Queue [![BotCity Maestro Task Queue](https://botcity.dev/
-github/readme/maestro/tasks.png)](https://botcity.atlassian.net/l/c/gR3AAd2a)
-### 4ï¸â£ Manage your Runtime Environments [![BotCity Maestro Machines]
-(https://botcity.dev/github/readme/maestro/machines.png)](https://
-botcity.atlassian.net/l/c/uDB087nK) ### 5ï¸â£ Create Alerts and Reports from
-the Automation Execution [![BotCity Maestro Alerts](https://botcity.dev/github/
-readme/maestro/alerts.png)](https://botcity.atlassian.net/l/c/McH09qYw) ###
-6ï¸â£ Create Google Data Studio Dashboards [![BotCity Maestro Dashboards]
-(https://botcity.dev/github/readme/maestro/dashboard.png)](https://
-botcity.atlassian.net/l/c/Z1uMY1vX) ### 7ï¸â£ Create your Community Account
-We have a community account for hobbyists and students. Just signup and start
-automating. [![Sign Up](https://botcity.dev/github/readme/signup.png)](https://
-developers.botcity.dev/signup) ## ð¤ Contributing to BotCity Framework -
-[Guidelines](https://github.com/botcity-dev/botcity-framework-core-python/blob/
-main/.github/CONTRIBUTING.md) - [Documentation](https://botcity-dev.github.io/
-botcity-framework-core-python/) ## â Support ### ð Bug reports and ð
-Feature requests If you spot a problem, please let us know by following the
-template in here: [Report a bug](https://github.com/botcity-dev/botcity-
-framework-core-python/issues/new?template=bug-report.md). Ideas or suggestions
-for enhancements are more than welcome. Please use the following template in
-here: [Request feature](https://github.com/botcity-dev/botcity-framework-core-
-python/issues/new?template=feature-request.md). ### ð¢ Contact us If you have
-questions or comments in general about the framework, we want to know. You can
-choose between the channels the one that best fit you: - [BotCity Community](
+from-the-automation-execution) - [6ï¸â£ Create your Community Account]
+(#6ï¸â£--create-your-community-account) - [ð¤ Contributing to BotCity
+Framework](#-contributing-to-botcity-framework) - [â Support](#-support) -
+[ð Bug reports and ð Feature requests](#-bug-reports-and--feature-
+requests) - [ð¢ Contact us](#-contact-us) - [ð¡ Related Projects](#-
+related-projects) ## ð¤ Computer-vision based UI Automation Recognize and
+interact with UI elements using state-of-art computer vision module. Operate
+any UI interface independent of the technology or platform (desktop, web,
+terminal). ## ð Generate Python Code while Interacting with your UI Use our
+Development Tool alongside your favorite IDE to select UI components and
+generate python code. [![BotCity Studio](https://botcity.dev/github/readme/
+studio/studio.gif)](https://documentation.botcity.dev/studio/) [SIGN UP](https:
+//developers.botcity.dev/signup) and download our tools. ## ð Getting
+Started ### ð¦ Prerequisites * Python 3.7+ * python3-tk **(Linux Only)** *
+scrot **(Linux Only)** * xsel **(Linux Only)** * xclip **(Linux Only)** ###
+ð« Installing ```bash pip install botcity-framework-core ``` ### â­
+Developing Your First Automation [![First Automation](https://botcity.dev/
+github/readme/python-core/firstbot.png)](https://documentation.botcity.dev/
+tutorials/python-automations/desktop/) ## ð Documentation Documentation is
+available at https://documentation.botcity.dev/frameworks/desktop/. ## ð»
+Developers Portal [![Developers Portal](https://botcity.dev/github/readme/
+portal.png?)](https://documentation.botcity.dev) ## ð¬ Forum [![Forum](https:
+//botcity.dev/github/readme/forum.png)](https://community.botcity.dev/) ## ð
+BotCity Automation Platform BotCity is a platform to develop, deploy, manage
+and maintain automations. Automations can be developed in Python or Java using
+open-source libraries that are market standard. ### 1ï¸â£ All in One Platform
+Develop, deploy, manage and scale your Automation Ops using All in One platform
+that provides task queue, runtime environment management, reports, alerts, logs
+and much more. [![BotCity Maestro](https://botcity.dev/github/readme/maestro/
+maestro.png?)](https://documentation.botcity.dev/maestro/) ### 2ï¸â£ Deploy
+with a Single Line Use BotCity command-line interface (CLI) to deploy your bot
+into a runtime environment with a single line: [![BotCity CLI](https://
+botcity.dev/github/readme/cli/botcli.gif)](https://documentation.botcity.dev/
+cli/) ### 3ï¸â£ Manage your Task Queue [![BotCity Maestro Task Queue](https:/
+/botcity.dev/github/readme/maestro/tasks.png?)](https://
+documentation.botcity.dev/maestro/features/task-queue/) ### 4ï¸â£ Manage your
+Runtime Environments [![BotCity Maestro Machines](https://botcity.dev/github/
+readme/maestro/machines.png?)](https://documentation.botcity.dev/maestro/
+features/runners/) ### 5ï¸â£ Create Alerts and Reports from the Automation
+Execution #### Alerts [![BotCity Maestro Alerts](https://botcity.dev/github/
+readme/maestro/alerts.png?)](https://documentation.botcity.dev/maestro/
+features/alerts/) #### Execution Logs [![BotCity Maestro Alerts](https://
+botcity.dev/github/readme/maestro/logs.png?)](https://
+documentation.botcity.dev/maestro/features/logs/) ### 6ï¸â£ Create your
+Community Account We have a community account for hobbyists and students. Just
+signup and start automating. [![Sign Up](https://botcity.dev/github/readme/
+signup.png?)](https://developers.botcity.dev/signup) ## ð¤ Contributing to
+BotCity Framework - [Guidelines](https://github.com/botcity-dev/botcity-
+framework-core-python/blob/main/.github/CONTRIBUTING.md) - [Documentation]
+(https://documentation.botcity.dev/frameworks/desktop/) ## â Support ### ð
+Bug reports and ð Feature requests If you spot a problem, please let us know
+by following the template in here: [Report a bug](https://github.com/botcity-
+dev/botcity-framework-core-python/issues/new?template=bug-report.md). Ideas or
+suggestions for enhancements are more than welcome. Please use the following
+template in here: [Request feature](https://github.com/botcity-dev/botcity-
+framework-core-python/issues/new?template=feature-request.md). ### ð¢ Contact
+us If you have questions or comments in general about the framework, we want to
+know. You can choose between the channels the one that best fit you: - [BotCity
+Community](
 community.botcity.dev>) (Public) or you can [file a bug](https://github.com/
 botcity-dev/botcity-framework-core-python/issues/new?template=bug-report.md)
 and let us know where our documentation could be improved. ## ð¡ Related
 Projects [https://github-readme-stats.vercel.app/api/pin/?username=botcity-
 dev&repo=botcity-framework-web-python] [https://github-readme-stats.vercel.app/
 api/pin/?username=botcity-dev&repo=botcity-maestro-sdk-python]
```

### Comparing `botcity-framework-core-1.1.1/botcity_framework_core.egg-info/SOURCES.txt` & `botcity-framework-core-1.1.2/botcity_framework_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.1/setup.py` & `botcity-framework-core-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.1/versioneer.py` & `botcity-framework-core-1.1.2/versioneer.py`

 * *Files identical despite different names*

